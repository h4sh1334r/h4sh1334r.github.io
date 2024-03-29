---
title: "IrisCTF 2024 WriteUp"
date: 2024-01-08T07:42:50+07:00
draft: false
author: "h4sh1334r"
description: "Solution for IrisCTF 2024 challenges" 
tags: ["WriteUp"]
categories: ["blog"]
---

Solution for IrisCTF 2024 challenges.

<!--more-->

# Overview

- For my first CTF tournament of the year, I mainly considered challenges related to Misc, Osint, Forensics but most of them were difficult for me, so I could only do 2 Osint problems. Too bad for that.
# Solution

## 1. Czech where? (Osint)
- The first challenge gave me a photo like below.
    ![Smile](/IrisCTF2024/Czech-Where/image.png)
- I tried searching with GG images and got 1 [article](http://tabiichigo.livedoor.biz/archives/51921024.html) .Use GG map to searh `Golden Lane` and we got the name of street .

    -> flag : *irisctf{zlata_ulicka_u_daliborky}*

## 2.Personal Breach (Osint)

- The challenge shows us 1 website.
    ![Smile](/IrisCTF2024/Personal-Breach/Iris-Steain.png)
- I initially confused it with the cybersecurity company `iris` lol. But when I read the age section, I adjusted my direction. I searched for `Iris Stein` and found her profile - Her [Instagram](https://www.instagram.com/irisstein_station/) and [Linkedin page](https://www.linkedin.com/in/iris-stein-57894b2a7/). Linkedin page helps me answer question number 3-> `Mountain Peak Hiring Agency`. Next I saw she mentioned her mother in an article. Tried searching her mother's name: `Elaina Stein` on google and I found her [Facebook](https://www.facebook.com/people/Elaina-Stein/61555040318052/).
    ![Smile](/IrisCTF2024/Personal-Breach/Elaina-St.png)
- At the bottom of the profile page we will see a pinned event and Elaina was born in 1996 -> she is `27` years old (answer to part 1). 
    ![Smile](/IrisCTF2024/Personal-Breach/Birthday.png)
- Attached is the hospital her mother mentioned. I used google images again and saw the name of the hospital -> `Lenox Hill Hospital`.
    ![Smile](/IrisCTF2024/Personal-Breach/Lenox-Hill.png)
- Enter all the information and get the flag.

    -> flag: *irisctf{s0c1al_m3d1a_1s_an_1nf3cti0n}*

## 3.Away on Vacation (Osint)
-    ![Smile](/IrisCTF2024/Away-on-Vacation/AwayonVac.png)
- We received a transcript for the mp3 file: Transcript: `Hello, you’ve reached Iris Stein, head of the HR department! I’m currently away on vacation, please contact my assistant Michel. You can reach out to him at michelangelocorning0490@gmail.com. Have a good day and take care`
- I did challenge number 3 first, so it seems like I got this associate's profile right away when he followed Iris on Insta. Looking closely at each photo he posted, we immediately get the flag. 
    ![Smile](/IrisCTF2024/Away-on-Vacation/Follow-Ins.png)
    ![Smile](/IrisCTF2024/Away-on-Vacation/flag.png)
- Looking up his gmail with `Epieos` also gives some results but doesn't seem to help with the flag.
   
    -> flag : *irisctf{pub1ic_4cc0unt5_4r3_51tt1ng_duck5}*