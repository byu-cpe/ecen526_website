---
layout: lab
toc: false
title: Site Survey
number: 2
---

## Overview

Understanding a wireless network's performance in any environment can be quite challenging, especially in a home. This lab aims to give you better insights into your home's WiFi and how to characterize a wireless network's performance by doing a site survey.

Since each home is different, I don't want to limit your exploration, so I do not require specific measurements. However, I will reward thoroughness. Here are some things you might consider measuring:

- Run an Internet speed test at various locations in your house (for example using [speedtest-cli](https://github.com/sivel/speedtest-cli)).

- Run [iperf3](https://iperf.fr) on your local network. You can do this by setting up a server (e.g., Raspberry Pi, desktop, laptop, etc.) and then, with a laptop, measure different spots in your house.

- Compare the results of iperf3 with the Internet speed test to see if they are different.

- Determine the channel allocation of your access points as well as your neighbors' access points.

- Look at the signal strength of your neighbors' access points.

- Measure channel utilization.

- Look at how distance from your access point or the access point's placement makes a difference to throughput. 

- Measure your network's utilization over time

I want you to make this assignment personal. We all have issues with our WiFi network that we would like to make better. Figure out what is wrong and then figure out how to improve it (you don't have to improve it, though). If you think your WiFi network has no issues, then prove it, and explain what you did to make it that way.

Your experiments must be thoughtful and well planned out. Think about the implications of your design decisions. For example, what are the consequences of running iperf3 tests when both the server and client are wireless? What are the implications of using UDP instead of TCP (the default) for your iperf3 tests? Think about these things as you perform your experiments.

## Requirements

For this lab, you will turn in a **2-page report**. Your report must contain the following three sections:

1. Current state of WiFi in your home. Give us an idea of what you are working with. For example, how many access points do you have? What kind of configuration you have (shared between roommates, manage by your apartment complex, etc.)? Do you have any WiFi issues?

2. A detailed analysis of your home's WiFi. This section is the meat of your report. Once again, I leave this up to you to figure out based on your home and WiFi issues you might be having. However, it should contain the following information:
    - The experiments you performed
    - Rationale for why you performed those experiments
    - The results of your experiments

3. Suggested improvements you can make to your network and why you think those changes would help. For example, would buying more access points help? Would changing the position of your APs help? Some of these things might be out of your control, but I want you to think about what changes you would make and why they would help.

