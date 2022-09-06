---
title: LED Dot-matrix
summary: Firmware and APP software system development based on LED Dot-matrix.
tags:
- Electron
- LED
date: "2021-10-30T00:00:00Z"

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

This project originated from an academic competition, based on LED Dot-matrix PWM control to adjust a variety of colors, with touch device and APP software, design and manufacture of intelligent tone modulation light system

## **Hardware**

The product consists of 4 × 7 LED to form the LED dot matrix, including MCU main control module, voltage regulator module, WiFi module, touch module.

{{< figure src = "SCH.png" caption = "Hardware - Schematic Diagram" numbered = "true" >}}

{{< figure src = "PCB.png" caption = "Hardware - Circuit Diagram" numbered = "true" >}}

## **Software**

A variety of images can be designed through the LED imaging principle. The output voltage duty cycle can be controlled by PWM to control the color and brightness of LED. The intelligent tone modulation light system can be realized with the key, touch wheel and touch slider

{{< figure src = "Software.png" caption = "Software" numbered = "true" >}}

## **APP Development**

Based on the Tuya loT platform MCU SDK development cloud, so as to develop the 6 functions of the product, respectively, switch, brightness, breathing light, static, color, animation.

{{< figure src = "APP.png" caption = "APP" numbered = "true" >}}

In order to achieve a simple and beautiful page, we use blue as the main color of the UI interface. It includes the main interface, breathing light interface, intelligent interaction interface.

{{< figure src = "UI.png" caption = "UI" numbered = "true" >}}

Through continuous modification and debugging, we designed a simple and beautiful APP control system.

{{< figure src = "Edition.png" caption = "Edition" numbered = "true" >}}

## **Product Display**

👇🏻 Please see the video Product Display below

- LED Dot-matrix Display

{{< video src="Display1.mp4" controls="yes" >}}

- APP Control Display

{{< video src="Display2.mp4" controls="yes" >}}

