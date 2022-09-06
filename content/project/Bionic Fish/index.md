---
title: Bionic Fish
summary: Underwater bionic robotic fish based on vision for dynamic target tracking.
tags:
- Robot
- Bionic
date: "2022-09-06T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  # caption: Photo by rawpixel on Unsplash
  focal_point: Large

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
# url_code: ""
# url_pdf: ""
# url_slides: ""
# url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

I was in charge of the Bionic Fish project, responsible for the development of embedded systems and machine vision.

## **Bionic Fish**

Although the traditional propulsion mode of "propeller + steering rudder" can better provide large thrust and high speed, its application in the above occasions is limited due to its inherent characteristics, such as obvious fluid disturbance and poor low-speed maneuvering performance. Bionic Fish can meet the characteristics of small turbulence, high propulsion efficiency, small wake characteristics and good maneuverability.

{{< figure src="Design.png" caption="Bionic Fish Design" numbered="true" >}}

## **Model**

The Bionic Fish model includes mechanical design and hardware deployment. Through the double structure with waterproof paint, can effectively improve the water - proofing of fish. The Bionic Fish moves freely through the water by swinging its fins and caudal fins. 

{{< figure src = "Model.png" caption = "Bionic Fish Model" numbered = "true" >}}

## **Hardware**

Hardware includes power supply, switch, sensor, controller, camera, drive element, indicator element. The stability of the hardware in water can be improved by designing the PCB and arranging the space properly.

{{< figure src = "Hardware.png" caption = "Bionic Fish Hardware" numbered = "true" >}}

## **Control**

Bionic Fish through infrared sensor, machine vision parameters, MPU6020 Angle sensor as input, through the low-pass filter and PID controller output error parameters to control the steering gear rotation Angle, so as to control the posture and movement of the Bionic Fish.

{{< figure src = "Control.jpeg" caption = "Bionic Fish Contorl" numbered = "true" >}}


## **Future**

Because the steering gear of the original model is directly connected to drive the fin, there are certain shortcomings, such as large mass, large occupancy volume and slow response speed. The new Bionic Fish will be based on the line pull technology for the fish tail adaptive control, using a servo motor with faster response speed to drive.

{{< figure src = "Future.jpeg" caption = "New Bionic Fish Design" numbered = "true" >}}
