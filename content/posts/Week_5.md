+++
title = "Final Portfolio Submission"
date = "2020-03-02"
author = "Donny"
cover = "/Week5_deloitte_ctf2.PNG"
description = "A reflection of the progress made in week 5"
+++

# Wk 5 summer studio Reflection

---

# Introduction

This week, like the last week, the goal was to work on a box. The box this time was on TryHackMe, it was also stressed that these boxes were a lot harder. There were 3 boxes to choose from, OpenAdmin, Traverxec, and Postman, each increasing in difficulty. I chose to go with Travserxec mainly because everyone else was doing OpenAdmin and moreso because I like a challenge. Since the boxes were pretty difficult, the requirement for this week was to try to get the user.txt file for a user, while obtaining root user was the goal for next week. 

# Goals

- Get user.txt and possibly root by this week.
- Maintain progress on reflection and write up by not leaving it to the end.

# Implementation

- Allocate time for the box and utilise tutors only when really stuck.
- Ensure write up is completed as I do the work rather than at the end.

# Monday

We were told from the onset that both this week and the next will push us to our limits. Although nerve-wracking, I am not too worried about it, even a bit excited. The University subjects I have had until now, and there are some exceptions to this, never really pushed us to learn. The only times we were pushed was when the subject was run badly and we had to compensate by teaching ourselves. In addition, week 4 was a great catalyst to get us in the mindset for the next 2 weeks. We now are armed with experience, we have had practical experience with the pen-tester methodology, we know how to research better, and we at least have a solid idea of what is expected. We are definitely more confident.

{{<image src="/Week5_pen_LifeCyc.PNG" alt="" position="center" style="border-radius: 8px;" >}}


It was also mentioned that we were getting a visit from Deloitte Services Pty Ltd on Thursday this week. I had never actually heard of this company before, I will definitely allocate a small portion of time this week learning about different companies involved in the cyber security industry since it will be useful to know. The day would consist of a workshop/seminar where the company members would basically tell us more about themselves. To make things interesting, at the end of the seminar, there will be a CTF where all the class members will participate in a race to win. 

{{<image src="/Week5_thursday_prep.PNG" alt="" position="center" style="border-radius: 8px;" >}}

One of the things I will try this week is to create a document where for each heading of the pen-tester methodology, I will have various tools, their uses, and example of use. The theory being, rather than trying to remember a lot of information in a time-constrained environment, I can simply utilise a document with everything I need. It also saves time because I won't have to google as much. The tutors stressed that punctuality was a must for this Thursday, it made sense seeing as you would want to create a good first impression and also because it would make the day run smoother. My plan is to rock up a bit early, maybe around 9 and do some work on my box so to get my mind warmed up for the challenge.

Speaking of Boxes, the theme for this week is harder boxes. The task is to complete a box on [HackTheBox.eu](http://hackthebox.eu) by achieving root access and obtaining the user.txt file, for proof, we have to show user.txt either through screenshot or password protected pdf. I'll go with the password option because I spend a lot of time with Notion and I can easily just export it out along with the write-up. To make things easier, I finally got myself an ssd from the university. As soon as I got the device, I uploaded my vm disk onto it and noticed a considerable difference in performance. I had to delete a few files before I could transfer the vm disk because I had no space to even copy the file. 

{{<image src="/Week5_ssd.jpg" alt="" position="center" style="border-radius: 8px;" >}}

One of the cool things about Hack the box is that you actually a have to hack the login page to get an invite to log in. I think that is really cool personally. Hacking into the login was fun, especially because I made some silly mistakes. I cannot publicly post about the login but it was a fun web-testing exercise and I also learnt from it. One thing I am sad about is that you don't have to hack into the store to get merch. It is convenient but I prefer to earn it because it feels better. I spent most of the class time getting into the website, at home I had little time so I spent it on the reflection and started my write up. 

# Tuesday

Today was a really productive day for me. In terms of the deliverable, I spent a lot of today going through it and making good progress. I was quick to spot something that allowed me to get semi-shell access. After a quick google search and some thinking I made my way into the shell. I used metasploit only due to time restraints since I know from talking to Max that there is a long way to go even after basic shell access. I basically wanted to spend the majority of the time with gaining root priviledges which again thanks to Max is going to test me just like the Mr Robot box. If I do manage to complete the box early I will then try it again not using metasploit as an additional challenge. And If I somehow manage that which is really unlikely, but if I do, I will try my hand at the Postman box. The more I can challenge myself the better.

{{<image src="/Week5_teamsConvo.PNG" alt="" position="center" style="border-radius: 8px;" >}}

One of the things that has also changed this week is that I compile my write up for my box as I am doing it rather than towards the end which is what I did last week. The reason for this are as follows

- I ended up rushing towards the end of last week for my write up, in doing so the quality of my report wasn't as good as I had liked.
- I might have failed attempts that I would not remember If I just compile it at the end.
- It also helps me mentally, so that at the end of the day I can look at my work and properly measure my productivity.

The difficulty however wasn't getting into the shell but rather obtaining user shell access. Basic SUID tactics didn't work. I had to read a lot of man pages for different programs and there were so many rabbit holes I went down with no results. The only result was that I learnt different methods that did not work for this box but just might work for other boxes. I also helped Phillip a bit since he was struggling to get Metasploit working and he basically already knew what to do. 

{{<image src="/Week5_phillip_convo.PNG" alt="" position="center" style="border-radius: 8px;" >}}

As I am writing this reflection, I realise that producing content for said reflection is difficult to find because of the restriction of HackTheBox. So, I can't post any artefacts that directly show my work. I will also add that the use of notion has greatly increased my productivity. Unlike with OneNote, it is easy to log my work due to the keyboard driven events. Furthermore, unlike OneNote, which I had been using predominantly until last week, placing in artefacts is so easy which allows me to not lose time to logging when I do my work. It also has a built in organiser which is really useful when i transferred my notes from OneNote to Notion this week.

{{<image src="/Week5_notion.PNG" alt="" position="center" style="border-radius: 8px;" >}}

# Wednesday

I learnt quite a bit today and I would say I've made a fair amount of progress since yesterday. However there were also many barriers I faced today too. I came into University this morning to work more on my box since the tutors were available. One of the barriers I faced was using metasploit. Although easy to use, it was fairly unstable, when I would use the exploit I would be given a meterpreter with a shell but no terminal. This was a problem since the meterpreter had limited functionality thus forcing me to import a terminal with the following script:

```bash
python -c "import pty; pty.spawn('/bin/sh')"
```

I had worked the previous night and was basically exhausted. Luckily there are many coffee shops around UTS. I am not much of a coffee drinker but I do have it when I need to work. Larry suggested a cold brew called Nitro. I had never heard of cold brew before, let alone Nitro, but anything to get me productive was necessary at that point. In definitely made me more productive, I got my head down and enumerated a lot and found out many things about hidden files. 

Luckily for me Jason hated the instability of Metasploit too and helped me with using the python program on exploit-db. The python program was so much easier and stable to use and only required 1 command saving valuable time. Using the following link given previously given by the tutors:

https://highon.coffee/blog/reverse-shell-cheat-sheet/

I was easily able to locate and execute a reverse shell into the system. The site is easy to read and has a reverse shell for almost everything. Also, Tyrone may or may not have almost spilt coffee on my computer. One of the things that slowed everyone down today was the resetting of servers and slow internet speed. I was less affected than everyone else since I was doing the Traverxec box but even my server got reset at times. Funnily enough, one of those resets was by Phillip which he did by accident. The set back were annoying because we didn't have time and the reset happened whenever we were trying things out. So, we'd Enumerate, then try our solution, the server would get reset and then we'd have to wait and try again.

{{<image src="/Week5_Enumeration.PNG" alt="" position="center" style="border-radius: 8px;" >}}

In summary, I had progressed in a more lateral movement rather than straight forward. What I mean by that is, I had not succeeded in getting a user shell, but I learnt not to rely on Metasploit and further to use scripts to get access to the shell. Also, I handed Larry my resume that had been approved by Max. He said it was a lot better than my initial approach which was really good to hear. I will eagerly wait for his feedback and once I get the all clear I will apply for the position.

{{<image src="/Week5_resume.PNG" alt="" position="center" style="border-radius: 8px;" >}}

# Thursday

Today was a really cool day. Two speakers from Deloitte Australia; Peter Westein and Nathan Jones came in to tell us about their work and how they go about their days. They spoke about the practice of cybersecurity and the processes they carry out in their day to day operations. The topics included Red Teaming, Blue Teaming, Cyber intelligence and much more. As someone who desires a career in the same industry as them, it was incredibly insightful to have such an informal presentation from them.

{{<image src="/Week5_Deloitte.PNG" alt="" position="center" style="border-radius: 8px;" >}}

I made sure to take notes down as best I could. One of the things that really struck me was the mindset. The speakers informed us that with red team operations, the point is to think like a criminal and that it is like a real game of strategy. 

{{<image src="/Week5_strategy.PNG" alt="" position="center" style="border-radius: 8px;" >}}

This was actually one of the things that drew me to cybersecurity, the warfare, not just restricted to the attacking of programs/systems but things like physical attacks, e.g. using a Wi-Fi pineapple to steal credentials or using Pinterest for intel on the layout of a building. Even things like dressing up in high-visibility clothing to look like a maintenance worker. After the talk finished, we all participated in a ctf that the speakers introduced. I was a bit slow to get into it due to the myriad of problems with the VMware on my laptop, although thanks to Max and the speakers, I was able to rectify the problem. No one managed to achieve root that I know of. Me and David worked together and managed to get pretty far in that we both retrieved the deleted git hub files.

{{<image src="/Week5_deloitte_ctf2.PNG" alt="" position="center" style="border-radius: 8px;" >}}

I also signed up for the Ninja night next Tuesday night hosted by Sectalks. This will be our first official extra-curricular  CTF. I am so excited because Max and a handful of people from the class will be also be going. Hopefully, we do well in the ctf and I get to meet some more interesting people. I'll make sure to blog it for next week and If I get a good photo, I'll put it up on my LinkedIn and twitter as well. I might even see a few of the people from the previous Sectalks night a few weeks back.

# Friday

At this point I had shell access and some valuable information in how to get user shell access. There was a drop in but I didn't go because the VMware on my laptop was annoying and I am way more productive on my desktop at home. 

The server got reset once again forcing me out of my shell for a good 10 minutes and forcing me to  connect to the VPN once again. I made sure to keep the Shoutbox tab open on my second monitor to cancel any future reset attempts.

{{<image src="/Week5_HTB_reset.PNG" alt="" position="center" style="border-radius: 8px;" >}}

I had made a lot of progress in terms of the file I found, I had even extracted important information from it. I didn't really understand the extraction tool I was using, so I consulted the man page.

{{<image src="/Week5_Man_page.PNG" alt="" position="center" style="border-radius: 8px;" >}}

Upon doing so I had the information I needed to pretty much get authorized access to the user shell. The information wasn't in a form that would allow to access the user shell directly so I had to do some work on it and figure out also how to use said information to gain access. Due to my inexperience with the tools and the lack of a man page or documentation for one of the required tools. What should have been a quick and decisive attack, turned into hours of hell. I spent so much time researching the tool which will be in my Write-up once the box is retired, and I ended up getting no where. In the end I had to stop and go to work. Even with help from Philip I still could not get it to work, nevertheless I was determined to figure out the problem the next day.

On a more positive note, Several of the students in my class, myself included, banded together and found a place to stay in for Bsides in Canberra. It was a good place, three double beds for 6 people, for around $123 each. Furthermore, it was only a 10 minutes walk from the venue for Bsides. This was a really great turnout because I got my ticket straight away and it would be good to go with some people I already know. Its also beneficial in terms of cost-effectiveness. We also organised transportation via grey 

put grey line picture here

# Saturday

The goal for today was to obtain user.txt. I don't think I'll be able to achieve root by this week since I have work both today night and tomorrow night. Getting root is not necessary for this week but I would have liked to get it so that I could get an early start on Postman. My efforts today were greatly slowed down due to a very crucial mistake. I did manage to figure out the mistake but I had lost about 4 hours to it which is a big setback. Luckily, according to Jason, I am very close to user.txt. 

The setback was as such. On Friday, I had found a certain folder. As Jason had hinted on Monday this is due to the file structure of linux. Once again due to the restrictions of Hack The Box I cannot show the artifacts necessary to illustrate my point. The Write-up will be available however, only after the box is retired as per the rules of the site. The basic problem is as follows. I was trying to get user shell access, I knew how to do it but there was a tool that I needed to. 

{{<image src="/Week5_tool.PNG" alt="" position="center" style="border-radius: 8px;" >}}

I had tried using this tool but always got an error. I usually restrict myself to not asking for help until I have exhausted all options which is what I did today. I had looked far and wide on the internet, but in the end, regardless of which solution I tried, the tool always gave me the same error. When I used other tools, I also got errors. Because of this setback I did not go to the gym, I really wanted to get the user shell.

 In hindsight I realise this was a mistake because I had dragged down another commitment with me. It would have been better to go to the gym and get my mind of the box. Finally when I exhausted all available means I contacted Jason. At that moment I figured out it was the way I was input the data into the tool that caused the error as shown above. This mistake took a lot of time due to the enumeration process I undertook to overcome it. Once I figured it out and input the data in correctly, I had all I needed to own user.txt.

{{<image src="/Week5_usertxt_.PNG" alt="" position="center" style="border-radius: 8px;" >}}

After I got this I was relieved because I could got to work and not worry about getting user.txt. All I had to do was touch up my reflection and I was finished for this week. On a side note, I also bought a hack the box T-shirt, I really like cyber security merch e.g. stickers and patches. I'll also get the sticker to put on my laptop, but that's for later.

# Sunday

I had managed to get the user shell and thus access to user.txt yesterday so I just focused on polishing my reflection for most of today. It was hard since I .On Sundays, I have tried to use the day to try to plan out the rest of my week. I do this by making a schedule which takes some time to actually do properly. I use Google calendar which is a basic scheduler. In my opinion, it works pretty well, especially since I have to balance work, University, and other extra curricular activates. 

{{<image src="/Week5_calender.PNG" alt="" position="center" style="border-radius: 8px;" >}}

Furthermore, since O'day was coming up, I was thinking of joining the UTS Oztag team. I really liked Oztag in school although I never played comp which was a shame. For the longest time I've been wanting to play a team sport, I had looked at it last year but I missed sign up so I didn't get in. I only have two years of University left and I don't really want to leave without playing at least one team sport. Luckily for me, I had a mate that I met during the tragedy that was Routing and Switching essentials. He was joining too and was already training, after talking a bit we just basically decided to go for it since O'day was close and we would both be there.

{{<image src="/Week5_lastpost.PNG" alt="" position="center" style="border-radius: 8px;" >}}

# Conclusion

This week went really well in my opinion although things got a little hard towards the end. Other than the problems with the box itself like resets, my ability to progress was slowed down due to my mistakes. Although I accept my mistakes and will learn from them, I need to ensure that I don't sacrifice other things like going to the gym just because I won't be able to get root early. I realised that if I do things like that, I not only don't do well with finishing my box, but I also ensure that I am not dragging down my other commitments.