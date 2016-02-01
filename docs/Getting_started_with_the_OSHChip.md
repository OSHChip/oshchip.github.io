---
layout: page
title: Getting started with the OSHChip V1.0
excerpt: "Getting started with the OSHChip"
tags: [OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart]
categories: [Electronics]
comments: false
modified: 2016-01-31
image:
  feature: header.jpg
---


##Choosing an Environment for software development

The OSHChip processor 16 pin Dual Inline Package (DIP) contains a Nordic
Semiconductors nRF51822 System On Chip (SoC). There are several versions
of this device, and OSHChip uses the most advanced one, that includes
256 KBytes of Flash memory and 32 KBytes of Static Random Access Memory (SRAM).

Programming support initially is focussed on C and C++, with other languages
at a later date.

There are several different C compiler environments available for OSHChip,
each with various pros and cons.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
.tg .tg-y9fb{font-size:18px;font-family:"Times New Roman", Times, serif !important;;vertical-align:top}
.tg .tg-wvtc{font-size:18px;font-family:"Times New Roman", Times, serif !important;}
</style>
<table class="tg">
  <tr>
    <th class="tg-wvtc">Compiler</th>
    <th class="tg-wvtc">Pros</th>
    <th class="tg-wvtc">Cons</th>
  </tr>
  <tr>
    <td class="tg-wvtc">Keil</td>
    <td class="tg-y9fb">The primary compiler that Nordic uses for their development and examples<br>Excellent debug support<br>Probably the most nRF51822 users<br>Free evaluation version, most applications work within the restrictions</td>
    <td class="tg-y9fb">Evaluation version is limited to 32 KBytes of generated code<br>Unlimited version is fairly expensive<br>Only available for Windows</td>
  </tr>
  <tr>
    <td class="tg-wvtc">mbed</td>
    <td class="tg-y9fb">No restrictions<br>Extensive libraries<br>Nordic Semiconductor SDK libraries already available<br>Large user community sharing projects<br>Online compiler, runs inside browser, independent of host OS<br>No software to install<br></td>
    <td class="tg-y9fb">No debugger<br>No control of compiler options</td>
  </tr>
  <tr>
    <td class="tg-wvtc">GCC</td>
    <td class="tg-wvtc">Nordic Semiconductor SDK includes support for GCC<br>Text based debugger GDB available</td>
    <td class="tg-y9fb">Complex software install<br>Graphical debugger Eclipse is considered difficult to use<br>   by some people</td>
  </tr>
  <tr>
    <td class="tg-wvtc">Arduino</td>
    <td class="tg-wvtc">Broad use by hobbyist community<br>Other nRF51822 products already supported</td>
    <td class="tg-y9fb">No Debugger<br>Support for OSHChip V1.0 planned but not yet available</td>
  </tr>
  <tr>
    <td class="tg-wvtc">IAR</td>
    <td class="tg-wvtc">Nordic Semiconductor SDK includes support for IAR<br>Built in debugger.</td>
    <td class="tg-y9fb">Unknown support for OSHChip_CMSIS_DAP debugging</td>
  </tr>
  <tr>
    <td class="tg-y9fb">Imagecraft</td>
    <td class="tg-y9fb">Commercial version much less expensive than Keil<br>Eval version is fully functional for 45 days, then restricted to<br>   10 KBytes of generated code for non-commercial use.</td>
    <td class="tg-y9fb">Unknown support for nRF51822 processor and SDK<br>Unknown support for OSHChip_CMSIS_DAP debugging</td>
  </tr>
</table>










https://www.nordicsemi.com/eng/nordic/download_resource/18799/4/95790481

https://www.nordicsemi.com/eng/nordic/download_resource/18974/4/42687144

https://www.nordicsemi.com/eng/nordic/download_resource/18799/7/99017986
