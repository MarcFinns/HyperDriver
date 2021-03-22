# HyperDriver
LED driver and power board for Hyperion (DYI Ambilight)

See short video: https://www.youtube.com/watch?v=JoaK5aRHBMA

After setting up hyperion I was annoyed by starting/stopping it manually every time.
My weekend project was to build a proper solution - with components I had in the drawer, which might explain some weird design choices.

The board does the following:

* Connects as a PI hat
* Powers the PI and the LED strip with the same power supply
* Provides 5V drivers / level adaptation for the APA 102 LED stripe
* Allows to turn the PI on by pushing a button
* With the same button, triggers a proper shutdown (no abrupt power cut)
* Connects to TV via USB and can start the PI when the TV turns on
* The PI can automatically shutdown when TV goes off (immediately or after X minutes)
* If the automatic turn on from TV is triggered, the PI can still be shut down via the button
* A 5V socket is available for a small fan, in case

The On/Off function is proper, meaning the power supply is truly disconnected from the mains when off.
I made sure that the PCB is single side and doable at home with some medium skills (e.g. i made it with toner transfer). 
I could not avoid one SMD but only because I did not have the through-hole part in the drawer. Convertinf the PCB to through hole is trivial.
The whole thing fits in a small electric junction box. See pictures.

**IMPORTANT DISCLAIMER:**<BR>
* This is **NOT** your typical 5V Arduino project. <BR>
* It is **NOT** breadboard friendly.<BR>
* Make it **ONLY** if you know what you are doing.<BR>
* Danger of electrocution

