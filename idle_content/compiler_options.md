---
layout: page
title: OSHChip V1.0
excerpt: "Compiler Options"
tags: [OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart, Keil, ARM, GCC, Debug, IAR]
categories: [Compileres]
comments: true
modified: 2015-11-11
thumbnail: images/20-15/10/oshchip.jpg
image:
  feature: header.jpg
---

![OSHChip](/images/2015/11/OSHChip_Black_on_breadboard_4.JPG "OSHChip")


#C/C++ Compilers

OSHChip_V1.0 has an ARM Cortex-M0 processor, 256 KBytes of flash
memory for program storage, 32 KBytes of SRAM for data storage, and a
wide range of peripheral blocks. Programs for OSHChip_V1.0 can be
written in any programming language for which you have a compiler, or
even assembler can be used. Predominantly, C or C++ is used, and there
are several compilers to choose between. This page will help you
decide which one is best for your situation.

*   Compiler overview
    *   Top level synopsys
    *   Important factors

*   Keil
    *   Capabilities and Limitations
    *   Running on Windows
    *   Running on Mac or Linux
    *   Debugging
*   mbed
    *   Capabilities and Limitations
    *   Run anywhere
    *   Debugging
    *   Libraries
    *   Community
*   GCC
    *   Capabilities and Limitations
    *   Running on Windows
    *   Running on Mac or Linux
    *   Debugging
*   Arduino
    *   Capabilities and Limitations
    *   Running on Windows
    *   Running on Mac or Linux
    *   Debugging



*   [Overview](#overview)
    *   [Philosophy](#philosophy)
    *   [Inline HTML](#html)
    *   [Automatic Escaping for Special Characters](#autoescape)
*   [Block Elements](#block)























OSHChip V1.0 includes the following functional blocks
* ARM Cortex-M0 32 bit micro processor running at 16 MHz
* 256KB Flash Memory
* 32KB SRAM
* 2.4 GHz Radio supports 4 protocols:
    * Bluetooth Low Energy (BLE) / Bluetooth Smart
      - Supports communications from OSHChip to smart phones that support BLE
    * ANT
    * Proprietary Gazell
    * Proprietary ESB
      - Supports Chip to Chip communications.
* Built-in antenna, range is 10 to 20 feet, depending on environment (metal, desks, chairs, ...)
* Runs from 1.8V to 3.6V .  Multiple low power modes
* 14 general purpose I/O pins. All peripherals (except ADC) can use any I/O pin
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


