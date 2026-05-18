---
layout: post
title: "Sonic Chippy - an ultrasonic wind sensor"
author: "Chase Sun"
categories: electronics-optics
tags: [mechatronics,embedded,sensing]
image: Wind_Title.jpg
---

When I deployed my methane sensor at the Arctic Coast, it was clear that wind plays a huge factor in the gas concentration measured. The commercial cup-and-arrow wind sensor we deployed was expensive, heavy, and very delicate. I decided to create a sonar-based compact wind sensor with the beaglebone black single board computer using assembly to program ultra-high frequency data capture.

## Operating Principle
![Ultrasonic Operations principle]({{ site.baseurl }}/assets/img/Wind/Wind_Physics.jpg){: .img-breakout}
The sonic wind sensor features 3 orthogonal pairs of opposing sonar transceivers where the transmitters are periodically pulsed and the travel time to the receivers are measured. This time is equal to the distance between the transceivers divided by the sum of the speed of sound and the parallel component of the wind. Accurately measuring this time means 3 orthogonal components of wind speed can be calculated.

## Mechatronics
![Ultrasonic Operations principle]({{ site.baseurl }}/assets/img/Wind/Wind_Schematic.jpg){: .img-wrap-left}
The Beagonebone black SBC is used since it can handle ultra-fast real time operation with assembly. A custom capeboard is used to amplify high-impednace digital signals from the BBB to +-10V low impedance output to power the piezo-electric speakers. The signals from receivers are then read as digital inputs by the BBB with constant polling to precisely calculate time required for the sound to travel. The circut, along with the high-speed assembly code, allows the sensor to measure 3D wind at __1000Hz__, compared to a traditional wind cup sensor which can only measure 2D wind at ~1Hz.

## Deployment
![Ultrasonic Operations principle]({{ site.baseurl }}/assets/img/Wind/Wind_deployment.jpg){: .img-breakout}
Here the ultrasonic sensor is deployed along with a traditional wind cup sensor to measure the long term stability of the sensor.