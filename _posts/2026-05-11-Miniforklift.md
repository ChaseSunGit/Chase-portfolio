---
layout: post
title: "GT Miniforklift - a hinge free, under-actuated cable-drvien exoskeleton"
author: "Chase Sun"
categories: wearable-robotics
tags: [cad,controls,embedded,mechatronics]
image: EPIC_Title.jpg
---

Workplace injuries are common place for high-intensity manual labor workers in the US, especially in environments where heavy duty equipment cannot be used. Exoskeletons have been used to increase the work capacity and reduce injury for the user in this application, but typical designs only target single joints and often incorporate rigid hinges which impede natural motion. As a master's student in the EPIC lab at Georgia Tech, I am working to design a multi-jointed, completely hinge free exoskeleton to reduce knee & back injuries for manual laborers.

## Design Overview
![Miniforklift Design Diagram]({{ site.baseurl }}/assets/img/MF3K/EPIC_Design.jpg){: .img-breakout}

## Operating Principle
![Miniforklift Operations principle]({{ site.baseurl }}/assets/img/MF3K/EPIC_Lift_Painted.jpg){: .img-wrap-left}
The soft exoskeleton works by having 2 motors mounted on the thighs to reel in the paracord of the exoskeleton. The cord travels down to the knee and back up, forming a double pulley. It then by-passes the thigh using soft PTFE tubes and attaches at the back, where strain gauges measure the tension in the cord and closing the control loop. When the cord is reeled in, the exoskeleton exerts positive extension work on how 3 joints most involved in lifting motion (knee, hip, and back), and therefore reducing muscle activation and metabolic costs of the user thus reducing the likelihood of injury.

## Control Loop
![Miniforklift Controls]({{ site.baseurl }}/assets/img/MF3K/EPIC_Control.jpg){: .img-breakout}
Since the exoskeleton is actuated by soft paracord, the controller must be adapted to the reality that the actuators can only pull and not push, and that force can only be exerted in 1 direction. The controller hierarchy consists of 3 levels:
 - High level: A finite state machine that determines if the user is in lifting or any other activity and outputs the desired tension in the cord.
 - Mid level: An admittance controller that outputs velocity commands to the actuator based on the force required.
 - Low level: A PD controller within the actuator to reach desired velocity.
 
 All 3 levels work in series to allow the exoskeleton to near instantanously output desired torque on the assisted joints.

## CAD Render
 ![Miniforklift CAD]({{ site.baseurl }}/assets/img/MF3K/EPIC_CAD.jpg){: .img-breakout}
