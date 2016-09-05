---
layout: page
title: Flip-Pins
excerpt: "Flip-Pins Description"
tags: [Flip-Pins, OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart]
categories: [Electronics]
comments: false
modified: 2016-09-05
image:
  feature: header.jpg
---

<html>
<p style="float: left; font-size: 10pt; text-align: center; width: 45%; margin-right: 1%; margin-bottom: 0.5em;"><img src="/images/Flip-Pins-08_small.jpg" style="width: 100%">Flip-Pins-08</p>
<p style="float: left; font-size: 10pt; text-align: center; width: 45%; margin-right: 1%; margin-bottom: 0.5em;"><img src="/images/OSHChip_on_1_cent_coin_small.jpg" style="width: 100%">OSHChip</p>
</html>

 
## Description

Flip-Pins are the third generation of the Integrated Circuit (IC)
pins designed by Fliptronics for use in products like OSHChip. The
goal for Flip-Pins was to create pins that could be soldered into
a Printed Circuit Board (PCB) and to look as much like an IC pin
as possible. _(Current production OSHChips use the second generation
pins, and will change over to third generation with the next
production run.)_ With the plastic aligner, the pins are held 0.1"
apart, with a .062" solder tail exposed.

A significant feature of Flip-Pins is that their width (.020") is the
same as traditional Dual-Inline-Package (DIP) IC pins, and so Flip-Pins
are directly compatible with standard Breadboards. Many people use
header pins which are .025" square to connect their PCBs to breadboards,
and are unaware that header pins damage the breadboard because they are
wider than standard DIP pins.

Flip-Pin are available in 3 lengths: 8, 14, and 20 pins. Other
lengths can be achieved by either using multiple strips, or removing
pins from a strip.

## How they are used (quick version)

When soldered into PCBs that are commonly .062" thick, a near flush
surface can be achieved on the non-pin side of the PCB (see pictures
below). After soldering the pins into your PCB, the plastic aligner
can be easily removed and discarded.

## Compatibility

Examples of breadboards that Flip-Pins were designed for:

<html>
<a href="http://shop.evilmadscientist.com/productsmenu/partsmenu/439" target="_blank">EMSL Mini Breadboard</a>
<br>
<a href="http://shop.evilmadscientist.com/productsmenu/partsmenu/623" target="_blank">EMSL 630-Point Transparent Breadboard</a>
<br>
<a href="http://www.digikey.com/product-detail/en/twin-industries/TW-E40-1020/438-1045-ND" target="_blank">DigiKey 830 point Breadboard</a>
<br>
</html>


Flip-Pins are compatible with IC sockets that have flat contacts, for example
<html>
<a href="http://shop.evilmadscientist.com/partsmenu/494" target="_blank">EMSL 16 pin DIP sockets</a>
<br>
<a href="http://www.digikey.com/product-search/en?keywords=ED3046-5-ND" target="_blank">DigiKey ED3046-5-ND</a>
<br>
</html>



Examples of Boards that can be used with Flip-Pins

* Printed Circuit Board you design yourself, maybe manufactured by [OSHPark](https://www.oshpark.com/){:target="_blank"}
* [DigiKey breakout boards](https://www.sparkfun.com/categories/20){:target="_blank"}


* ARM Cortex-M0 32 bit micro processor running at 16 MHz
* 256KB Flash Memory
* 32KB SRAM
* 2.4 GHz Radio supports 3 protocols:
  * Bluetooth Low Energy (BLE) / Bluetooth Smart
    * Supports communications from OSHChip  
      to smart phones that support BLE
  * Gazell
    * Supports Chip to Chip communications.
  * ESB (Enhanced Shock Burst)
    * Supports Chip to Chip communications.
* Built-in antenna, range is 10 to 20 feet, depending  
  on environment (metal, desks, chairs, ...)
* Runs from 1.8V to 3.6V .  Multiple low power modes
* 14 general purpose I/O pins. All peripherals (except  
  the ADC) can use any I/O pin
* UART
* 10-bit ADC
* Low Power Comparator
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

## Buying OSHChip

* OSHChip products are sold in our store that is hosted on <a href="https://www.tindie.com/products/OSHChip/oshchip-v10/" target="_blank">Tindie</a>
* The price of OSHChip_V1.0 is $25.00
* Shipping is fixed price regardless of how many you order.

## Related Information

* [Is OSHChip right for me](/docs/Is_OSHChip_right_for_me.html)
* [Connecting OSHChip to the programmer/debugger](/docs/OSHChip_Connections.html)

## Resources

* Very quick start, a  
  [Blinky program using the online mbed environment](/docs/mbed_Blinky.html)
* Getting started with [GCC and Yotta](https://github.com/OSHChip/target-OSHChip-gcc)
* Nordic Semiconductor's [Getting Started Guide](http://infocenter.nordicsemi.com/topic/com.nordic.infocenter.sdk5.v11.0.0/nrf51_getting_started.html?cp=4_0_0_1)  
  (assumes Nordic's development board, and J-Link programmer)
* [Nordic Semiconductor's Documentation library](http://infocenter.nordicsemi.com/index.jsp)
* [Nordic Semiconductor's Development Libraries (SDK)](http://developer.nordicsemi.com)
* [Nordic Semiconductor's Developer Zone (User Forum)](https://devzone.nordicsemi.com/questions/)
* [Setting up development with GCC on Mac OS X](https://devzone.nordicsemi.com/blogs/22/getting-started-with-nrf51-development-on-mac-os-x/)
* These links are to pages currently being developed
  * [Getting started with OSHChip](/docs/Getting_started_with_OSHChip.html)
* These links are place holders
  * [Setting up development with Keil](Sorry_not_yet_written.html)
  * [Setting up development with GCC and Ubuntu](Sorry_not_yet_written.html)
  * [Setting up development with mbed](Sorry_not_yet_written.html)
  * [Setting up development with GCC and Windows 7](Sorry_not_yet_written.html)
  * [Setting up development with Arduino](Sorry_not_yet_written.html)

At the heart of OSHChip_V1.0 is a System-On-Chip (SOC) manufactured by
[Nordic&nbsp;Semiconductors](https://www.nordicsemi.com/). The specific
product is the
[nRF51822](https://www.nordicsemi.com/eng/Products/Bluetooth-Smart-
Bluetooth-low-energy/nRF51822)

To use OSHChip_V1.0 you will need to become familiar with the
documentation provided by Nordic Semiconductor. Because navigating
their site can be challenging, start at
[nRF51822](https://www.nordicsemi.com/eng/Products/Bluetooth-Smart-
Bluetooth-low-energy/nRF51822) and underneath the product title, there
are a set of tabs, starting with "OVERVIEW" and ending with
"DOWNLOADS".  Select the DOWNLOADS tab.

Nordic Semiconductor has split the main documentaion for the nRF51822
into two documents.

* In the **Product Specification** it list the specific recources
included in the device (for example, how many counter-timer blocks are
included) and the timing and power consumption details for all the
functional blocks. The **Product Specification** does not include the
detailed programming information for each functional block.

* In the **nRF51 Series Reference Manual** which does give the detailed
programming information as well as detailed functional operation. It
does not reference a specific product.


The reason for the documentation split is that Nordic has another SOC
(nRF51422) that has its own product specification, but shares the non-
product specific **nRF51 Series Reference Manual**. Even with this
split of documentation, there are several variant of the nRF51822,
which differ in the amount of Flash memory and SRAM. OSHChip_V1.0 uses
the most advanced variant of the nRF51822, which includes 256 KBytes
of Flash and 32 KBytes of SRAM. The specific variant is nRF51822-
CFAC-A0.

For each document, the most recent version is listed, and when
you select it, the page that is presented gives a link for the
most recent document, and all the previous versions.
OSHChip_V1.0 uses the nRF51822 described by:

|**Document**|**Version**|
|:-----------|----------:|
|[nRF51822 Product Specification](https://www.nordicsemi.com/eng/nordic/download_resource/20339/13/41227812) | version 3.1 |
|[nRF51 Series Reference Manual](https://www.nordicsemi.com/eng/nordic/download_resource/20337/12/45450728) | version 3.0 |

## Open Source

OSHChip_V1.0 is an Open Source Hardware design. It's right there
in the name. You can find all the schematics, bill of materials,
printed circuit board design files and the resultant Gerber files
here: [https://github.com/OSHChip/OSHChip_V1.0_Docs](https://github.com/OSHChip/OSHChip_V1.0_Docs)

#### Navigating the GitHub repository for OSHChip V1.0

The repository contains the design files for OSHChip V1.0

The PCB design files are in the directory *Design_Files* and were
created with Altium Designer Release 10

Since you may not have access to Altium Designer, I have also
included all the Gerber files and the Excelon drill file in the
directory *Gerbers_and_Drill_Files*.

In the *Other_Files* directory, you will find the following:

* OSHChip_V1.0___Schematic.PDF
* OSHChip_V1.0___PCB_Prints.PDF
* OSHChip_V1.0___Assembly_Drawings.PDF
* OSHChip_V1.0___Bill_of_Materials.xls
* OSHChip_V1.0___Bill_of_Materials.PDF

## Gallery
<html>
<center><img src="/images/First_OSHChip_V1.0_Array_Width_600.jpg" alt="OSHChip" width="600"></center>
<center><b>OSHChip_V1.0 is manufactured in a panelized form</b></center>
</html>
