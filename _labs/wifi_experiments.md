---
layout: lab
toc: false
title: Networking Experiments
number: 1
---

## Overview

This lab aims to give you experience with network performance under different conditions and the tools used to measure network performance. There are many tools out there, but the one we will be using is [iperf3](https://iperf.fr){:target="_blank"}. This tool uses a client-server paradigm to test network performance. The client connects to a server and sends data at a specific rate (by default, it sends as fast as possible). The server receives the data and reports how fast the data was sent. 

## Objectives

1. Get a feel for how networking characteristics change with different environmental factors.

2. Become familiar with `iperf3`.

## Requirements

To complete this lab, you will need a laptop to act as the client. I will provide the server. If you do not have access to a laptop, let me know, and we can figure something out. You will perform the experiments outlined below and answer questions about those experiments. You must do all experiments on campus.

## Setup

First, install `iperf3` on your laptop.

Second, get familiar with `iperf3` by running it a few times. Figure out how to set up a client and server on the same computer. Look at the command-line options that you can provide. To do this lab, you will need to change some of the default options (such as the duration and protocol used). Once you feel comfortable with `iperf3`, you can do the experiments.

## Experiments

For all experiments, set the `iperf3` run time to 2 minutes, and the interval between throughput reports to 1 second. The `iperf3` servers are running at `ecen426.byu.edu`, `ecen224.byu.edu`, and `aq.byu.edu`. Only one client can connect to an `iperf3` server at a time, which is why I provide three. If you have access to a wired desktop computer and you want to run your own server, that is fine. Please use the same server for all of your experiments to maintain consistent results. For all experiments, consider piping the results to a file so you can refer to them later.

1. Run `iperf3` using **TCP** on your laptop **wired** into the campus network.

2. Run `iperf3` using **UDP** on your laptop **wired** into the campus network. By default, the throughput gets limited to 1 Mbps when running `iperf3` in UDP mode. Set the throughput to be unlimited for these experiments.

3. Run `iperf3` using **TCP** using the **campus WiFi**.

4. Run `iperf3` using **UDP** using the **campus WiFi**. Make sure to set the throughput to unlimited.

5. Run `iperf3` using **TCP** while walking around a building. When walking around, try to go between different access points (e.g., don't just walk around in a small circle in one room).

6. Run `iperf3` using **UDP** while walking around a building. Use the same path you took for the previous experiment and make sure to set the throughput to unlimited.

## Report

Graph all reported throughputs (`iperf3` calls them "Bitrate") for each experiment on a time-series graph. Then answer the following questions:

1. At the end of a run, `iperf3` reports the amount of data transferred and the bitrates of both the sender (client) and receiver (server). See [here for an example]({% link assets/iperf.png %}){:target="_blank"}. Is the amount of data sent by the sender different from the amount of data received by the receiver? If so, using your knowledge about TCP and UDP, explain why.

2. Which setup had higher throughput: wired or wireless? Explain why.

3. Explain what happened when you started walking around while performing experiments compared to the stationary experiments.

4. Compare the results of experiments 5 and 6. How are the results of these experiments similar or different?
