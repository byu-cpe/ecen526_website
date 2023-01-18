---
layout: lab
toc: false
title: Cracking WEP and WPA2
number: 3
---

<div class="alert alert-primary" role="alert">
    <b>Disclaimer</b>: By performing this lab, you agree that you will not use these skills in an unethical manner. I give you permission to gain access to the wireless network I created for this lab, but I do not give you permission to access any other wireless network using the techniques you will learn in this lab.
</div>

## Overview

In this lab you will hack into two wireless networks, one protected by WEP and another protected by WPA2. The lab will teach you how trivial it is to crack WEP and WPA2 with a weak password.

I have set up two wireless networks, "ECEn526-WEP" and "ECEn526-WPA2". Each of these networks has a computer attach to it. Your job is to gain access to the network, SSH into the computer, and retrieve the secret off of the computer. There is two secrets in total, one for each network. You will then upload the secrets to Learning Suite. Since the point of the lab is to learn about WiFi security, I will give you the username and password of the computer attached to the network.

Here are the steps of the lab:

1. Gain access to the network. You are on your own for this one. There are plenty of tutorials online for how to do this for WEP and WPA. Good luck!
   
2. SSH into the computer attached to the network. Here is the information for the computer attached to the network (it is the same for both networks):
   - IP Address: 192.168.0.2
   - Username: student
   - Password: student

3. Find the file "secret.txt" in the home directory and view its contents. 
   
4. Repeat steps 1-3 for the second wireless network. Upload the two secrets to Learning Suite.

## Objectives

- Gain experience with WiFi security
