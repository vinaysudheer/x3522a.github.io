```markdown
---
layout: single
title: "CRTP bites the dust. CRTP Bootcamp Review"
date: 2021-03-13
classes: wide
header:
  teaser: /assets/images/CRTP/CRTP.png
tags:
  - CRTP
  - Pentester Academy
  - Windows Active Directory
  - Red Teaming
---

It was back in August 2020 that I achieved the OSCP certification. Ever since I cleared the OSCP I was looking for the next certification to take next, sadly, it took me 6 months to finally make up my mind and to enroll for the CRTP certification. I chose to go for CRTP purely due to the fact that its and introductory level Active Directory certifcation, and in this course the instructor Nikhil Mittal takes the beginners approach in the 4 live sessions that we have with him. Nikhil is also the author of [Nishang](https://github.com/samratashok/nishang), a popular collection of scripts which is used in Penetration Testing and Red Teaming.

## CRTP Bootcamps

To anyone who's planning to take the CRTP certification I'd say go for the [Pentester Academy Bootcamps](https://bootcamps.pentesteracademy.com/course/active-directory-6) rather than taking the course listed [here](https://www.pentesteracademy.com/activedirectorylab). I'm suggesting this because at the time of writing this blog the certification is available at a great discount for $299, for this you get 4 weeks of lab access, 4 live sessions(1 live session per week) with the instructor Nikhil Mittal and an attempt to take the examination as well. The quality of live sessions are amazing, since it's a live session you can ask any query's or clarifications to the instructor directly.

Topics covered in the course:
+ Active Directory Enumeration
+ Kerberoasting
+ Abusing ACLs/ACEs
+ Impersonating Privileges
+ Abusing MSSQL Server Links
+ AV Bypass
+ Bypassing Applocker, AMSI, Powershell CLM Mode etc.
+ Cross Domain and Forest Trust Abuse

## The Labs

One thing I noticed about the labs is that the labs go along with the course modules. You gotta wait for the next session with the instructor to get to the next phase in the labs. To me it wasn't a bad thing, I dedicated each week to practice the attacks and methodologies taught in each sessions. The lab automatically resets everyday, so I had to make sure I copied the scripts/commands which I ran to gain access. The most important thing in the lab is to take notes. This course has lots of attacks to go through, since this course doesn't use the automated or c2 frameworks and only relies on the manual approach it's really important to save the commands and scripts that we ran in the lab as notes for future reference. This helped me a lot for the exam. By the end of all the sessions you would possess the skillset to gain admin privileges in the entire active directory forest.

## CRTP Exam

CRTP Exam runs for 24hours. In order to pass the exam successfully you need to compromise 5 machines in the active directory environment and get OS level command execution, the access to the machines should't compulsorly be administrative privs, any user prives will do fine. Once the 24 hours exam time has elapsed, you're given 48 hours to prep the report. Report doesn't have any templates available so basically you can take any template or create your own for the report. In the report you need all the screenshots for the attacks and paths you took in the exam in a neatly presented format. It is also to be noted that even if you have successfully gained access to all the machines required to pass the exam, but the report you submitted turns out to be one which the reviewers have a hard time understanding your methodology or with incomplete screenshots then there's a big chance that you will fail the exam. In the exam instructions pentester academy has clearly stated that the report should be such that a technical/non-technical person should be able to recreate the attacks you have mentioned in the report, all the things must be clearly mentioned with screenshots in the report.

The very next day my lab access ended I took the exam. The exam is an assumed breach scenario where you get access to a machine from there you have to move laterally and vertically to compromise the remaining computers in the domain to get the requirements to pass the exam. You will be given a separate VPN access to the exam environment different from the lab environment.  Enumeration is the key in the exam. Make sure you get BloodHound and the enumeration scripts ready for thorough enumeration. Take notes on each approach in the exam, I personally would suggest to make CherryTree the primary tool to take notes. Only the attacks and methodology you have learned in the course and labs so far will be there for the exam, this means you're not required to perform any attacks outside the course syllabus to pass the exam. You're free to use any tools or frameworks if you are familiar with any. There is no restriction for the tools to be used in the exam.

## Takeaways
+ Take notes for everything you encounter in the course. Let it be anything you understand or not understand at the first take, just make a note of it.
+ I say this again, enumeration is the key. Don't just jump into the attack phase if you figure out any possible attack path at the first glane. Take your time to enumerate thoroughly and then go for the next phase.
+ Don't skim through the course and lab. Take your time to do the lab exercises as well. Lab exercises will come in handy to get you preped for the exam.
+ Similar to the takeaway I mentioned in my OSCP Review writeup, an important thing you have to keep in mind is not to burn out during the exam. Take regular breaks, keep snacks and drinks aside while taking the exam. Drink lots of water.

## Resources

+ [ADSecurity.org](https://adsecurity.org/)
+ [harmj0y blog](https://www.harmj0y.net/blog/)
+ [PowerView Cheatsheet](https://github.com/HarmJ0y/CheatSheets/blob/master/PowerView.pdf)
+ [ired.team](https://www.ired.team/)
+ [The Dog Whisperers Handbook](https://insinuator.net/2018/11/the-dog-whisperers-handbook/)
+ [Nikhil's Personal Blog](http://www.labofapenetrationtester.com/)
```