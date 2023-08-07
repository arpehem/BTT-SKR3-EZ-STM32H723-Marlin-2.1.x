# BTT-SKR3-EZ-Marlin-2.1.x 
This is my Marlin configuration and firmware to be used with an Ender 5 plus with the **Big Tree Tech SKR 3 EZ** motherboard with the **STM32H723VG** processor variant and the **Big tree tech TFT35 V3**.

Make sure to adjust the probe Z-offset to avoid bed damage. **Z offset is intentionally to high to avoid bed damage, if you don't adjust it, you should print above, not on the bed!** It's value should be equal to the distance between the bed and the nozzle when the probe triggers. Ajdjust XY in the negative if the probe is front left of the nozzle, positive if it's back right. For more information, look at the NOZZLE_TO_PROBE_OFFSET info in the Configuration.h file.

USB and SD cards both work. You can print from the screen, onboard USB, SD card or host (octoprint, ponterface...).

Platform.ini goes in the main marlin folder(Marlin-bugfix-2.1.x), the other 3 files go in the marlin sub folder (Marlin).

Use VS code with the Marlin autobuild plugin and your printer should be good to go!

Don't forget to set NOZZLE_TO_PROBE_OFFSET, bed level, PID tune, Tune E-steps and confirm servo directions as well as change bed level device if not BLTouch.
