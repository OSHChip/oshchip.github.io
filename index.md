---
layout: home_no_recents
excerpt: "OSHChip home on the WWW"
tags: [OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart]
categories: [Electronics]
comments: false
modified: 2015-12-29
image:
  feature: header.jpg
---

OSHChip:&emsp;One product, Two views
================================

### OSHChip as a general purpose processor board

<br>
**View 1:  OSHChip_V1.0 is a unique combination of**

* ARM Cortex-M0 32 bit processor running at 16 MHz
* 2.4 GHz Bluetooth Low Energy radio
* Broad range of built-in Peripheral functions
* 256 KBytes of Flash memory for program and data
*  32 KBytes of SRAM
* Minature packaging, compatible with bread board construction
* Support for in-system debugging including breakpoints

The most striking thing you see is that it is the size of a 16 pin
DIP, and unlike other processor boards, it is designed from the start
to be compatible with the white breadboards that are commonly used by
electronic hobbyists, robotics projects, and oh so many hackaday
projects. The pins are directly designed to work with these bread
boards, and unlike the usual pin strips found on other processor
boards, they plug in easily to the bread board, and don't damage it.
Unlike other processor boards that are far larger, OSHChip can be
plugged into the middle two rows of a bread board, and it doesn't
cover the connected holes that you will be connecting to.

Take me to the [OSHChip Product Page](products/OSHChip_V1.0_Product.html)


### OSHChip as a platform for designing custom chips

<br>
**View 2:  You get to be a chip designer.**

Imagine you wanted to design a chip. Nothing too fancy, but let's
including some general purpose digital inputs and outputs, some analog
inputs, some counters, timers, or PWM, maybe able to talk to another
chip over SPI or I2C, some storage for calibration constants, maybe a
linearization table, and an on-board processor that can be programmed
in C. While we are dreaming, lets also include a low power mode that
only draws a microamp or two, can communicate with a UART to a
terminal program on your computer, and lets add in a 2.4 GHz radio
that can operate with the Bluetooth Low Energy protocol to smart
phones, like Android phones and iDevices.

[Chip Design with OSHChip](chipdesign/index.html)
