---
layout: page
title: Chip Design Introduction
excerpt: "Chip Design Introduction"
tags: [OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart, Chip Design]
categories: [Electronics, IC Design]
comments: false
modified: 2016-01-02
image:
  feature: header.jpg
---

 
##An Introduction to designing your own chip

Designing Integrated Circuits (chips) typically is reserved for large companies with engineering
teams that can range from just a few people to over 100. The process includes creating the masks
that are used to create the microscopic patterns on silicon wafers that eventually becomes millions
to billions of transistors. For big/complex chips like processors and FPGAs, the set of masks can
cost 10's of millions of dollars. It only makes sense to head down this path if you expect to be
making hundreds of thousands to millions of the same chip. If your requirement is for smaller
quantities, then ASICs and FPGAs may be the right choice. OSHChip would like to offer another
possible approach, and it isn't even new. It's been done before several times, but as it is not
a high profile approach, you may not have heard of it.

At its most simple description, it is the creation of a chip for a specific function, using a
standard programmable product (microprocessor, FPGA, System on Chip(SoC)) and pre-programming
it with the desired function. While you are limited to the resources that the underlying programmable
product provides, the advance of SoC technology in recent years has lead to products with
capabilities that allow the creation of very sophisticated chips using this technique. The goal
of OSHChip is to provide an ideal platform for you to create your own chips, without having
to spend millions of dollars on manufacturing, or committing to huge volumes of parts.

* No minimum quantity of parts need to be made. Create just 1 instance if you wish
* No external components required. Built in oscillator components, and supporting decoupling
  capacitors, and even 3 indicator LEDs (no other chip on the market has indicator LEDs!)
* Built in 32 bit ARM Cortex-M0 processor, running at 16 MHz
* Ultra low power operation
* Compatible with systems operating from 1.8V to 3.6V
* 2.4 GHz Bluetooth Low Energy radio
* Broad range of built-in Peripheral functions, including 1 or more of the following
  * UART
  * 10-bit ADC
  * Counter/Timers
  * SPI
  * I2C
  * Temp
  * RTC
  * Watchdog Timer
  * Quadrature Decoder
  * AES Encryption
  * Random Number Generator.
  * 3 On-board LEDs (near top connector), Red Green and Blue.
* 256 KBytes of Flash memory for program and data, including data-logging
* 32 KBytes of SRAM
* Packaging that is physically very similar to the standard 16 pin DIP (Dual Inline Pins),
  and it is compatible with standard bread board construction
* Support for in-system debugging including breakpoints
* Re-programmable. If you no longer need an OSHChip to perform the custom chip design
  that you have created, you can just reprogram it with an alternative custom chip design,
  or just use it as a general purpose processor board.
* The hardware design for OSHChip is Open Source (it's in the name **Open&nbsp;Source&nbsp;Hardware&nbsp;Chip**)

The OSHChip web site will guide you through the process with a worked example, and
this site also provides a forum for you to discuss your design with other OSHChip
designers, and best of all, submit your design for inclusion in the parts catalog,
where your chip will be assigned a unique chip part number that others can use in
their designs.

Let's get started: [Planning your Chip](Planning_your_Chip.html)


{% include chipdesign_index.md %}
