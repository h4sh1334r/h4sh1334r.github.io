---
title: "EyesOpen CTF WriteUp"
date: 2023-11-19T02:16:50+07:00
draft: false
author: "Bear4Ts1ck"
description: "Some write-up for EyesOpen CTF tournement" 
tags: ["WriteUp"]
categories: ["blog"]
---

Some write-up for EyesOpen CTF tournement.

<!--more-->

# Overview

This EyesOpen ended quite a while ago but I was able to post for it today. Actually, it is not difficult for newcomers, nor is it easy. You need better eyes lol.

# Solution

# Stegano
<br>*Note: Look like all link not working until tournament end. Thanks

#### 1.flag67

- Spectrum analyze : [Spectrum Analyzer](https://academo.org/demos/spectrum-analyzer/)
- [Link challenge](http://52.2.19.143:8080/challenges#flag67-59)
- At the beginning we saw that it is a wav file. I immediately thought of 'audacity' and 'spectrogram'.

- Open Audacity and change to spectro view, we get the flag. If we don't see it clearly we can use the link above: 
  
  => *flag{edmplscr}*



#### 2.flag66 

- [Link challenge](http://52.2.19.143:8080/challenges#flag66-58/)

- I was quite struggling with this challenge. I opened this jpg file and saw:

- Well,it reminds me of stegsolve, but I tried all stegsolve tools to no avail. After asking and receiving a hint about using "stegseek", i downloaded and used stegseek with 'wordlist.txt' but it seems the sample space is a bit small so it doesn't return results for me. I tried it with 'rockyou.txt' and got the result : 

    => *flag{pml5j21}*