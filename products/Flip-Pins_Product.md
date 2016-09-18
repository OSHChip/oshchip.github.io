---
layout: page
title: Flip-Pins
excerpt: "Flip-Pins Description"
tags: [Flip-Pins, OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart]
categories: [Electronics]
comments: false
modified: 2016-09-12
image:
  feature: header.jpg
---

### IC pins for your own projects.

<html>
<p style="float: left; font-size: 12pt; text-align: center; width: 45%; margin-right: 1%; margin-bottom: 0.5em;">
   <A HREF="/images/Flip-Pins-08_w1200.jpg" target="_blank"><img src="/images/Flip-Pins-08_small.jpg" style="width: 100%"></A>Flip-Pins-08</p>
<p style="float: left; font-size: 12pt; text-align: center; width: 45%; margin-right: 1%; margin-bottom: 0.5em;">
   <A HREF="/images/OSHChip_on_1_cent_coin_w1200.jpg" target="_blank"><img src="/images/OSHChip_on_1_cent_coin_small.jpg" style="width: 100%"></A>OSHChip</p>
<div style="clear:both;"></div>
<div style="text-align:center"> <i> Click on pictures for a larger image </i> </div>
<div style="text-align:center"> <i> Photo Credit: Windell Oskay </i> </div>
</html>
 
## Description

Flip-Pins are the third generation of the Integrated Circuit (IC)
pins designed by Fliptronics for use in products like OSHChip. The
goal for Flip-Pins was to create pins that could be soldered into
a Printed Circuit Board (PCB) and to look as much like an IC pin
as possible. _(Current production OSHChips use the second generation
pins, and will change over to third generation with the next
production run.)_ With the unique plastic aligner, the pins are held 0.100"
apart, with a 0.062" solder tail exposed.

A significant feature of Flip-Pins is that their width (0.020") is the
same as traditional Dual-Inline-Package (DIP) IC pins, and so Flip-Pins
are directly compatible with standard Breadboards. Many people use
header pins which are square to connect their PCBs to breadboards,
and are unaware that header pins damage the breadboard because they are
wider than standard DIP pins. PCBs that use Flip-Pins are easier to
insert and remove from breadboards, compared to PCBs with header pins.

Flip-Pin are available in 3 lengths: 8, 14, and 20 pins. Other
lengths can be achieved by either using multiple strips, or removing
pins from a strip.

## How Flip-Pins are used

When soldered into PCBs that are commonly 0.062" thick, a near flush
surface can be achieved on the non-pin side of the PCB (see the OSHChip
on a penny picture, above). After soldering the pins into your PCB, the
plastic aligner can be easily removed and discarded.

[Detailed description of how to solder Flip-Pins](/products/Soldering_Flip-Pins.html)

The recommended footprint on your PCB for Flip-Pins is shown in the
datasheet. Briefly, the holes should be 0.025" in diameter, and the
associated pads should be at least 0.040" in diameter. On the top side
of your PCB (the side that does not have the pins) you can place
components and vias close to the pads. On the bottom of the PCB, you
must leave clearance for the plastic aligner. For the narrow dimension,
the clearance should be 0.120" centered on the center line of the row of
pins. For the length, the clearance area should be 0.100" times the
number of pins +0.040". For example, for the 14 pin version of Flip-
Pins, the clearance area is 0.120" x 1.440".

## Libraries

For your convenience, PCB CAD libraries have already been created
for the following CAD systems:

* [Altium](/products/Flip-Pins_Altium.html){:target="_blank"}
* [Kicad](/products/Flip-Pins_Kicad.html){:target="_blank"}
* [Eagle](/products/Flip-Pins_Eagle.html){:target="_blank"}

## Documents

* [Datasheet Flip-Pins-XX_REV_A.pdf](/docs/Flip-Pins-XX_REV_A.pdf){:target="_blank"}
* [Step model for a single pin](/docs/Flip-Pins_one_pin.step){:target="_blank"}
* [Step model for a single pin with aligner](/docs/Flip-Pins_one_pin_with_aligner.step){:target="_blank"}

## Compatibility

Examples of breadboards that Flip-Pins were designed for:

* [EMSL 170 point Breadboard](http://shop.evilmadscientist.com/productsmenu/partsmenu/439){:target="_blank"}
* [EMSL 630 Point Transparent Breadboard](http://shop.evilmadscientist.com/productsmenu/partsmenu/623){:target="_blank"}
* [DigiKey 170 point Breadboard](http://www.digikey.com/product-detail/en/parallax-inc/700-00012/700-00012-ND){:target="_blank"}
* [DigiKey 830 point Breadboard](http://www.digikey.com/product-detail/en/twin-industries/TW-E40-1020/438-1045-ND){:target="_blank"}
* [Sparkfun 170 point Breadboard](https://www.sparkfun.com/products/12043){:target="_blank"}
* [Sparkfun 830 point Breadboard](https://www.sparkfun.com/products/12615){:target="_blank"}
* [Adafruit 170 point Breadboard](https://www.adafruit.com/products/65){:target="_blank"}
* [Adafruit 830 point Breadboard](https://www.adafruit.com/products/239){:target="_blank"}

Flip-Pins are compatible with IC sockets that have flat contacts, for example:

* [EMSL 16 pin DIP sockets](http://shop.evilmadscientist.com/partsmenu/494){:target="_blank"}
* [Digikey 16 pin DIP sockets](http://www.digikey.com/product-detail/en/on-shore-technology-inc/ED16DT/ED3046-5-ND){:target="_blank"}
* [Sparkfun 16 pin DIP sockets](https://www.sparkfun.com/products/7938){:target="_blank"}
* [Adafruit 16 pin DIP sockets](https://www.adafruit.com/products/2203){:target="_blank"}

Flip-Pins might not be compatible with IC sockets that have a round entry hole
for the IC pin. Please check carefully with an actual socket. For example, these types
of sockets: [DigiKey ED3016-ND](http://www.digikey.com/product-detail/en/on-shore-technology-inc/SA163000/ED3016-ND){:target="_blank"}

Examples of Boards that can be used with Flip-Pins

* Printed Circuit Board you design yourself, maybe etching them yourself, or
  milling, or having them manufactured by a company like [OSHPark](https://www.oshpark.com/){:target="_blank"}
* [EMSL breakout boards](http://shop.evilmadscientist.com/search-main?q=breakout){:target="_blank"}
* [Sparkfun breakout boards](https://www.sparkfun.com/categories/20){:target="_blank"}
* [Adafruit breakout boards](https://www.adafruit.com/categories/42){:target="_blank"}

## Buying Flip-Pins

Flip-Pins are available in 3 different lengths: 8, 14, and 20 pins.

The following are authorized distributors for Flip-Pins:

* At the [OSHChip store on Tindie](https://www.tindie.com/stores/OSHChip/){:target="_blank"}
* [Evil Mad Scientist LLC](http://shop.evilmadscientist.com/directory){:target="_blank"}
* Distributor A (not yet setup)
* Distributor D (not yet setup)
* Distributor S (not yet setup)
