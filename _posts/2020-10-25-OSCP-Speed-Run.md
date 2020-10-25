---
layout: single
title: "OSCP Speed Run"
date: 2020-10-25
classes: wide
header:
  Zero to Hero in 3 months
  teaser: /assets/images/OSCP/oscp.png
tags:
  - OSCP
  - PWK
  - Offensive Security
  - Penetration Testing
---
Another cliché OSCP review? Yes.

On August 3rd 2020, I gave a shot at the OSCP exam. I Pwned 4 out of the 5 machines(I wasn't able to get the initial foothold of the 25 point hard one) and officially got the result as ceritified in 4 days after the exam. I've been eyeing for getting OSCP certified ever since I got my job into infosec but since I possess a unique quality named "Procrastination" I kept postpoining the actual preparation for it to the later stage.

Now this is not a blog where I boast about obtaining the OSCP in my first attempt, but rather I aim to guide others who is already preparing or planning to take the exam. If I could obtain the ceritifcation in a matter of 3 months, anyone can, maybe in a lesser period. I'll try to keep this blog as short and precise as possible.

## Training Plan
During the quarantine period I dedicated my time for the actual preparation of the course. Initialy I alloted time to get a clear picture of the exam, how difficult could possibily be the boxes, and read lot's of blogs relating to the course. After a while I found the holy bible for OSCP(atleast to me) TJnulls OSCP prep guide: https://www.netsecfocus.com/oscp/2019/03/29/The_Journey_to_Try_Harder-_TJNulls_Preparation_Guide_for_PWK_OSCP.html. This contains everything you require to pass the exam, explained in the most accurate manner.

My takeaways:
+ Basic understanding of Linux
+ Knowledge of the Linux Terminal, Windows CMD
+ Solid understanding of Networking, TCP/IP, Web
+ Understanding of infosec concepts
+ A familiarity with scripting languages, one should be able to make out what the script is intended for

My preparation started by the middle of April 2020 till the first week of June. During that period I practiced on the retired boxes in HackTheBox platform following the list which was curated by TJnull.
![TJnull Boxes](/assets/images/OSCP/tjnull.png)

I'd suggest to start off by rooting the easy machines first and then later move to the medium and hard ones. Initially when I started solving the machines I was only reliant on the walkthroughs as I wasn't able to root them on my own methodologies.
Good authors of walkthroughs:
Ippsec: https://www.youtube.com/channel/UCa6eh7gCkpPo5XXUDfygQQA
Rana Khalil: https://rana-khalil.gitbook.io/hack-the-box-oscp-preparation/
0xdf: https://0xdf.gitlab.io/

For me this phase was dreadful and frustrating as each machine I solved with the help of walkthroughs, I was losing my confidence at the same time. I went through around 20 machines from the list and decided to take the PWK course head on.

## PWK Labs
Honestly I found the labs to be pretty easy compared to HTB or any of the boxes I rooted, except for the Big 5 - Ghost, Humble, Pain, Sufferance, and 1nsider. If you have done your HackTheBox homework thoroughly you could easily root all machines other than the Big 5. I only went through the machines in the Student network, didn't bother to touch the Active Directory ones nor pivoted to the other Department networks. The reason that I didn't go for the Active Directory machines is that I read in the PWK FAQ's that the exam would remaing the same and there will be a BoF machine which has 25 points, easy machine with 10 points, 2 Medium machines with 20 points each and the hard one which has 25 points, I decided that I'll leave the AD part for the CRTP certification which I plan to take next. All in all I managed to root around 30 machines in the lab.

## PWK Exam
I didn't wanna wait much longer after my labs got ended, so I scheduled the exam as soon as my lab time got over. Scheduled the exam for 3rd August 2020 at 7.30AM IST. I started off with the 25 point BoF machine since I was faily confident on by Buffer Overflow methodology, but here I lost track the count of bad characters in the program which lead to creating a payload which wasn't right for the program. I wasted more than 2 hours just to finally go back and debug the whole program again.
After rooting the BoF box I had 25 points in hand. Next I rooted the 10 point machine, which was very easy - there was no need for Privesc as the initial exploit would give you the root shell. Both the 20 point machines were a good challenge, I struggled to get the privilege escalation on one of the 20 point box, the privilege escalation was right in front of my eyes but took me a while to find it. Almost 19 hours had gone by when I rooted the 4 machines and obtained enough points to pass the exam. I took a shot at the final 25 point machine but that was way out of my league as I struggled to find out the exploit to get the initial shell in the box. With a few hours remaining I gave the white flag and ended the exam.

Reporting was the next step once the 24 hour exam got over. I took screenshot at each and every progress I made in the exam, so didn't have much difficulty in putting together the necessary proof and screenshots in the repot template. Regarding the template I found https://github.com/whoisflynn/OSCP-Exam-Report-Template to be the best among custom OSCP templates. This gets the job done as everything is set up in order, you just have to paste in the screenshots, explanations and the proofs.

## Thoughts
+ Make notes of all the machines you have rooted in your preparation so far. This will become handy as there is a possibility that you might encounter that tecnology in your exam.
+ Do your enumeration on all the open ports thoroughly. Let's say the default SSH port running on port 22 might not be running SSH server ;)
+ Manage your time properly - if you're stuck with a box for a very long period of time I'd suggest you to pause that one, take a short break and move to the next machine
+ The most important thing you have to keep in mind is not to burn out during the exam. Take regular breaks, keep snacks and drinks aside while taking the exam. Drink lots of water.
+ Don't lose your hope if you don't make it at the first attempt. I believe that OSCP is all about the journey and not the destination. The second journey and effort you make would be better in terms of the knowledge you'd acquire than that person who passed the exam in the first attempt.

## Resources

+ [OSCP HTB Walkthrough Playlist by @TJNull and @Ippsec](https://www.youtube.com/playlist?list=PLidcsTyj9JXK-fnabFLVEvHinQ14Jy5tf)
+ [g0tmi1k Linux Privesc Guide](https://blog.g0tmi1k.com/2011/08/basic-linux-privilege-escalation/)
+ [Fuzzy Windows Privesc Guide](http://www.fuzzysecurity.com/tutorials/16.html)
+ [Unix Binaries for Security Bypass](https://gtfobins.github.io/#)
+ [Windows Binaries for Security Bypass](https://lolbas-project.github.io/#)
+ [Buffer Overflow](https://github.com/justinsteven/dostackbufferoverflowgood)
+ [Reverse Shell Cheat Sheet](http://pentestmonkey.net/cheat-sheet/shells/reverse-shell-cheat-sheet)
