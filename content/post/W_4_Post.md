+++
title = "Week 4 Reflection"
date = "2020-02-16"
author = "Donny"
cover = ""
description = "A reflection of the progress made in week 3"
+++

### SLO1 — Introduction 
The theme of this week is boot2root.

 This week we root our first box. Rather than a simple ctf,the challenge involves many techniques with end results. There are many methods to root the box and in this weeks sprint is the Writeup that details my method given by a link to the next post at the bottom of the page.



### Goals
	1) To root my box and document it

### How it will be achieved
* Pure willpower, and some help from the tutors of course.
-

### Monday 

---

Once again, a stand-up meeting to start the week. It's nice to see everyone has come along way from where they began at the start of the subject. My objective for this week is to be more studious and disciplined when it comes to times allocated for study. 

The deliverable for this week is interesting. Rather than a presentation, we have a practical
assessment where we have to choose a box and then break into it. The goal is to
gain the highest level of authority in the box. It's  a big step up the projects we've had and is
definitely a plunge into the deep end. I followed along as best as I could but I know that this deliverable will definitely test me. The notes I took down are a bit hard to read since I write one-liners in the interest of time.

{{<image src="/img/Wk4Arti0.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

It was hard to digest all of the information in Jason's demonstration. Although I understand what happened, it's still a lot of information to process. Even though this deliverable will be incredibly difficult, I am looking forward to it since it will be even better when I overcome it. Google, YouTube and the stack skills will be my most visited sites, I can already tell. It is also great practice for the assignment at the end where we will have to break into another system. 

I still need to learn how to use things like burp suite, vim, and Metasploit. Another interesting point that Larry pointed out is that we should be up to level 15-20  in both bandit and Natas in order to really get a good understanding. I am only up to level 4 in Natas and level 6 in Bandit. I will focus on getting that done as soon as possible. We also tried our hand at the beginner Box, it was the Basic pen testing 1 box on Vulnhub. I wasn't able to do much at University because the demonstration was long and I spent most of my time trying to understand why certain things were done. For the most part I spent the time inspecting the box using nmap as well as looking at the source web app. Luckily for me (and the rest of the class), Yukari had not only recorded, but also uploaded the whole process of Jason rooting the Wakanda box to her YouTube channel.
 

{{<image src="/img/Wk4Arti1.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

When I got home I worked on the machine some more.  I realised with some hints form Anthony in class that the box was running FTP. I simply looked up the exploit on the Metasploit database and filled out the options.

{{<image src="/img/Wk4Arti2.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

Using metasploit didn't work at first but after using a YouTube video I was able to get into the box. It turned out I was inputting a value in the wrong place. After that I used the "whoami" command to observe my privilege level. It was root and so I had cracked the box.  I see now why it was a beginner task but I'm glad I'm happy I cracked it, especially because I had Kick-boxing that night so I didn't have much time to work on it. 

 

### Tuesday

---

I finally finished touching up my resume and sent it to Max. Using Microsoft Word to craft resumes
is a pain in the ass, I might have to re-learn how to use Latex. I also discovered Notion which is one of the most spectacular note-taking programs that I have ever seen. It combines the automatic multi-device sync ability of OneNote with the powerful note-editing abilities of Latex, although to a
lesser extent. It's wonderful for taking notes when coding or just normal notes, I haven't tried it for mathematics. 

{{<image src="/img/Wk4Arti3.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

I talked to Max about my experiences with my basic pen testing 1, he usually gives helpful advice and has a lot of experience that I can glean from. He asked me if I had found the password which I didn't do since I got root and just assumed I was done. After googling I found out that you can break hashes using John the ripper or hash cat, and If I am really lazy I can also use online hash crackers.

{{<image src="/img/Wk4Arti4.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

In fact Max was actually the one who one who challenged me with the Mr Robot box. I loved the show and more importantly he had asked me if I wanted a challenge. I did want a challenge, firstly, because it would would boost my confidence doing it, and secondly, because I would learn a lot in the process. I did start the Box and it was pretty fun. I'll admit, the content was very interesting and I low-key spent more time on it than I should of. I did manage to get the first flag of the box which was good, it was simply in the robots.txt file of the site. I though that was pretty comical since the box is called "Mr. Robot". There were 3 flags (the box called them "keys") in total for me to get. I wasn't able to do much today since I spent quite some time figuring out how to get the box running and more so because I had work. The important thing was that I had started and that I already had the first key.

### Wednesday

---

Today was not as productive as I would have liked it to be. Even though the day is optional, I came in anyway because I knew I would need help with the challenge. I got a bit further in the box by using directory traversal and realizing the website used WordPress. I also knew of a particular tool that would help me bypass the admin login page of WordPress to give me administrative power. From there it should have been easy. The problem was that I used wpscan wrong and then deduced that wpscan was the wrong tool. That was mistake number 1. I then went straight to google to find other ways to hack the site.

{{<image src="/img/Wk4Arti5.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

One of the solutions involved using burpsuite, Max informed me that using burpsuite wasn't necessary, yet I persisted anyways. That was mistake number 2.

{{<image src="/img/Wk4Arti6.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

The reason for that being a mistake was simply because Burp suite didn't work on my kali. And getting to to work yielded no results. I lost so much time trying to get it to work. I deleted and re-imported certificates, I removed and re-added Foxy Proxy, et cetera. After hours of trial an error, and with the help of the tutors, the problem seemed to be my version of Kali. I also met Jai which was cool, had some funny banter with him that kind of lifted the mood. Nevertheless not being able to use Burp suite was driving me up the wall. The internet was slow for some reason so I couldn't use it to re-download the 2020 kali. Even Jai tried to help out using his hotspot but it still was too slow. The only solution was Max who had kindly offered to let me borrow his SSD to download the kali distribution I needed. The first time I used his SSD I did not realize that his version had I3 which made the distro unusable for me. Luckily, for me Max once again helped me out by sitting down with me and showing me that he had another version of kali on his SSD and by the end of the day we got it done.

{{<image src="/img/Wk4Arti7.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

### Thursday

---

Finally got burp suite working after the demo today around lunchtime. I don't know what the problem was exactly, I upgraded my kali with another kali distro that Max kindly gave me yesterday and it solved the problem. Another problem that came up though is space. My laptop has enough space for now to run the VM kali. However, windows is always increasing the amount of data it takes from me so hopefully my laptop holds out until next week when I can utilize the SSD for the course.

On the bright side, I now have notion which is huge help for someone like me who prioritizes organisation and flexibility. Onenote is good only because of its cross-device functionality. The problem is that it is not that good at facilitating note taking and the sync process can be a bit dodgy at times. Notion also has the advantage of text driven modification which really helped with note taking during the demo. For example, Jason was using Enumeration at one point which I had only heard people mention before. Thus, when he was using Enumeration to find shared directories,   I was able to easily take down notes with minimal effort. If there was a command I hadn't seen before, I simply took down the command using "/code" and then proceeded with the command. I didn't even need to use the mousepad. The result was effective notes that was clean and organised (shown below):

{{<image src="/img/Wk4Arti8.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

After lunch, I resumed my efforts on my box. I knew with my commitments to work and other things that I couldn't waste time since this box was challenging or at least reputed to be so. I also convinced Mihailo to do the same box so that he actually challenged himself rather than just complain about not being smart. Here is something else I figured out:

You have to keep the openvpn script running.

I already had the IP address of the website, so I simply would use nmap to investigate for any open and/or vulnerable. When I did so I'd go to the shell where I connected to openvpn, use Ctrl+C and then use Nmap. My hypothesis was that when I Initially connected to the vpn, it would stay open. But whenever I did the Nmap wouldn't get results that I wanted. Thankfully in today's class, Max spotted my mistake and let me know that I had to open another terminal and use Nmap there. Luckily I had that error fixed before work so that the next day I could be more productive.

### Friday 

---

The theme of today is "you win some you lose some". This isn't some cliché either that I am adding to my reflection, I mean this literally. As you will see from the write up for my box, I spent a large amount of time trying to bypass the WordPress login, specifcally 5 hours. The reason for this was that WPScan didn't work for me, well in actuality I didn't use it properly. Because I thought it didn't work I used google, youtube and anything I could find to try and crack the login. As it turns out, there are so many ways to get past a WordPress login. I of course, used as many as I could.

The methods involving Burp suite took the longest simply because I had to learn how to use it and I also had to learn about http messages in general. I went through so many resources, and each time I hit a dead end. The reason I say the theme of today is as such is because although I lost significant time with all these methods, I learnt a lot about the many different ways to exploit wordpress. I also learnt about things like "?author=1" and "xml=rcp" which I had no idea about. Of course after I had exhausted so many methods I was at my wits end. Logically I asked Max for a clue or a hint.

{{<image src="/img/Wk4Arti9.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

I learnt a lot like being able to look through man pages using "/", search for the command and then hitting return. Max is helpful in that he doesn't give me the answer but will tell me if things are just out right wrong. By learning what things are wrong, I may not know what to do, but I know what not to do which helps me focus on finding what I need. I had discovered a dictionary list previously which Max reminded me of and he told me using BurpSuite was not going to help in the scenario I had encountered. With this I knew that the WordPress site had to be cracked using WPScan. Finding out how to do that was another challenge in and of itself. 

Furthermore, to complicate things, my internet has been dropping out every now and then at random intervals. I don't know what the source of the problem is, I am running windows and the symptoms are so commonplace that the source could be literally anything. I definitely plan to fully convert my laptop to Manjaro once this course is finished. The biggest problem with this is that I'd be performing a particular exploit on the box and then the machine would cut out. My internet is already slow as it is given it is ADSL 2+ (I get NBN set up in 3 weeks thank god) so it takes some time for me to realize that the page doesn't work. 

{{<image src="/img/Wk4Arti10.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

But after it doesn't work the openvpn script shuts down and so does the server. The only way to resolve it is by running windows diagnostic which eventually solves the problem but takes like 5 - 10 minutes. Then I have to run the script again and launch the server. 

{{<image src="/img/Wk4Arti11.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

Let me be perfectly clear that this is not me whining or complaining, there are others in my class who probably have it worse than me due to the recent flooding. I am simply making the case that this problem hindered my ability to get through different exploits and learn which of them were dead ends.

By the afternoon I was going through WPScan like nothing else. I spent literal hours searching through resources and trying to utilise the dictionary I had. I read through the man page extensively. I searched the internet far and wide, trying every single solution I came across to no avail. The same applied to YouTube, video after video trying to brute force my way through the WordPress login. I don't know how the others are doing in terms of cracking this, but I really want to root this box, no matter how much it does my head in. As you can see from my search history, wpscan did prove challenging.

{{<image src="/img/Wk4Arti12.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

One of my biggest problems today was documentation, more so in terms of the write-up than the reflection. I went through so many failed methods that I didn't document all of them as I was doing them. I'll have to go through my google history later and find all the methods I used, but there are just so many. I was really manic, literally just clicking on link after link. Now I understand what Jason and Larry meant when they said:

> "*This deliverable is meant to push you to the point where you are ripping out your hair"*

This was certainly a big task, regrettably my plans at the beginning of the week to work on things like Natas, bandit, or the Vulnerversity box were unsuccessful. Even with my schedule, unlike the previous assignments I couldn't break this down into smaller tasks because I don't know how long I will need to finish it. Therefore, I was fine with putting things like my Linux+ study, Natas on hold because I am still learning with this deliverable and it is also great practice for the next 2 weeks.

### Saturday

---

By now I had already figured out how to use WPScan to get into the admin page of the WordPress site. I had also learnt of different methods to use the access I had to reverse shell into the machine. There were 2 primary ways I could do this, reverse shell php into a word theme, use Metasploit. I tried using Metasploit at first, but I got an error. Upon consultation with Max, I was told that I could use Metasploit but it would be better to use the other method as Metasploit does all the work and I don't learn anything. I chose the php injection method because I actually did want to learn. I also planned to do this box again using different methods like Metasploit after this deliverable so to gain more experience and reinforce my skills.

{{<image src="/img/Wk4Arti13.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

Another mistake I made today which is a silly mistake that I need to watch out for in the future is my use of IP address. In the code for the Wordpress theme reverse shell php, I had used the wrong IP address for the shell to connect to. This took up hours, but eventually, thanks to Max's insight once again I was able to get past it. David nearly made the same mistake as I did. Once I was in I used:

    whoami
    
    and then
    
    sudo -v

I had been playing around with the reverse shell and after a while with consultation from Max I was able to stumble onto a site. The site helped me find the method which allowed me to Finally get Root.

{{<image src="/img/Wk4Arti14.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

I was so relieved that I was able to finish the box. David also finished around the same time as me albeit a bit sooner. Mihailo was having a bit of trouble and it was clear he was nervous. Nevertheless, even after we had done the box, we helped him as much as we could. It was really late but he was close to the end so if we worked on it he could easily finish it. 

Overall, I am very proud of my efforts for this week. There are things that I need to work on, but I feel like I have learned a lot. I am also more motivated doing a hard box and I look forward to the next challenge.

{{<image src="/img/Wk4Arti15.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}

### Sunday 

---

I spent most of the day doing my write-ups and finishing my sprint/reflection for week 4. I had kept up my reflection for both Monday and Tuesday. On Wednesday, I had little time since I spent so much  of it trying to get burp suite to work as you have already read. Then after Uni I had work so I couldn't do much work then. From Thursday to Saturday I basically spent minimal time on the sprint and even the writeup because I just got so deep into rooting my box. I went down so many rabbit holes and made a lot of stupid mistakes. But now, I guess you can say that I'm a lot more clued in on way to approach rooting boxes.

I also spent a lot of the day helping out Mihailo and anyone else who needed help in general. He is really smart but he puts himself down a lot and that stops him achieving which is a shame. Luckily both me and David were able to convince him to keep going. Soon enough even he was able to root the box. 

{{<image src="/img/Wk4Arti16.PNG" alt="Hello Friend" position="center" style="border-radius: 8px;" >}}
### Conclusion
