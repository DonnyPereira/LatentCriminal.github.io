+++
title = "Week 3 Sprint evaluation"
date = "2020-02-09"
author = "Donny"
cover = ""
description = "A reflection of the progress made in week 3"
+++

# Mr Robot

# Engagement

As soon as the site was live, I spent an obscene amount of time on the actual content almost forgetting my task was to hack the box. Recalling the pent tester methodology below, the first step requires Information gathering. 

![Mr%20Robot/Untitled.png](Mr%20Robot/Untitled.png)

# Information Gathering

The most logical simple step was to scan for ports using nmap, luckily it comes pre-installed on linux.

![Mr%20Robot/Untitled%201.png](Mr%20Robot/Untitled%201.png)

Once the scan was finished, I saw that 2 ports were open, one was http on port 80 and the other was SSL on port 443. I also saw that the website was running apache. There was no useful information to me so I tried something else. I knew that Directory traversal could be used to find arbitrary files on a server. To my luck I found the etc/shadow directory was running a wordpress page. 

![Mr%20Robot/Untitled%202.png](Mr%20Robot/Untitled%202.png)

# Vulnerability Assessment

And it just so happens that there is a tool that scans wordpress sites that I can use. Even better, it comes pre-installed on Kali. I also looked at the page source but found nothing. I whip out my terminal, and type in the following command:

    wpscan --url <ip address>

I find some interesting things, mainly that the version running is 4.3.1 released in 2015. I also find that this version is insecure. I find the robots.txt file which was the fist key - WOOOOO! 

![Mr%20Robot/Untitled%203.png](Mr%20Robot/Untitled%203.png)

There is also a dictionary file that after consulting with Max I realised I could use to get the password for the admin. Here is the robots page with the first key and the dictionary file.

![Mr%20Robot/Untitled%204.png](Mr%20Robot/Untitled%204.png)

I had watched the show and knew that Elliot was the name of the main character so I changed my command from:

    wpscan --url <ip Address> -U robotlist.txt -P robotlist.txt  

to 

    wpscan --url <ip Address> --passwords RobotWordList --usernames elliot
    //Can also we written as:
    wpscan --url <ip Address> -P RobotWordList -U elliot

Some things to note:

- Robotlist.txt  and RobotWordList are have the same content, it is the fsocity.dic file I got from the robots.txt page. The reason for this change is because I thought the reason for the abnormally long waiting time was that the duplicates had not been removed properly. Therefore, I used the command below to redo the process of removing the duplicate entries and thus had to make another file.

    cat robotlist.txt | sort | uniq > RobotWordList

- The second thing to note is that the -U = —username and the -P = —passwords are the same parameter.  Just different ways of writing the same thing.

After I tried the second command I had the results in about 10 minutes, as opposed to hours of waiting. A major problem with this box is that for some reasons, windows loses internet connection at certain intervals so I have to constantly reconnect to the VPN and deploy the machine, I cannot wait to fully convert to Linux. Back to the box, this is the result I got: 

![Mr%20Robot/Capture.png](Mr%20Robot/Capture.png)

After putting it into the login form to confirm: 

![Mr%20Robot/Capture%201.png](Mr%20Robot/Capture%201.png)

After many long hours of struggle and hardship, I was able to get admin access onto the wordpress site. The next question is - "What do I do next".

Answer - ask Google.

# Exploitation

After just a quick youtube video I knew exactly what to do. This is the process:

For the reverse shell code, you could download the zip file from a source like Pentest Monkey or copy and paste the code from the GitHub into the 404.php template. I didn't bother with downloading a malicious plugin and installing it either. The resource I was using at the time showed me that it was already included in kali.

![Mr%20Robot/Untitled%205.png](Mr%20Robot/Untitled%205.png)

I simply changed my IP address which I gained from using "ifconfig" and also the port number "1234" since it was easy to remember. I could've picked any theme but I chose the 404.php page because it is more stealthy. In other words, the code will cause the site to appear to hang and thus nothing will appear to be suspicious. However, my backdoor runs and I have access. 

![Mr%20Robot/Untitled%206.png](Mr%20Robot/Untitled%206.png)

Using netcat, I started listening on port 1234. I refreshed the page and then had access. I also checked who I was using "whoami" and then tested If had sudo privileges using "sudo -v". I didn't but I wasn't expecting it to be that easy. 

![Mr%20Robot/Untitled%207.png](Mr%20Robot/Untitled%207.png)

Then I went into the "home" directory, then from there I saw there was another user named Robot. I  also saw that with "robot" was another key and an m5d hashed password. I did not have access to the key as daemon, but I used an online MD5 cracker to get the password. Then I used a python script to import a terminal shell so that I could set user as Robot. After I was logged in as robot I was able to get the second flag.

![Mr%20Robot/Untitled%208.png](Mr%20Robot/Untitled%208.png)

The last steps were a bit of a pain but I managed it. I knew the last step was privilege escalation. Now privilege escalation is a huge rabbit hole. So I just watch a YouTube video on common privilege escalation.

![Mr%20Robot/Untitled%209.png](Mr%20Robot/Untitled%209.png)

I was talking to max trying to understand SUID better because there were gaps in my knowledge. The I realised that Nmap was executable by robot but is owned by root. Using gtfobins - [https://gtfobins.github.io/](https://gtfobins.github.io/) the Nmap had an entry to execute shell commands:

![Mr%20Robot/Untitled%2010.png](Mr%20Robot/Untitled%2010.png)

I had to start nmap in interactive mode and then the "!sh" command and then see that I am root user.

![Mr%20Robot/Untitled%2011.png](Mr%20Robot/Untitled%2011.png)

# Reporting

This box was a challenge to be sure, and I made many errors. Some of them very stupid, some of them showcased the gaps in my knowledge. Nevertheless I really enjoyed rooting this box, I learnt a lot and I am motivated to try another box soon. 

![Mr%20Robot/Capture%202.png](Mr%20Robot/Capture%202.png)