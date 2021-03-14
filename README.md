# HyperDriver
LED driver and power board for Hyperion

After setting up hyperion I was annoyed by starting/stopping it manually every time.
My weekend project was to build a proper solution - with components I had in the drawer.

The board does the following:

* Connects as a PI hat
* Powers the PI and the LED strip with the same power supply
* Provides 5V drivers / level adaptation for the APA 102 LED stripe
* Allows to turn the PI on by pushing a button
* With the same button, triggers a proper shutdown (no abrupt power cut)
* Connects to TV via USB and can start the PI when the TV turns on
* The PI can automatically shutdown when TV goes off (immediately or after X minutes)
* If the automatic turn on from TV is triggered, the PI can still be shut down via the button

The On/Off function is proper, meaning the power supply is truly disconnected from the mains when off.
I made sure that the PCB is single side and doable at home with some medium skills. I could not avoid one SMD as i did not have the through-hole part in the drawer, but it is trivial to convert it.
The whole thing fits in a small electric junction box. See pictures.

DISCLAIMER
This is not your typical 5V Arduino project. 
It is NOT breadboard friendly.
Make it only if you know what you are doing.
