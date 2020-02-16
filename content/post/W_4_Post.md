+++
title = "Week 4 Reflection"
date = "2020-02-16"
author = "Donny"
cover = ""
description = "A reflection of the progress made in week 3"
+++

### SLO1 — Introduction 
The theme of this week is web application pen testing.

 I have also gotten a lot better at using a schedule. One thing I have found which I have included in my portfolio this week is my declaration of goals, justifications for them, and methods for achievement . By clearly defining my goals in a non-abstract concrete way, I have a target to aim at and I can clearly see if my actions are producing positive/negative results.  The methods of achievement are my way of breaking the goal down into manageable chunks and clearly defining the path I will take to achieve them. This is really important because I use this to make my schedule.



### Goals
	1) My goals for this week are to properly set up my schedule such that it accommodates for my practising of my CompTIA certifications and wargames. Furthermore, I have to do this in such a way that I can still adhere to responsibilities I already have, that being work, the deliverable, gym, and Muay Thai Kickboxing. I also have to make sure to look after my mental and physical health by making sure I give myself breaks and not burn out by grinding as well as making time for friends.
	
	2) I also wish to be much more efficient. I am aware that even with a good schedule if I don’t do things properly the schedule is pointless. I tend to procrastinate a lot mostly through YouTube and also by talking to my friend on social media.
	
	3) I would like to learn about as much of the web pen testing tools as possible, Document whatever I have done on the and upload it all on Sunday.
	
	4) I would like to start on each war game.
	
	5) If possible I would also like to start working on my Raspberry Pi.

    6) Remember things I have learnt

### How it will be achieved
* Since I have most things already on my Google Calendar, I simply have to find out how much time per week I will allocate to studying the CompTIA certifications. I will complete this by Monday so I can schedule them in for the rest of the week.
	
- Every day I will document how much of the day I did well and give it a score out of 100 starting from Monday. Also I will aim for accumulative improvement because it will take time for me to develop focus. So, if I only manage to hit one day with 50% accuracy, then my goal the next day is to achieve at least 51%. In other words, the goal is to finish the day better than I was at the start and over time become more efficient. 
	
- I will aim to finish my part of the deliverable as soon as possible thus giving me more time throughout the week to study this. I will utilise the resources on the week 3 slides especially the practical ones because I learn best through labs.  
	
- I will allocate at least 1 hour of these week to a particular war games. It isn't much but since there are so many wargames I feel this will suffice. I will also make sure to write down every step I so that I can view them at any time and see my though processes as well as learn from my mistakes. 

- I have bootcamp workshop that gets right into starting with a raspberry Pi, I will spend at least 2 hours this week just getting into it at doing what I can in those 2 hours even though it might not be much, it's still a start.

-I discovered this really cool app called Anki, it is a flashcard app that syncs across mobile and pc. It’s has spaced repitition, in other words if you get an answer right it won't show that card again for an extended period of time, If you get it wrong however it will show you that card again in a shorter period of time. This really helps me because I tend to forget basics after I've studied them but with this app I can resolve that.

# Sprint Post

Monday 

---

Once again, a stand-up meeting to start the week. It's nice to see everyone has come along way from where they began at the start of the subject. My objective for this week is to be more studious and disciplined when it comes to times allocated for study. 

The deliverable for this week is interesting. Rather than a presentation, we have a practical
assessment where we have to choose a box and then break into it. The goal is to
gain the highest level of authority in the box. It's  a big step up the projects we've had and is
definitely a plunge into the deep end. I followed along as best as I could but I know that this deliverable will definitely test me. The notes I took down are a bit hard to read since I write one-liners in the interest of time.

![Sprint%20Post/Untitled.png](Sprint%20Post/Untitled.png)

It was hard to digest all of the information in Jason's demonstration. Although I understand what happened, it's still a lot of information to process. Even though this deliverable will be incredibly difficult, I am looking forward to it since it will be even better when I overcome it. Google, YouTube and the stack skills will be my most visited sites, I can already tell. It is also great practice for the assignment at the end where we will have to break into another system. 

I still need to learn how to use things like burp suite, vim, and Metasploit. Another interesting point that Larry pointed out is that we should be up to level 15-20  in both bandit and Natas in order to really get a good understanding. I am only up to level 4 in Natas and level 6 in Bandit. I will focus on getting that done as soon as possible. We also tried our hand at the beginner Box, it was the Basic pen testing 1 box on Vulnhub. I wasn't able to do much at University because the demonstration was long and I spent most of my time trying to understand why certain things were done. For the most part I spent the time inspecting the box using nmap as well as looking at the source web app. Luckily for me (and the rest of the class), Yukari had not only recorded, but also uploaded the whole process of Jason rooting the Wakanda box to her YouTube channel.
 

![Sprint%20Post/Untitled%201.png](Sprint%20Post/Untitled%201.png)

When I got home I worked on the machine some more.  I realised with some hints form Anthony in class that the box was running FTP. I simply looked up the exploit on the Metasploit database and filled out the options.

![Sprint%20Post/Untitled%202.png](Sprint%20Post/Untitled%202.png)

Using metasploit didn't work at first but after using a YouTube video I was able to get into the box. It turned out I was inputting a value in the wrong place. After that I used the "whoami" command to observe my privilege level. It was root and so I had cracked the box.  I see now why it was a beginner task but I'm glad I'm happy I cracked it, especially because I had Kick-boxing that night so I didn't have much time to work on it. 

 

Tuesday

---

I finally finished touching up my resume and sent it to Max. Using Microsoft Word to craft resumes
is a pain in the ass, I might have to re-learn how to use Latex. I also discovered Notion which is one of the most spectacular note-taking programs that I have ever seen. It combines the automatic multi-device sync ability of OneNote with the powerful note-editing abilities of Latex, although to a
lesser extent. It's wonderful for taking notes when coding or just normal notes, I haven't tried it for mathematics. 

![Sprint%20Post/Untitled%203.png](Sprint%20Post/Untitled%203.png)

I talked to Max about my experiences with my basic pen testing 1, he usually gives helpful advice and has a lot of experience that I can glean from. He asked me if I had found the password which I didn't do since I got root and just assumed I was done. After googling I found out that you can break hashes using John the ripper or hash cat, and If I am really lazy I can also use online hash crackers.

![Sprint%20Post/Untitled%204.png](Sprint%20Post/Untitled%204.png)

In fact Max was actually the one who one who challenged me with the Mr Robot box. I loved the show and more importantly he had asked me if I wanted a challenge. I did want a challenge, firstly, because it would would boost my confidence doing it, and secondly, because I would learn a lot in the process. I did start the Box and it was pretty fun. I'll admit, the content was very interesting and I low-key spent more time on it than I should of. I did manage to get the first flag of the box which was good, it was simply in the robots.txt file of the site. I though that was pretty comical since the box is called "Mr. Robot". There were 3 flags (the box called them "keys") in total for me to get. I wasn't able to do much today since I spent quite some time figuring out how to get the box running and more so because I had work. The important thing was that I had started and that I already had the first key.

Wednesday

---

Today was not as productive as I would have liked it to be. Even though the day is optional, I came in anyway because I knew I would need help with the challenge. I got a bit further in the box by using directory traversal and realizing the website used WordPress. I also knew of a particular tool that would help me bypass the admin login page of WordPress to give me administrative power. From there it should have been easy. The problem was that I used wpscan wrong and then deduced that wpscan was the wrong tool. That was mistake number 1. I then went straight to google to find other ways to hack the site.

![Sprint%20Post/Untitled%205.png](Sprint%20Post/Untitled%205.png)

One of the solutions involved using burpsuite, Max informed me that using burpsuite wasn't necessary, yet I persisted anyways. That was mistake number 2.

![Sprint%20Post/Untitled%206.png](Sprint%20Post/Untitled%206.png)

The reason for that being a mistake was simply because Burp suite didn't work on my kali. And getting to to work yielded no results. I lost so much time trying to get it to work. I deleted and re-imported certificates, I removed and re-added Foxy Proxy, et cetera. After hours of trial an error, and with the help of the tutors, the problem seemed to be my version of Kali. I also met Jai which was cool, had some funny banter with him that kind of lifted the mood. Nevertheless not being able to use Burp suite was driving me up the wall. The internet was slow for some reason so I couldn't use it to re-download the 2020 kali. Even Jai tried to help out using his hotspot but it still was too slow. The only solution was Max who had kindly offered to let me borrow his SSD to download the kali distribution I needed. The first time I used his SSD I did not realize that his version had I3 which made the distro unusable for me. Luckily, for me Max once again helped me out by sitting down with me and showing me that he had another version of kali on his SSD and by the end of the day we got it done.

![Sprint%20Post/Untitled%207.png](Sprint%20Post/Untitled%207.png)

Thursday

---

Finally got burp suite working after the demo today around lunchtime. I don't know what the problem was exactly, I upgraded my kali with another kali distro that Max kindly gave me yesterday and it solved the problem. Another problem that came up though is space. My laptop has enough space for now to run the VM kali. However, windows is always increasing the amount of data it takes from me so hopefully my laptop holds out until next week when I can utilize the SSD for the course.

On the bright side, I now have notion which is huge help for someone like me who prioritizes organisation and flexibility. Onenote is good only because of its cross-device functionality. The problem is that it is not that good at facilitating note taking and the sync process can be a bit dodgy at times. Notion also has the advantage of text driven modification which really helped with note taking during the demo. For example, Jason was using Enumeration at one point which I had only heard people mention before. Thus, when he was using Enumeration to find shared directories,   I was able to easily take down notes with minimal effort. If there was a command I hadn't seen before, I simply took down the command using "/code" and then proceeded with the command. I didn't even need to use the mousepad. The result was effective notes that was clean and organised (shown below):

![Sprint%20Post/Untitled%208.png](Sprint%20Post/Untitled%208.png)

After lunch, I resumed my efforts on my box. I knew with my commitments to work and other things that I couldn't waste time since this box was challenging or at least reputed to be so. I also convinced Mihailo to do the same box so that he actually challenged himself rather than just complain about not being smart. Here is something else I figured out:

You have to keep the openvpn script running.

I already had the IP address of the website, so I simply would use nmap to investigate for any open and/or vulnerable. When I did so I'd go to the shell where I connected to openvpn, use Ctrl+C and then use Nmap. My hypothesis was that when I Initially connected to the vpn, it would stay open. But whenever I did the Nmap wouldn't get results that I wanted. Thankfully in today's class, Max spotted my mistake and let me know that I had to open another terminal and use Nmap there. Luckily I had that error fixed before work so that the next day I could be more productive.

Friday 

---

The theme of today is "you win some you lose some". This isn't some cliché either that I am adding to my reflection, I mean this literally. As you will see from the write up for my box, I spent a large amount of time trying to bypass the WordPress login, specifcally 5 hours. The reason for this was that WPScan didn't work for me, well in actuality I didn't use it properly. Because I thought it didn't work I used google, youtube and anything I could find to try and crack the login. As it turns out, there are so many ways to get past a WordPress login. I of course, used as many as I could.

The methods involving Burp suite took the longest simply because I had to learn how to use it and I also had to learn about http messages in general. I went through so many resources, and each time I hit a dead end. The reason I say the theme of today is as such is because although I lost significant time with all these methods, I learnt a lot about the many different ways to exploit wordpress. I also learnt about things like "?author=1" and "xml=rcp" which I had no idea about. Of course after I had exhausted so many methods I was at my wits end. Logically I asked Max for a clue or a hint.

![Sprint%20Post/Untitled%209.png](Sprint%20Post/Untitled%209.png)

I learnt a lot like being able to look through man pages using "/", search for the command and then hitting return. Max is helpful in that he doesn't give me the answer but will tell me if things are just out right wrong. By learning what things are wrong, I may not know what to do, but I know what not to do which helps me focus on finding what I need. I had discovered a dictionary list previously which Max reminded me of and he told me using BurpSuite was not going to help in the scenario I had encountered. With this I knew that the WordPress site had to be cracked using WPScan. Finding out how to do that was another challenge in and of itself. 

Furthermore, to complicate things, my internet has been dropping out every now and then at random intervals. I don't know what the source of the problem is, I am running windows and the symptoms are so commonplace that the source could be literally anything. I definitely plan to fully convert my laptop to Manjaro once this course is finished. The biggest problem with this is that I'd be performing a particular exploit on the box and then the machine would cut out. My internet is already slow as it is given it is ADSL 2+ (I get NBN set up in 3 weeks thank god) so it takes some time for me to realize that the page doesn't work. 

![Sprint%20Post/Capture.png](Sprint%20Post/Capture.png)

But after it doesn't work the openvpn script shuts down and so does the server. The only way to resolve it is by running windows diagnostic which eventually solves the problem but takes like 5 - 10 minutes. Then I have to run the script again and launch the server. 

![Sprint%20Post/Capture%201.png](Sprint%20Post/Capture%201.png)

Let me be perfectly clear that this is not me whining or complaining, there are others in my class who probably have it worse than me due to the recent flooding. I am simply making the case that this problem hindered my ability to get through different exploits and learn which of them were dead ends.

By the afternoon I was going through WPScan like nothing else. I spent literal hours searching through resources and trying to utilise the dictionary I had. I read through the man page extensively. I searched the internet far and wide, trying every single solution I came across to no avail. The same applied to YouTube, video after video trying to brute force my way through the WordPress login. I don't know how the others are doing in terms of cracking this, but I really want to root this box, no matter how much it does my head in. As you can see from my search history, wpscan did prove challenging.

![Sprint%20Post/Untitled%2010.png](Sprint%20Post/Untitled%2010.png)

One of my biggest problems today was documentation, more so in terms of the write-up than the reflection. I went through so many failed methods that I didn't document all of them as I was doing them. I'll have to go through my google history later and find all the methods I used, but there are just so many. I was really manic, literally just clicking on link after link. Now I understand what Jason and Larry meant when they said:

> "*This deliverable is meant to push you to the point where you are ripping out your hair"*

This was certainly a big task, regrettably my plans at the beginning of the week to work on things like Natas, bandit, or the Vulnerversity box were unsuccessful. Even with my schedule, unlike the previous assignments I couldn't break this down into smaller tasks because I don't know how long I will need to finish it. Therefore, I was fine with putting things like my Linux+ study, Natas on hold because I am still learning with this deliverable and it is also great practice for the next 2 weeks.

Saturday

---

By now I had already figured out how to use WPScan to get into the admin page of the WordPress site. I had also learnt of different methods to use the access I had to reverse shell into the machine. There were 2 primary ways I could do this, reverse shell php into a word theme, use Metasploit. I tried using Metasploit at first, but I got an error. Upon consultation with Max, I was told that I could use Metasploit but it would be better to use the other method as Metasploit does all the work and I don't learn anything. I chose the php injection method because I actually did want to learn. I also planned to do this box again using different methods like Metasploit after this deliverable so to gain more experience and reinforce my skills.

![Sprint%20Post/Untitled%2011.png](Sprint%20Post/Untitled%2011.png)

Another mistake I made today which is a silly mistake that I need to watch out for in the future is my use of IP address. In the code for the Wordpress theme reverse shell php, I had used the wrong IP address for the shell to connect to. This took up hours, but eventually, thanks to Max's insight once again I was able to get past it. David nearly made the same mistake as I did. Once I was in I used:

    whoami
    
    and then
    
    sudo -v

I had been playing around with the reverse shell and after a while with consultation from Max I was able to stumble onto a site. The site helped me find the method which allowed me to Finally get Root.

![Sprint%20Post/Untitled%2012.png](Sprint%20Post/Untitled%2012.png)

I was so relieved that I was able to finish the box. David also finished around the same time as me albeit a bit sooner. Mihailo was having a bit of trouble and it was clear he was nervous. Nevertheless, even after we had done the box, we helped him as much as we could. It was really late but he was close to the end so if we worked on it he could easily finish it. 

Overall, I am very proud of my efforts for this week. There are things that I need to work on, but I feel like I have learned a lot. I am also more motivated doing a hard box and I look forward to the next challenge.

![Sprint%20Post/Untitled%2013.png](Sprint%20Post/Untitled%2013.png)

Sunday 

---

I spent most of the day doing my write-ups and finishing my sprint/reflection for week 4. I had kept up my reflection for both Monday and Tuesday. On Wednesday, I had little time since I spent so much  of it trying to get burp suite to work as you have already read. Then after Uni I had work so I couldn't do much work then. From Thursday to Saturday I basically spent minimal time on the sprint and even the writeup because I just got so deep into rooting my box. I went down so many rabbit holes and made a lot of stupid mistakes. But now, I guess you can say that I'm a lot more clued in on way to approach rooting boxes.

I also spent a lot of the day helping out Mihailo and anyone else who needed help in general. He is really smart but he puts himself down a lot and that stops him achieving which is a shame. Luckily both me and David were able to convince him to keep going. Soon enough even he was able to root the box. 

![Sprint%20Post/Untitled%2014.png](Sprint%20Post/Untitled%2014.png)
### Conclusion
There are definately things for me to improve upon, mostly procrastination during study time. However compared to week 2, I have progressed a lot and I am proud of that. I've had so much fun working with my group for the deilverable. I also cannot state just how much I am learning each day thanks to this summer studio. Furthermore, I'm making sure to balance life by doing things like diving and Kick-boxing so to ensure I don't waste my youth. And lastly I cannot wait for the ninja night from Sectalk and the same goes for Bsides which I hav already bought my ticket for. Until then, peace out! 