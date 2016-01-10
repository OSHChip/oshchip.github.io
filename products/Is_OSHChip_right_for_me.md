---
layout: page
title: Is OSHChip right for me
excerpt: "Selection Features"
tags: [OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart]
categories: [Electronics]
comments: false
modified: 2016-01-10
image:
  feature: header.jpg
---

There are so many processor boards and modules available, trying to decide
what is the right one for your project can be a real challenge. This page
will try and help you in your consideration of OSHChip.

####History of OSHChip

TLDR; Build a product that is like a 16 pin DIP with amazing capabilities.

Some insights into the conception, design, and trade-offs made in creating
OSHChip may be of help. While not common for a technical site, I'm going
to slip into first person for most of what follows since the reality is
that OSHChip is the work of one person.

My original plan was to create a platform specifically to support the
creation of custom chips within the constraints of the programmable
resources I built into the product. This is the "View 2" described on
the home page. My goal is to motivate electronic hobbyists who are
unlikely to ever have the opportunity to actually design and
manufacture a custom chip to experience most of the challenges and
rewards of the process, without the costs.

I had already spent about 2 years working with the Nordic
Semiconductors nRF51822 System On Chip (SOC) and considered it an
extremely good value for the price. Even without the 2.4 GHz radio,
the rest of the device is very competitive with microprocessors from
other companies. The biggest challenge for hobbyists though, is that
the nRF51822 is only available in QFN and BGA packages, which means a
hobbyist would need to design and manufacture a PCB before they could
use the nRF51822. And even after creating the PCB, there is the quite
significant challenge of soldering a fine pitch QFN device, or the even
harder fine pitch BGA. While there are multiple manufacturers of
modules that include this part, all the modules are surface mount, so
the end user still has to create a PCB. There are also other
challenges that hobbyists may not be up to, such as fine line PCB
design, and design techniques for 2.4 GHz antennae. OSHChip solves
these problems by dealing with the micro BGA package, antenna, power
supply decoupling, crystal frequency reference, and bring it out in a
package that is ready to be used in a standard solderless bread board.

I wanted to do as much as possible (within my cost constraints) to
create something as much like a standard chip as possible. This lead
to the 16 pin DIP form factor, and the custom pins that no other
processor board has (well the closest is the Basic Stamp products from
Parallax, but their pins are not as pretty as mine).

###Pros and Cons of OSHChip
 
There are good and bad points about any processor board product, here
are what I consider the main Pros and Cons for OSHChip.

####Pros

- Very small size
- 16 pin format with unique IC type pins, well matched to standard solderless bread boards
- Rapid prototyping with bread boards
- Very low power modes
- Fully functional from 1.8V to 3.6V
- 32 bit CPU, 256KB of Flash, 32KB of RAM
- Higher performance and more Flash and RAM than many models of Arduios
- Bluetooth Low Energy radio
- Proprietary 2.4 GHz radio for chip-to-chip communications
- Broad range of built in peripherals, similar to most other micro processor products
- Except for ADC inputs, any peripheral function can be routed to any of the 14 I/O pins
- Efficient peripheral to peripheral Event/Task system that does not require CPU intervention
- Built in Red, Green, and Blue LEDs, that don't use any of the user's 14 I/O pins
- Extensive debug support
- Drag and drop programming.
- Existing support community at Nordic's web site
- Existing support community within the mbed environment
- Multiple compiler/IDE options already exist
- Open source hardware design, all files are on GitHub
- All software from OSHChip is Open Source, most of the software from Nordic is available in source form, except for the radio protocol stacks
- Looks cute
 
####Cons

- Only 14 I/O pins
- I/O is not 5V compliant
- I/O pins are only designed to drive CMOS type loads (mostly)





