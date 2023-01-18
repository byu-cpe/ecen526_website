---
layout: lab
toc: false
title: Site Survey
number: 4
---

## Overview

Understanding a wireless network's performance in any environment can be quite challenging, especially in a home. This lab aims to give you better insights into your home's WiFi and how to characterize a wireless network's performance by doing a site survey. I want you to make this assignment personal. We all have issues with our WiFi network that we would like to improve. Figure out what is wrong and then figure out how to improve it

Since each home is different, I don't want to limit your exploration, so I do not require specific measurements or how you perform those measurements. However, I will reward thoroughness. There are three parts to this lab.

### Part 1

You first must characterize the WiFi in your home (this is left purposefully vague to allow for flexibility). Here are some things you might consider measuring to characterize your home:

- Run an Internet speed test at various locations in your house (for example using [speedtest-cli](https://github.com/sivel/speedtest-cli){:target="_blank"}).

- Run [iperf3](https://iperf.fr){:target="_blank"} on your local network. You can do this by setting up a server (e.g., Raspberry Pi, desktop, laptop, etc.) and then measuring different spots in your house with a laptop.

- Compare the results of iperf3 with the Internet speed test to see if they are different. Are the iperf3 results much different from your Internet speed test? Why or why not? Are you getting the Internet speed you are paying for? Why or why not?

- Determine the channel allocation of your access points as well as your neighbors' access points. Look at the signal strength of your neighbors' access points.

- Measure channel utilization.

The result of this part should describe what measurements you performed, why you performed them, and the results of your measurements. A general floor plan of your home with a heat map or points you measured would be helpful. These measurements will be the baseline for your experiment in part 2.

### Part 2

Based on the results of part 1, pick something to change about your environment that you think will make your WiFi better. Design a small experiment to run. For example:

- Temporarily move your access point into a different part of your house.

- Switch your access point to a less congested or more congested channel.

- Temporarily set up two or more access points in your house. If you already have a few access points, remove some of them.

- Measure performance at different times of the day.

- Measure performance on different devices (e.g., tablet vs. laptop vs. smartphone, old WiFi device vs. new WiFi device, etc.)

Your experiments must be thoughtful and well planned out. Think about the implications of your design decisions.

### Part 3

Once you have made the change in part 2, rerun the same tests you ran in part 1. See how the performance of your network changed. If you feel like different measurements need to be collected compared to part 1, feel free to make those adjustments. Did your changes to your WiFi network work as expected based on the results?


## Requirements

For this lab, you will turn in a **2-page report** using [this template]({% link assets/site_survey_template.tex %}){:target="_blank"}. Your report must contain the following three sections:

1. **Part 1**. Describe the current state of WiFi in your home. Give us an idea of what you are working with. For example, how many access points do you have? What kind of configuration do you have (shared between roommates, managed by your apartment complex, etc.)? Do you have any WiFi issues? Report on and display the results of your part 1 measurements. Why did you perform those measurements? Were you surprised by any of the results? This section should contain a floor plan, chart, or graph showing the results of your measurements.

2. **Part 2**. Based on your results from part 1, describe what you changed about your environment. Why did you make those changes? How do you think your WiFi performance will improve because of these changes? Give your hypothesis on the impact the changes will have on part 3.

3. **Part 3**. Report on and display the results of your part 3 measurements. Was your hypothesis correct? Why or why not? What would you change about your experiment if you could do it again? This section should contain a floor plan, chart, or graph showing the results of your measurements.
