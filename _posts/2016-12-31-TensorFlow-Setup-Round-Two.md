---
layout: post
title: TensorFlow Setup (Round Two)
---

I already have TensorFlow up and running on my MacBook Pro (MBP). Shortly after my adventure with setting up Nervana neon, I moved on to getting TensorFlow up in the same way. It was fairly easy (I almost said straightforward, but that's not quite it) because I chose to run it in a Virtualenv setup because that's how I was running Nervana neon. I chose to do both CPU-only as well.

For whatever reason, I decided to get TensorFlow up and running on another device, my home PC which I mostly use for gaming. In fact, it was my boyfriend's old workstation so in the screenshots you'll see "JJ". No, he didn't do the work. It was all me!

TensorFlow has really good [setup instructions](https://www.tensorflow.org/get_started/) for a variety of ways to run it depending on your operating system. It feels very much like tasks a system administrator would love to do. And as a developer that prefers to stay a few steps removed from the hardware, I couldn't help but notice how uncomfortable most of these steps made me. 

I decided to go the route of [Pip install on Windows](https://www.tensorflow.org/get_started/os_setup#pip_installation_on_windows), thinking that sounded like something I could do (in fact I've worked with Python, Pip, and Windows before so all of this sounds great!). I got a fresh Python 3.5 via Anaconda and followed the CPU-only step. It looked like it was trying to pull dependencies and I didn't see any errors. This is good right? Who knows. I could never get it to an intelligent failure point. I tried testing my installation and still nothing helpful. I'm an impatient person, just ask my boyfriend, so I moved on. 

[Conda environment](https://www.tensorflow.org/get_started/os_setup#using_conda) sounded very similar to Virtualenv, so I thought that would be my next step. It gave me my CPU-only requirement and looked like something I could make work or see some obviously failure. 

![source activate tensorflow](/./images/source_activate.PNG)

Maybe one day I'll remember I'm working in bash. But why not type out a bash example? Or should I know that already? Who would know that? A sys admin?

I have my Conda environment up, its running Tensorflow! Yes! Now let's test the installation. Looks like there is an error, which I expected. Filepaths might be the issue, but the Tensorflow instructions give me a hint.

![file location](/./images/tensorflow_file_location.PNG)

That almost looks like the hints from the instructions. Navigate to that directory, run the demo model. SUCCESS!

So here's my tips for getting TensorFlow running on a Windows 10 Machine:

* Pip install on Windows -> Install Anaconda
* Give up on that
* Reset -> start a conda env
* Run your TensorFlow demo model after you figure out where your files are


01111000 01101111 01111000 01101111,

Amara
