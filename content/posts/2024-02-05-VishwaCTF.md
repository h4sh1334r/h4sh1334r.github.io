---
title: "VishwaCTF"
date: 2024-02-05T00:20:50+07:00
draft: false
author: "h4sh1334r"
description: "Solution for Vishwa CTF 2024 challenges" 
tags: ["WriteUp"]
categories: ["blog"]
---

<!--more-->
## Overview

- I've been waiting a long time to participate in a CTF tournament since IrisCTF in January. The days passed without CTF slowly like "waiting for the fish to take the bait" haha. Anyway, it's time for me to look back at myself. In this tournament, I only did 2 challenges, the rest were thanks to the reveal at the end of the tournament. Besides, I participated in 1 more Osint challenge of the BearCat tournament. Thank you for reading.
## Solution

### 1. Announcement (Osint)
- Challenge : 

- I searched for "CyberCell VIIT announces VishwaCTF 2024 Mini" and in an [Instagram post](https://www.instagram.com/reel/C2txmkqLVJn/), i got the flag . 

    -> flag : *VishwaCTF{m1n1_i5_h3r3_l3t_th3_c0untd0wn_b3g1n}*

### 2.Area96 (Stegano)
- Challenge : 

- This is the most confusing challenge because the organizers initially gave 3 files including 1 wav file and 2 zip files. I was about to give up, but after the organizers changed the topic, I didn't understand what the remaining 3 files were for, because the flag was only in 1 file. I used `stegseek` to extract hidden files in the image and got the flag right away. It's hard to understand!

    -> flag : *VishwaCTF{BeepBoop_Jaadu}*

### 3.Murder Mystery (Osint)
- Challenge

- In the received letter we see a part that looks like a barcode. After searching I found out it was *IMb barcode*. You can see the explanation below : 

- After decoding, I couldn't think about anything else. After the tournament ended, I learned that I needed to combine all the numbers given by the barcode and convert them to ASCII. The string I get after merging: `101 118 105 108 95 115 104 97 100 111 119` . And after conversion we get the flag:

    -> flag : *VishwaCTF{evil_shadow}*