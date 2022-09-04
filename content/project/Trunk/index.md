---
title: Trunk Robot
summary: Biomimetic elephant trunk robot based on wire pulling technology.
tags:
- Robot
date: "2022-09-04T00:00:00Z"

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

I am the general manager of the self-developed project - the bionic elephant trunk robot based on the wire pulling technology. I was responsible for personnel scheduling, task allocation and overall positioning design of the project. I was also responsible for embedded software development and hardware topology design.

👉 **Github**: https://github.com/BenjaminChen1024/Trunk-Robot

## **Trunk Robot**

Our team designed the bionic mechanical elephant trunk ecological restoration robot, based on the bionic wire pulling technology and the bionic mechanical transmission principle of elephant trunk.

{{< figure src="Trunk.jpg" caption="Trunk Robot" numbered="true" >}}

## **Mechanical Structure**

In terms of mechanical design, the robot adopts modular design, including: land-air integrated chassis, 360-degree rotating head, multi-degree-of-freedom line driven elephant trunk and modular end actuator, so as to realize ground movement, climbing, rotation, flexible movement of elephant trunk, clamping, cutting and other functions.

{{< figure src = "Mechanical Structure.png" caption = "Trunk Robot Mechanical Structure" numbered = "true" >}}

## **Hardware**

The power supply part is powered by 24V battery, and the chassis is driven by four 6020 motors to realize the free movement of front and back. The elephant trunk is controlled by a 6020 motor to control the YAW shaft of the cradle head and four 3508 motors to drive the wire pulling mechanism. The power supply independently supplies power to the STM32 main control board, which supplies power and controls the end-actuator steering gear. The power supply is supplied to the Raspberry PI through the 24V to 5V step down module, and the Raspberry PI supplies power to the camera through USB.

{{< figure src = "Hardware.png" caption = "Trunk Robot Hardware" numbered = "true" >}}

## **Softwork**

The embedded underlying driver is developed based on STM32 chip, and FreeRTOS real-time operating system is used for task management. System tasks include: remote control communication, mode switching, dropped line protection, PC communication, motor control, steering gear control, debugging mode, system reset. Initialize the Flash, Timer, CAN, and UART.

{{< figure src = "software.png" caption = "Trunk Robot Softwork" numbered = "true" >}}


## **Machine Vision**

Visual module uses raspberry sent 4 b as operation platform, driven by industrial camera to capture frames flow using OpenCV vision library for feature extraction, and the data sent to the embedded microcontroller, visual AIDS control functions, through object capture and fixed position, realize automatic clearing up the rubbish, automatic aerial work, etc.

{{< figure src = "Machine Vision.png" caption = "Trunk Robot Machine Vision" numbered = "true" >}}


## **Product Display**

{{< video src="Product Display.mp4" controls="yes" >}}

## **Awards**

- [Second prize in the 10th National College Students Mechanical Innovation Design Competition](http://umic.ckcest.cn/)
- [Third prize in the 15th National College Students Energy Conservation and Emission Reduction Social Practice and Technology Competition](http://www.jienengjianpai.org/)
- [Winning Prize in the physical group of the second round of the Southern Division of Huawei Embedded Software Competition in 2022](https://bbs.huaweicloud.com/forum/thread-193584-1-1.html)
