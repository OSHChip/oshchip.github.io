---
layout: page
title: Peripheral Pin Assignments for OSHChip
excerpt: "OSHChip Pin Assignments"
tags: [OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart, Pin Assignments]
categories: [Electronics]
comments: false
<<<<<<< HEAD
modified: 2016-03-16
=======
modified: 2016-03-13
>>>>>>> origin/master
image:
  feature: header.jpg
markdown:    kramdown
highlighter: rouge
---

For peripherals that need to have an I/O pin assigned, each pin of
the peripheral will have a **Pin Select** register that allows you
to map the I/O function to **any** of OSHChip's pins.

In most other processors there is a fixed pin assignments, with
each pin shared by multiple peripherals, and your choice of a specific
peripheral blocks the use of the other peripherals that share that pin.
So with OSHChip, the biggest limitation is the number of available I/O
pins (14) rather than the constraints of which peripherals are mutually
exclusive because of shared pin resources. Many peripheral blocks do not need any I/O Pins

#### Peripherals that don't need I/O pins

* 2.4 GHz Radio
* Counter/Timers
* Temp
* RTC
* Watchdog Timer
* AES Encryption
* Random Number Generator
* Memory Protection Unit
* Power Management
* Programmable Peripheral Interconnect  
    (this is connections between peripherals)
* Clock Management

#### Peripherals that need I/O pins

* UART
* 10-bit ADC
* Low Power Comparator
* SPI
* I2C
* Quadrature Decoder
* General Purpose I/O
* GPIO Task Event blocks
* External Interrupt inputs
* 3 On-board LEDs (near top connector), Red Green and Blue.

For the peripherals that need I/O pins, here are the very minimal
constraints on pin assignments:
(The following will be easier to understand if you look at the  
 right side of the <a href="OSHChip_V1.0___Schematic.PDF" target="_blank">Schematic for OSHChip V1.0</a> )


* The 3 LEDs on OSHChip have pre-assigned GPIO bits, but do not  
  use up any of the 14 physical pin resources.
  * **RED** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; P0_8
  * **GREEN** &nbsp;&nbsp;&nbsp; P0_5
  * **BLUE** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; P0_3
* The **ADC** and the **Low Power Comparator (LPCOMP)** share the same I/O  
  pins and are mutually exclusive.  
  If the **32 KHz external crystal** is used, it must be on a specific pair of pins,  
  in which case ADC/LPCOMP can't use inputs AIN0 and AIN1.
  * 32 KHz external crystal, if used must be connected to  
    OSHChip pin 12 and 13
  * If the ADC external reference is used, it must be on OSHChip pin 11
  * ADC/LPCOMP inputs are:
    * AIN0 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; OSHChip pin 13
    * AIN1 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; OSHChip pin 12
    * AIN2 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; OSHChip pin 9
    * AIN3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; OSHChip pin 10
    * AREF0 &nbsp;&nbsp;&nbsp; OSHChip pin 11
  * If AREF0 is not used, OSHChip pin 11 is available for all other peripherals
  * If the ADC/LPCOMP is used, only one of OSHChip pin 9, 10, 12, 13 is  
    connected to the ADC at any given time. The others could be used for  
    other peripherals. For example, if you needed 2 analog inputs, used the  
    internal reference (based on VDD of the OSHChip) and didn't need the  
    32KHz crystal, then you could use AIN0 and AIN1 for the analog inputs  
    (OSHChip pins 12 and 13) and the remaining OSHChip pins 9, 10, and 11  
    are available for all other peripherals.
  * The **General Purpose I/O** (GPIO) port is a special case, in that it  
    is the default if no other peripheral is using a pin. The port bits  
    still require configuration, before use for general I/O.
* All other peripherals can use any OSHChip pin 1 through 7 and 9 through 15  
  except for pins used by ADC/LPCOMP/32KHz crystal, *if* they are used.
* By default, the UART is assigned to OSHChip pins 1 and 2, but you can re-assign  
  the UART to other pins, or disable it and it will then not use any pins.

#### GPIO pin setup and use

This is documented in chapter 14 of the [nRF51 Series Reference Manual](https://www.nordicsemi.com/eng/nordic/download_resource/20337/12/45450728)  
A header file that has all the default pin names is here: [OSHChip_Pin_Names.h](https://github.com/OSHChip/OSHChip_Related_Files/tree/master/Getting_Started_Files)


<!--- 

On my Jekyll inside a VM, the ```c stuff didnt work  --- maybe rouge isn't working correctly
On my Jekyll inside a VM, indenting with 4 spaces does go into 'code' mode, but highlighting did not occur,
   and the line spacing sucks.
On the GitHub repo, ```c  does work, and looking at it in the repo, it highlights and looks great
   but rendered on my site, highlighting only partially works, and line spacing sucks
So I looked at the source for the ```c rendered stuff, viewed in the repo, and cut and pasted it below,
   and commented out the stuff that was used to create it.

End result is it looks ok with regard to line spacing, but no highlighting on my site

```c
#include <stdint.h>
#include "nrf_delay.h"
#include "nrf_gpio.h"
#include "OSHChip_Pin_Names.h"

int main()
{
    nrf_gpio_cfg_output(LED_RED);

    nrf_gpio_pin_set(LED_RED);

    while(1){
        nrf_gpio_pin_toggle(LED_RED);
        nrf_delay_ms(500);
<<<<<<< HEAD
    }
}
```
--->

<div class="highlight highlight-source-c"><pre>#<span class="pl-k">include</span> <span class="pl-s"><span class="pl-pds">&lt;</span>stdint.h<span class="pl-pds">&gt;</span></span>
#<span class="pl-k">include</span> <span class="pl-s"><span class="pl-pds">"</span>nrf_delay.h<span class="pl-pds">"</span></span>
#<span class="pl-k">include</span> <span class="pl-s"><span class="pl-pds">"</span>nrf_gpio.h<span class="pl-pds">"</span></span>
#<span class="pl-k">include</span> <span class="pl-s"><span class="pl-pds">"</span>OSHChip_Pin_Names.h<span class="pl-pds">"</span></span>
=======
    }
}
```
--->

<div class="highlight highlight-source-c"><pre>#<span class="pl-k">include</span> <span class="pl-s"><span class="pl-pds">&lt;</span>stdint.h<span class="pl-pds">&gt;</span></span>
#<span class="pl-k">include</span> <span class="pl-s"><span class="pl-pds">"</span>nrf_delay.h<span class="pl-pds">"</span></span>
#<span class="pl-k">include</span> <span class="pl-s"><span class="pl-pds">"</span>nrf_gpio.h<span class="pl-pds">"</span></span>
#<span class="pl-k">include</span> <span class="pl-s"><span class="pl-pds">"</span>OSHChip_Pin_Names.h<span class="pl-pds">"</span></span>

<span class="pl-k">int</span> <span class="pl-en">main</span>()
{
    <span class="pl-c1">nrf_gpio_cfg_output</span>(LED_RED);

    <span class="pl-c1">nrf_gpio_pin_set</span>(LED_RED);

    <span class="pl-k">while</span>(<span class="pl-c1">1</span>){
        <span class="pl-c1">nrf_gpio_pin_toggle</span>(LED_RED);
        <span class="pl-c1">nrf_delay_ms</span>(<span class="pl-c1">500</span>);
    }
}</pre></div>
>>>>>>> origin/master

<span class="pl-k">int</span> <span class="pl-en">main</span>()
{
    <span class="pl-c1">nrf_gpio_cfg_output</span>(LED_RED);

<<<<<<< HEAD
    <span class="pl-c1">nrf_gpio_pin_set</span>(LED_RED);

    <span class="pl-k">while</span>(<span class="pl-c1">1</span>){
        <span class="pl-c1">nrf_gpio_pin_toggle</span>(LED_RED);
        <span class="pl-c1">nrf_delay_ms</span>(<span class="pl-c1">500</span>);
    }
}</pre></div>



=======
>>>>>>> origin/master
--- detailed explanation still to be written ---


#### Pin Select Registers

Each peripheral that needs I/O pins has a **Pin Select Register** for each I/O pin
that it needs. Setting the pin select register to the bit position in the P0 Port
that connects to the OSHChip pin you want to use, makes the connection between
the peripheral and physical pin.



#### Let's look at some examples.

--- more stuff goes here
<<<<<<< HEAD

=======
>>>>>>> origin/master



