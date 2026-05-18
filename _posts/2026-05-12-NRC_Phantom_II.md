---
layout: post
title: "NRC Phantom II - an ultra-light weight, high-precision greenhouse gas sensor"
author: "Chase Sun"
categories: electronics-optics
tags: [embedded,cad,optics,mechatronics,sensing]
image: NRC_Title.jpg
---

Methane is a highly potent greenhouse gas that has been historically poorly measured. There is an increasing demand for portable, sensitive, and cost-effective instruments to better understand the emission of methane and its effect on the changing climate. As a mechantronics engineer at the National Research Council (NRC) between 2021 and 2024, I developed a laser-based methane sensor that allows climate scientists to accuately measure methane emissions with an ultra light-weight, UAV deployable package.

## Mechanical, Electrical, and Optical Design
![PhantomII Design Diagram]({{ site.baseurl }}/assets/img/PhantomII/NRC_Design_Diagram.jpg){: .img-breakout}

## Physical Assembly
![PhantomII Physical package]({{ site.baseurl }}/assets/img/PhantomII/NRC_Physical.jpg){: .img-wrap-left}
The physically assembled sensor with slightly extended formfactor but identicial electronics and optical design. The fully assembled sensor weighs __less than 1kg__ and measures at a sensitivity __less than 1 parts-per-billion__, making it easily deployale on mid-sized commerical UAVs.

## Upgrade From Previous Design
![PhantomII Size comparison]({{ site.baseurl }}/assets/img/PhantomII/NRC_2sensor_Ontop.jpg){: .img-wrap-right}
Two versions of the sensor, the open cell version Phantom II (right) and close cell version Chameleon (left) sitting on top of the previous NRC methane sensor. The weight was reduced from __25KG__ to __3KG__ for the closed cell sensor with no sacrifice in sensitivity due to highly custom electronics and embedded software.

## Deployment
![PhantomII Deployment]({{ site.baseurl }}/assets/img/PhantomII/NRC_Deployment.jpg){: .img-wrap-left}
The device has been deployed across Canada including near oil & gas facilities in Northern Alberta and the Arctic coast in collaboration with Geological Survey Canada and Envornmental & Climate Change Canada to quantify total methane emissions in the country. The sensor seen here is mounted on a DJI Matrice 300 drone as it is prepared to take measurements.

## Results
![PhantomII Deployment]({{ site.baseurl }}/assets/img/PhantomII/NRC_Results.jpg){: .img-wrap-right}
This is the result of a single collection done by the sensor mounted on an UAV measuring methane emissions in the Mackenzie Delta region of Northern Canada. The heatmap is the result of a fusion between GPS data, ambient conditions, and concentration measurement. Higher concentrations are shown in green around the slump site.

## Associated Publications
M. Beattie, __C. Sun__, R. MacLeod, N. Sabourin, P. Morse, J. Corbin, J. Oliaee,__ “_Ultra-Lightweight Mid-IR Methane Sensor for UAV-based measurements_”, Journal of Optical Express, Submitted for review

J. Oliaee, R. MacLeod, __C. Sun__, M. Beattie, S. Dallimore, P. Morse, “_Measurement of natural methane emissions in the western Canadian arctic using an ultra-lightweight laser spectroscopic sensor aboard a small UAV_”, CabCH4 symposium, Ottawa, Canada, May 2024

__C. Sun__, J. Oliaee, N. Sabourin, G. Smallwood, “_Development of a Lightweight UAV-Mountable Open-Cell Methane Sensor Using Mid-Infrared Tunable Diode Laser Interfaced with a Low-Cost Embedded Platform._” Onboard Sensing, Analysis, and Reporting (OSAR) conference. Riverside, CA, March 2023
