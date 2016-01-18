---
layout: page
title: OSHChip_CMSIS_DAP_V1.0 Serial Data interface
excerpt: "Product Description"
tags: [SWD, Debug, OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart]
categories: [Electronics, Programming, Debugging]
comments: false
modified: 2016-01-17
image:
  feature: header.jpg
---
![OSHChip](/images/OSHChip_CMSIS_DAP_J5.jpg "OSHChip_CMSIS_DAP Serial Data Interface")

OSHChip_CMSIS_DAP_V1.0 has a 2 pin connector labeled J5 for serial data.
It is located in the corner. The pin closest to the corner is labeled
**RX&nbsp;In** and it is an input to OSHChip_CMSIS_DAP_V1.0, typically
used to transfer information from printf() calls in your program running
on OSHChip to your computer. To use this you must have a wire connecting
this pin to the pin on OSHChip that the on-board UART TXD signal is
connected to. By default, if the UART is enabled, TXD is routed to pin 1
of OSHChip.

The second pin of J5 is is labeled **TX&nbsp;Out** and it is an output
from OSHChip_CMSIS_DAP_V1.0, typically used to send serial data to
OSHChip. C&nbsp;functions such as getc(), gets(), and scanf() can
receive this serial data. To use this you must have a wire connecting
this pin to the pin on OSHChip that the on-board UART RXD signal is
connected to. By default, if the UART is enabled, RXD is routed to pin 2
of OSHChip.

Both the serial transmitted and received data go to your computer via
the USB cable, and appear as a COM port on your computer. On your
computer you can either write a program to communicate with the COM
port, or use a terminal program (there are many to choose from). The
default serial protocol is 9600-N81 , and the signals switch between 0V
and 3.3V. These levels are not RS232 compatible, but they are compatible
with OSHChip when it is powered at a voltage close to 3.3V.
OSHChip_CMSIS_DAP_V1.0 is shipped with a jumper linking **TX&nbsp;Out**
to **RX&nbsp;In** . This provides a loopback capability, which you can
use to check that your program running on the computer is set up
correctly.

Reliable serial communications require that the grounds of both OSHChip
and OSHChip_CMSIS_DAP_V1.0 are connected together. If the SWD cable is
connected to both OSHChip_CMSIS_DAP_V1.0 and OSHChip, this provides a
ground connection.
