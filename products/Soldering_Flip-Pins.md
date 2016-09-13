---
layout: page
title: Soldering Flip-Pins
excerpt: "Soldering Flip-Pins"
tags: [Flip-Pins, OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart]
categories: [Electronics]
comments: false
modified: 2016-09-12
image:
  feature: header.jpg
---

### Notes

Flip-Pins are held loosely within the plastic aligner, which is designed
to tolerate soldering temperatures. The solder tail extends
approximately 0.062" so that when installed in a PCB that is the common
thickness of 0.062", it will result in a near flush top surface.
Sometimes the pins can fall out before being soldered into the board.
Just re-insert the pin into the plastic aligner, and adjust it to be at
the same depth as the rest of the pins.

If you need to install a row of pins that is not one of the standard
lengths (8, 14, and 20 pins), you can use multiple Flip-Pins to get the
length you need, or you can remove pins from an aligner, as needed.
Because the length of the plastic aligner is 0.020" longer than the
number of pins * 0.100" , the Flip-Pins can't be installed end-to-end.
The solution is to solder the pins in two stages. For example, if you
were adding pins to a Teensy 3.6, you would need to install 24 pins in a
row. Place two 8 pin parts, one at each end of 24 holes, and solder in,
then remove the two plastic aligners. You can then install the middle 8
pin part and solder it.



<html>
  <table border="1" cellpadding="5">
    <tr>
      <td style="width:50%; vertical-align:top;">Parts to be assembled. For clarity, all pictures are shown without
                  other components. Typically you would mount all other components first, before soldering in Flip-Pins.<br><br><i>Photo Credit for all picture: Windell Oskay</i></td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_Parts_to_be_assembled_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_Parts_to_be_assembled_w400.jpg"></A></td>
    </tr>
    <tr>
      <td style="width:50%; vertical-align:top;">Insert the soldertail end of the Flip-Pin into the appropriate holes on your PCB</td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_Insert_Flip-Pins_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_Insert_Flip-Pins_w400.jpg"></A></td>
    </tr>
    <tr>
      <td style="width:50%; vertical-align:top;">Place your board with the Flip-Pins on a flat surface</td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_Ready_for_soldering_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_Ready_for_soldering_w400.jpg"></A></td>
    </tr>
    <tr>
      <td style="width:50%; vertical-align:top;">Solder 1 pin, at the end, of each Flip-Pin strip(s). If this is your first time soldering Flip-Pins, you might want to practice on a spare prototype PCB to get a feel for how much solder is the right amount.</td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_Solder_1_pin_on_each_strip_a_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_Solder_1_pin_on_each_strip_a_w400.jpg"></A></td>
    </tr>
    <tr>
      <td style="width:50%; vertical-align:top;">After soldering the end pins, your board should look like this.</td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_Solder_1_pin_on_each_strip_b_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_Solder_1_pin_on_each_strip_b_w400.jpg"></A></td>
    </tr>
    <tr>
      <td style="width:50%; vertical-align:top;">Take the assembly, and check that the plastic aligner(s) is at right-angle to the PCB</td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_Check_pins_are_at_rightangle_to_PCB_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_Check_pins_are_at_rightangle_to_PCB_w400.jpg"></A></td>
    </tr>
    <tr>
      <td style="width:50%; vertical-align:top;">Check that the plastic aligner(s) is flush to the PCB</td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_Check_plastic_aligner_is_flush_to_PCB_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_Check_plastic_aligner_is_flush_to_PCB_w400.jpg"></A></td>
    </tr>
    <tr>
      <td style="width:50%; vertical-align:top;">Solder the remaining pins</td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_Solder_remaining_pins_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_Solder_remaining_pins_w400.jpg"></A></td>
    </tr>
    <tr>
      <td style="width:50%; vertical-align:top;">Remove the plastic aligner(s) by pulling it off, being careful not to bend the pins</td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_Carefully_remove_plastic_aligner_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_Carefully_remove_plastic_aligner_w400.jpg"></A></td>
    </tr>
    <tr>
      <td style="width:50%; vertical-align:top;">With the plastic aligner removed, you may optionally inspect the pin side of the PCB and see if there is sufficient solder to fill the hole in the PCB. If you want to add more solder,
                             put the aligner back on the pins, and add more solder from the top side. If there is too much solder, learn to use less, next time.</td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_1_aligner_removed_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_1_aligner_removed_w400.jpg"></A></td>
    </tr>
    <tr>
      <td style="width:50%; vertical-align:top;">The finished assembly after all aligner(s) have been removed.</td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_Finished_a_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_Finished_a_w400.jpg"></A></td>
    </tr>
    <tr>
      <td style="width:50%; vertical-align:top;">Another view of the finished assembly</td>
      <td style="width:50%;"><A HREF="/images/Flip-Pins_Assembly_Finished_b_w1200.jpg" target="_blank"><img src="/images/Flip-Pins_Assembly_Finished_b_w400.jpg"></A></td>
    </tr>
  </table>
</html>


