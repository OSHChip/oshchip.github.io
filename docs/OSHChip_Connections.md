---
layout: page
title: OSHChip Connections
excerpt: "Connecting CMSIS-DAP to OSHChip"
tags: [OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart]
categories: [Electronics]
comments: false
modified: 2016-01-26
image:
  feature: header.jpg
---

For programming and debugging of OSHChips, a standard SWD cable connects
the programmer/debugger to the connector on the top of the OSHChip.

The cable is a 10 wire ribbon cable, with a 0.050" pitch 2&nbsp;by&nbsp;5 pin
female keyed IDC connector at each end. The cable is typically 4 to 6 inches
long and has a red stripe on the wire that carries the signal between pin 1 of
each connector.

![SWD Ribbon Cable](/images/Labeled_Cable.png)

If you already have an SWD programmer from another vendor, provided
you also have a programming cable with the 0.050" pitch
2&nbsp;by&nbsp;5 IDC connector on the end, you can get by without the
adapter. See below for details.

The alignment key on the programming cable at the programmer end (right
end in the picture above) must match the alignment mark on the printed
circuit board. See the following picture.

<center>
<img src="/images/OSHChip_CMSIS_DAP_J2.jpg" width="500"><br>
</center>

Looking at the connector from above, with the alignment key on the
left side, the pins are numbered:

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;width:45px}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:2px 2px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;text-align:right}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
.tg .tg-yw4l{vertical-align:top}
</style>
<table class="tg">
  <tr>
    <td class="tg-031e">1</td>
    <td class="tg-031e">2</td>
  </tr>
  <tr>
    <td class="tg-031e">3</td>
    <td class="tg-031e">4</td>
  </tr>
  <tr>
    <td class="tg-yw4l">5</td>
    <td class="tg-yw4l">6</td>
  </tr>
  <tr>
    <td class="tg-yw4l">7</td>
    <td class="tg-yw4l">8</td>
  </tr>
  <tr>
    <td class="tg-yw4l">9</td>
    <td class="tg-yw4l">10</td>
  </tr>
</table>

The required signals are on pins 1, 2, 3, and 4, which are in
a 2&nbsp;by&nbsp;2 group at the red stripe end of the connector.
This matches the 2&nbsp;by&nbsp;2 connector on the top of OSHChip.

ARM documents both old and new programming/debugging connectors
in this documnet [cortex_debug_connectors.pdf](http://infocenter.arm.com/help/topic/com.arm.doc.faqs/attached/13634/cortex_debug_connectors.pdf)&nbsp;&nbsp;.&nbsp;
The OSHChip_CMSIS_DAP V1.0 Programmer/Debugger connector is shown
on the top of the second page of that document, with the only
signals implemented being pins 1 through 4.

##Serial Connector J5

See [Connecting and using the serial data interface](OSHChip_CMSIS_DAP_V1.0_Serial_Data_Interface.html)

##Programming voltages and Connector J1

OSHChip V1.0 can operate from 1.8 V to 3.6V . Typically 3.3V is used,
and 3.3V to 3.6V is a requirement if the on-board LEDs are used.

The OSHChip_CMSIS_DAP V1.0 Programmer/Debugger is powered by the USB
cable, and has an internal regulator for 3.3V .

####If OSHChip is powered from 2.5V to 3.6V but not 3.3V

* OSHChip can be left connected to the rest of the target system
* J1 must **not** have the jumper installed, because the target system
  and the programmer power supplies are at different voltages
* Both programming and debugging can be performed

####If OSHChip is powered at 3.3V

* OSHChip can be left connected to the rest of the target system
* J1 may have the jumper installed, but it is not necessary
* Both programming and debugging can be performed

####If OSHChip is powered from 1.8V to 2.4V

* OSHChip must be unplugged from the target system **before**
  connecting the programming cable for programming
* J1 **must** have the jumper installed (this powers OSHChip when
  it is not plugged into the target system)
* Programming can be performed
* Debugging can only be done if the program being debugged can operate
  without OSHChip being connected to the rest of the target system
* After programming is finished, the programming cable **must** be
  disconnected first from OSHChip, and then OSHChip can be plugged
  back into the target system. **Do not** plug it back into the
  target system with the programming cable and programmer still
  attached

<center>
<img src="/images/OSHChip_CMSIS_DAP_J1.jpg" width="400"><br>
</center>

##SWD Programmer/Debuggers from other suppliers

Example SWD programmers include:

* OSHChip_CMSIS_DAP V1.0
* Segger J-Link
* Segger J-Link Lite
* Keil ULink
* Nordic Semiconductor nRF51-DK

The following have not been tested, but may work using the Keil IDE

* CooCox CoLinkEx
* PEmicro Multilink

If you do not already have a programmer, when ordering OSHChips you
should also order an OSHChip_CMSIS_DAP V1.0  It comes with a programming
cable and an adapter that converts from the 2&nbsp;by&nbsp;5 pin
IDC connector on the end of the cable to a 2&nbsp;by&nbsp;2 conector
that mates with the connector on the top of OSHChip.

<center>
<img src="/images/SWD_2x5_to_2x2_Adapter.png" width="400"><br>
<b>SWD 2x5 to 2x2 Adapter</b>
</center>

<br>
<br>
<br>

##Programming/Debugging cable orientation

###With the adapter

<center>
<img src="/images/Cable_Adapter_and_OSHChip.jpg" width="400"><br>
<b>Programming cable, adapter, and OSHChip</b>
</center>
<br>
<br>
<center>
<img src="/images/OSHChip_adapter_DAP.jpg" width="600"><br>
<b>OSHChip, Adapter, Cable, and OSHChip_CMSIS_Dap</b>
</center>

###Without the adapter

OSHChip can be programmed with SWD programmers from other suppliers,
listed above. Provided they have a programming cable with the
2&nbsp;by&nbsp;5 pin IDC connector on the end, with 0.05" pitch, they
can be used to program and debug OSHChip. (the other common ARM debugger
cables have a 2&nbsp;by&nbsp;10 pin IDC connector on the end, with 0.1"
pitch, which cannot be used without a suitable conversion from 0.1" to
0.05" pitch)

To connect the SWD programmer to OSHChip without the adapter, the IDC
connector must be carefully positioned so that the 4 pins on the top of
OSHChip fit into the 2&nbsp;by&nbsp;2 pins at the red stripe end of the
connector at the end of the cable. The cable orientation is the same as
that used when the adapter is available. When attaching the cable to
OSHChip, just be very careful that the 4 pins from OSHChip go into the 4
holes in the connector that are closest to the red stripe on the cable.

 See the picture below.

<center>
<img src="/images/OSHChip_connected_without_adapter.jpg" width="300"><br>
<b>Programming cable and OSHChip</b>
</center>
