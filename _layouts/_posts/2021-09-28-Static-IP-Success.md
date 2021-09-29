---
layout: post
title: "Static IP Address Success!"
date: 2021-09-28
---

Today I got the static IP address on the opentrons robot set up. Now every time the robot powers on it won't change. This is helpful because now we can run a batch script, which I will put in the opentrons repo, to automatically transfer input files to scripts. We can also run a bash script on the robot itself called ./clean to remove any unnecessary .ipynb, .txt, .jpg, etc. This was a big step towards making the robot user friendly for operators. 
