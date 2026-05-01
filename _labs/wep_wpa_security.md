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

In this lab, you will hack into two wireless networks, one protected by WEP and another protected by WPA2. The lab will teach you how trivial it is to crack WEP and WPA2 with a weak password.

I have set up two wireless networks, "ECEn526-WEP" and "ECEn526-WPA2", in the Embedded Lab (EB 438). Each of these networks has a computer attached to it to help you in cracking the passwords. Your job is to discover the password for each network and upload it to Learning Suite.

You are on your own for figuring out how to attack the network. There are plenty of tutorials online for how to do this for WEP and WPA (and resources at the bottom of this page). Good luck! 

You are welcome to use your own device for this lab, but it needs to be capable of capturing and injecting WiFi frames, which depends on your computer's WiFi adapter firmware. To make the lab a more consistent experience for everyone, I am providing a Raspberry Pi as an SSH endpoint for you to log into from *on campus*. It has a WiFi adapter that is capable of going into monitor mode and injecting frames, and the aircrack-ng software suite. This device has two wireless adapters. For this lab, you will only be using the `wlan1` interface. The IP address and login information are on the Lab 3 Details Content Page on Learning Suite. If you use the Raspberry Pi, to make sure two people are not using it at the same time, I have created a document to schedule the device. The link to the document will be shared over LS. When you log in to the device, create a folder with your NetID and change into that directory so the files you create are self-contained. Delete your files from the Raspberry Pi when you have finished the lab.
   
## Objectives

- Gain experience with WiFi security

## Resources

- Aircrack-ng has good tutorials on how to crack WEP and WPA2. You can download them [here]({% link assets/lab3_resources.zip %}).

- This lab should only take around 1 hour to complete. If the lab takes longer than that, there is a chance you are doing something wrong. If you are stuck, ask for help.
