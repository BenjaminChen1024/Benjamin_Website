---
title: Deuterium Lamp SMPS
summary: Deuterium lamp continuous operation Switching Mode Power Supply design.
tags:
- Electron
- SMPS
date: "2022-05-20T00:00:00Z"

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

Deuterium lamp is a kind of ultraviolet light source, which emits light in the wavelength range of 190~400nm continuous spectral band. 

By comprehensively utilizing the technical advantages of linear switching mode power supply and modern power electronics technology, we can make the deuterium lamp power supply miniaturized, intelligent, and extend the service life of the traditional deuterium lamp.

## **Working Principle**

The voltammetry characteristic curve of deuterium lamp gas discharge is as follows. The working range of the deuterium lamp is the working range of the arc type and discharge on the charging and discharging characteristic curve of the gas cathode.

{{< figure src = "Working Principle.png" caption = "Working Principle" numbered = "true" >}}

## **Technical Index**

According to the overall design and the requirements of deuterium lamp electrical parameters, combined with the market demand and own level, I made the expected design and planning for the designed deuterium lamp power supply parameters.

{{< figure src = "Technical Index.png" caption = "Technical Index" numbered = "true" >}}

## **Circuit Design**

The voltage of the power module is boosted from 24V to 80V, so the BOOST converter is used as the main circuit topology.

{{< figure src = "Boost.png" caption = "Boost Converter" numbered = "true" >}}

The main circuit is divided into primary circuit and secondary circuit. The input voltage of the system is 24V. The control signal is realized by UC3843. In the primary loop, the voltage boost is realized, and the sampling resistance is set to control the peak current and play the role of current limiting. In the secondary loop, A constant current circuit is set with A constant current of 0.3A.

{{< figure src = "Circuit Design - 1.png" caption = "Flow Diagram" numbered = "true" >}}

The main circuit and control circuit are designed according to the index requirements, parameter calculation and BOOST topology.

{{< figure src = "Circuit Design - 2.png" caption = "Circuit Diagram" numbered = "true" >}}

## **Simulated Analysis**

- Output Current Waveform ( ≈ 300 mA ) 

{{< figure src = "Simulated Analysis - mA1.png" caption = "Output Current Waveform" numbered = "true" >}}

- Output Ripple Current ( ≤ 0.1 % )

{{< figure src = "Simulated Analysis - mA2.png" caption = "Output Ripple Current" numbered = "true" >}}

- Output Voltage Waveform ( ≤ 80 V ) 

{{< figure src = "Simulated Analysis - V1.png" caption = "Output Voltage Waveform" numbered = "true" >}}

- Output Ripple Voltage ( ≤ 0.1 % )

{{< figure src = "Simulated Analysis - V2.png" caption = "Output Ripple Voltage" numbered = "true" >}}

