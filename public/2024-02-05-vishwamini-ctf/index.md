# VishwaMini CTF 2024


Solution for VishwaMini CTF 2024 challenges.

<!--more-->
## Overview

- I've been waiting a long time to participate in a CTF tournament since IrisCTF in January. The days passed without CTF slowly like "waiting for the fish to take the bait" haha. Anyway, it's time for me to look back at myself. In this tournament, I only did 2 challenges, the rest were thanks to the reveal at the end of the tournament. Thank you for reading.
## Solution

### 1. Announcement (Osint)
- Challenge : 
![Smile](/VishwaCTF/Announcement/Announcement.png)

- I searched for "CyberCell VIIT announces VishwaCTF 2024 Mini" and in an [Instagram post](https://www.instagram.com/reel/C2txmkqLVJn/), i got the flag . 
![Smile](/VishwaCTF/Announcement/flag1.png)
    -> flag : *VishwaCTF{m1n1_i5_h3r3_l3t_th3_c0untd0wn_b3g1n}*

### 2.Area96 (Stegano)
- Challenge : 
![Smile](/VishwaCTF/Area96/Area96.png)
- This is the most confusing challenge because the organizers initially gave 3 files including 1 wav file and 2 zip files. I was about to give up, but after the organizers changed the topic, I didn't understand what the remaining 3 files were for, because the flag was only in 1 file. I used `stegseek` to extract hidden files in the image and got the flag right away. It's hard to understand!

    -> flag : *VishwaCTF{BeepBoop_Jaadu}*

<br> *Note: File of this challenge in /static/VishwaCTF/Area96 dir. Thanks*
### 3.Murder Mystery (Osint)
- Challenge
![Smile](/VishwaCTF/MurderMistery/Murder-Mistery.png)
- In the received letter we see a part that looks like a barcode. After searching I found out it was *IMb barcode*. You can see the explanation below : 
![Smile](/VishwaCTF/MurderMistery/IMb-Barcode.png)
- I did it by hand and got the following chain: `ATTTFTADAFFTDTTAADTDTTATDAFDDDATATDDDDTADFAFADFATATFDFADDFFAFATDT `. 
<br>After decoding by this web,I have this but I couldn't think about anything else. 
![Smile](/VishwaCTF/MurderMistery/IMb-decode.png)
- After the tournament ended, I known that I needed to combine all the numbers given by the barcode and convert them to ASCII. The string I get after merging: `101 118 105 108 95 115 104 97 100 111 119` . And after conversion we get the flag:

    -> flag : *VishwaCTF{evil_shadow}*

### 4. I'm a Peaky Blinder (Osint)
- Challenge : 
![Smile](/VishwaCTF/PeakyBlinder/Peaky-Blinder.png)
- I tried copying the entire introduction and realized it was part of a song from the recent famous movie 'Peaky Blinder'. The film's popularity cannot be disputed.
Back to the challenge, the last part of the introduction is an Insta account. For each photo we will receive a portion of a [Facebook account](https://www.facebook.com/profile.php?id=61554610571803&mibextid=hIlR13). Which takes us to that page, at the bottom of the page is another Insta account. 
![Smile](/VishwaCTF/PeakyBlinder/PB-Insta.png)
- In the new insta page just received,look carefully at each photo and see that there is a question there. The flag we receive is the answer to the question.
![Smile](/VishwaCTF/PeakyBlinder/flag4.png)
    -> flag: *VishwaCTF{The_Garrison}*

