---
layout: post
title: Neon Hands On
---

> "Installation isn't always easy"

Challenge accepted.

***

[Nervana's neon](https://github.com/NervanaSystems/neon) is a python-based deep learning library and part of their full stack deep learning framework, from silicon to application. It runs on CPU, GPU, and Nervana hardware (see, full stack!). It's supposed to be easy to use and extensible, and I won't argue with either because I'm just trying to get the installation done at this point. 

It took me just under 24 hours to get neon up and running. No, I wasn't continuously working for 24 hours trying to get it installed, but I was working it on and off for a couple hours over the course of two afternoons. 

![so close to getting neon working](/./images/error-neon-mnist.PNG)

Some "gotchas" I ran into:
* works on CPU (yay!) but Windows isn't supported (boo!)
* more dependencies than I anticipated (which I'm curious about, is it because my machine wasn't already setup for ML/DL?)
* installation instructions that left me wanting more

Of course my work computer is a Windows machine and I'm nowhere near lucky enough to have it dual boot Linux (Ubuntu). I did have a personal laptop that I ran into the ground a few years ago that would have been the perfect candidate. Instead, my only option was my personal MacBook Pro (my desktop graphics card died during my recent move to the Bay Area), which was recently replaced and I was fairly confident it wouldn't catch fire if I asked it to do some MNIST deep learning. The obvious bummer here is installation required downloading dependencies and I couldn't bring my MBP onto the nice work wifi. So I was limited to only afternoon/evening neon time. Which makes this a great time to ask my manager from a work MBP for Christmas!!

I wouldn't call the installation process hard so much as it was "involved". 

* Attempt 'quick install": https://github.com/NervanaSystems/neon#quick-install
..* Fail - MBP's new to dev setup need to confirm Xcode agreements, etc. 
* Confirm Python (2.x), git, etc.
* Follow these: http://neon.nervanasys.com/docs/latest/installation.html
..* Install pip, virtualenv, h5py, pyaml, pkg-config (I had to flip back and forth between pip and easy_install)
..* Install OpenCV
..* OpenBLAS (CPU, suboptimal performance warning a total non-issue for me)
* Keep working the dependency installs until you get "make" to work, per quick install steps. You may have 2 virtual envs running and have cloned neon like 3 times but it will work.

![mnist working in my terminal](/./images/working mnist in neon.png)

So my first question (and I haven't done any research) is "why"? Why can't I run Nervana neon on Windows? What does Windows do (or not do)? Will this be supported in the future? My inital thoughts are this could very well limit enterprise type customers who are Windows shops. How do we enable those data scientists and developers? Or do we care? If the "we" in the last two questions is confusing to you, perhaps you should read [this](https://www.nervanasys.com/intel-nervana/). 

Next up, I'll do some of the other tutorials and put together a beginner DL post. 

01111000 01101111 01111000 01101111,

Amara
