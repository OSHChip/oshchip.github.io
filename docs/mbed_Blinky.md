---
layout: page
title: Setting up and using the mbed Classic site for OSHChip
excerpt: "mbed Blinky"
tags: [OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart, mbed]
categories: [Electronics]
comments: false
modified: 2016-03-26
image:
  feature: header.jpg
---

The long term plan is to have OSHChip registered as an mbed enabled platform, but until that is done,
the following describes how to get started with mbed and OSHChip, using a simple **blinky** example.

1. To try it out, you should go to the Classic mbed web site and create an account if you don't already
have one:  
  <a href="https://developer.mbed.org/" target="_blank">https://developer.mbed.org/</a>
2. After logging in, select **Compiler** in the top right corner.
3. Click on the **Import** button
4. Select the program tab, and type **OSHChip_Blinky** in the search box, and click Search
5. Double click on the result line, select "import as program" and either accept or modify the import
   name, then click **Import**.
6. Read the 3 files to understand what is going on.
7. Confirm that the target board selected is nRF51-DK (Default) in the top right corner of the page.
8. Click the compile button. Compilation should only take a few seconds, then you should be presented
   with a HEX file to be saved. (OSHChip_Blinky_NRF51_DK.hex if you didn't change the project name in
   step 5 above)
9. Save this to the USB drive for the OSHChip_CMSIS_DAP. This should load the program into the Flash
   memory in OSHChip, and then the program should run and blink the 3 on-board LEDs.

Basically, what is going on here is that you tell the mbed system that you are using the nRF51-DK board
(from Nordic Semiconductor) that uses the same processor chip as OSHChip. Then as you can see in the
example project, there is a replacement header file that is OSHChip specific, and a trivial
initialization function that re-assigns the UART to pins 1 and 2 of OSHChip.

The resulting HEX file is surprisingly large (if you save it to a normal disk drive, you will see that
it is 320 KB. This is because with mbed, the hex file always includes the *SoftDevice* for Bluetooth
Low Energy (BLE), regardless of whether you are using BLE or not. This means that download time to
OSHChip is a few seconds longer than if the SoftDevice was not part of the HEX file.
