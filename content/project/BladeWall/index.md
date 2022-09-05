---
title: Blade Wall
summary: Somatosensory multi - motor array synchronous control system.
tags:
- Kinect
- Other
date: "2022-09-05T00:00:00Z"

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

The Blade Wall is a student research and development project jointly developed by Scut Robot Lab and DJI. I am the head of the embedded system of the project, responsible for the hardware scheme and the embedded underlying firmware system of blade wall.

## **Blade Wall**

The Blade Wall is composed of the upper computer and firmware system. The upper computer is based on Unity for body sensing monitoring and pattern algorithm implementation, while the lower computer is based on STM main control chip for motor control algorithm implementation and multi-mode underlying design.

{{< video src="BladeWall1.mp4" controls="yes" >}}

## **Development**

In order to make the Blade Wall more perfect, we use different algorithms for motor control, such as Kalman filter, interpolation fitting, PID controller and so on. And through a lot of debugging, we found the appropriate parameters to make the motor rotation more smooth and pattern switching more coherent.

{{< video src="BladeWall0.mp4" controls="yes" >}}

## **Latest**

Work continues, with the latest Blade Wall replacing the somatosensory interaction, focusing on the continuity and beauty of pattern switching.

{{< video src="BladeWall2.mp4" controls="yes" >}}
