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

I have set up two wireless networks, "ECEn526-WEP" and "ECEn526-WPA2" in the Embedded Lab (EB 438). Each of these networks has a computer attach to it. Your job is to gain access to the network, SSH into the computer, and retrieve the secret off of the computer. There is two secrets in total, one for each network. You will then upload the secrets to Learning Suite. Since the point of the lab is to learn about WiFi security and not hacking, I will give you the username and password of the computer attached to the network.

Here are the steps of the lab:

1. Gain access to the network. You are on your own for this one. There are plenty of tutorials online for how to do this for WEP and WPA (and resources at the bottom of this page). Good luck! To make the lab a more consistent experience for everyone, I am providing a Raspberry Pi as an SSH endpoint for you to log into from *on campus*. It has a WiFi adapter that is capable of going into monitor mode and injecting frames and the aircrack-ng software suite. This device has two wireless adapters. For this lab, you will only be using the `wlan1` interface.
    - IP Address: 10.35.120.211
    - Username: student

     To make sure two people are not using the computer at the same time, I have created a document to schedule the device. The link to the document will be shared over LS. When you log into the device, create a folder with your NetID and change into that directory so the files you create will be self contained.
   
2. SSH into the computer attached to the network. Here is the information for the computer attached to the network:
    - Network Name: ECEn526-WEP
      - IP Address: 192.168.0.11
      - Username: student
      - Password: student

    - Network Name: ECEn526-WPA2
      - IP Address: 192.168.0.2
      - Username: student
      - Password: student
      
3. Find the file "secret.txt" in the home directory and view its contents. 
   
4. Repeat steps 1-3 for the second wireless network. Upload the two secrets to Learning Suite.

## Objectives

- Gain experience with WiFi security

## Resources

- Aircrack-ng has a good tutorials on how to crack WEP and WPA2. You can download them [here]({% link assets/lab3_resources.zip %}).

- To perform some of the attacks, you need to be able to capture packets and inject frames. The ability to capture and inject depends on your computers WiFi adapter firmware. If your wireless chipset does not support these capabilities, you can borrow a USB WiFi adapter from me.

- This lab should only take around 45 minutes to complete. If the lab takes longer than that, there is a chance you are doing something wrong. If you are stuck, ask for help.

- WEP keys is hex. Aircrack will return the key in the following format: XX:XX:XX:XX:XX:XX:XX:XX:XX:XX:XX:XX:XX. To join the WEP network, you will want to remove all of the colons: XXXXXXXXXXXXXXXXXXXXXXXXXX.
