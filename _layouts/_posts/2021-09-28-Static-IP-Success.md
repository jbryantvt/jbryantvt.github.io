---
layout: post
title: "John Bryant, static IP success!"
date: 2021-09-28
---

Today I successfully set up the static IP address for the opentrons robot. Previously, the IP address would change every time it was turned on. With the new static address, it is now possible to transfer files onto the robot seamlessly using a batch script. There is also a ./clean script in the root directory of the robot itself capable of deleting any unnecessary .ipynb, .txt, .jpg, etc. This is an important step forward for making the robot user friendly for an operator.
