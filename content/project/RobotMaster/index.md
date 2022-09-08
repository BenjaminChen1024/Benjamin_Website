---
title: Robomaster - Engineer Robot
summary: RoboMaster University Series (RMU), initiated by DJI.
tags:
- Robot
- Robomaster
date: "2021-09-04T00:00:00Z"

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

I am a member of engineering embedded software in the 21st season of Scut Robot Lab, responsible for engineering robot hardware deployment and embedded software research and development.

👉 Github: https://github.com/BenjaminChen1024/21_Engineer_Top

## **Engineer Robot**

Engineer robot is responsible for competing for its own resources and resurrecting its own robot, which consists of two parts: mobile chassis and upper mechanism. The mobile chassis includes the McNamham wheel, the rescue mechanism and the card swiping mechanism which can move in all directions. The upper mechanism includes lifting mechanism, extending mechanism, flipping mechanism and clamping mechanism.

{{< figure src="mechine.jpg" caption="Engineer Robot Model" numbered="true" >}}

## **Hardware**

Engineer robot hardware uses STM32F405 chip as the controller. Robomaster M3508 motor and 2006 motor are used as drivers. CAN communication protocol and serial communication protocol are adopted. Photoelectric gate and visual camera are used as sensors.

{{< figure src = "hardware.png" caption = "Engineer Robot Hardware" numbered = "true" >}}

## **PCB Development**

Engineer robot PCB has Chassis and Topper, which are responsible for controlling Chassis and Topper hardware devices respectively.

Chassis PCB consists of STM32F405 chip, IMU chip, CAN communication module, serial port communication module, IIC communication module, and DBUS communication module.

{{< figure src = "Chassis.jpg" caption = "Engineer Robot Chassis PCB" numbered = "true" >}}

Topper PCB is composed of STM32F405 chip, CAN communication module, serial communication module, IIC communication module, free IO port, overcurrent protection module and relay module.

{{< figure src = "Topper.jpg" caption = "Engineer Robot Topper PCB" numbered = "true" >}}

## **Softwork**

Engineer robot software is based on FreeRTOS real-time operating system, and the different modules of the robot are controlled by multi-thread management. These include motor control, visual assistance, mode switching, drop protection, handle key control and so on.

{{< figure src = "software.png" caption = "Engineer Robot Software" numbered = "true" >}}


## **Robot Control**

Engineer robot control is divided into action group and automatic group. The action group is assigned by the state machine to execute individual actions, including rotation, flip, extension, lift, cylinder control. The automatic group is to control the state machine through continuous instructions to execute corresponding continuous actions, including one-key mining, one-key exchange, one-key reset, automatic rescue, one-key interrupt protection.

{{< figure src = "control.png" caption = "Engineer Robot Control" numbered = "true" >}}


## **Debug**

In order to make the movement of the robot more stable and prevent various accidents in the competition, we need to debug the robot again and again, and record its test parameters such as: clamping success rate, exchange success rate, chassis moving speed, etc.

{{< video src="debug.mp4" controls="yes" >}}

## **Competition**

Through continuous iteration and debugging, we finally won the victory and won the first prize of the National College Student Robotics Competition RoboMaster2021 Mecha Master Competition.

{{< figure src = "competition.jpg" caption = "My engineering robot and I" numbered = "true" >}}
