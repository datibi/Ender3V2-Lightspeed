# Lightspeed+ Firmware for the Creality Ender 3 V2 Printers



## Ender 3 V2 Edition

Forked from Marlin -> Miguel Risco-Castillo professional Firmware
<BR/>
This fork has:
- Built so far for 4.2.2
- All G-codes required by LaserGRBL for basic functionality. 
- Engrave from SD card (added *.N* extension)
- Laser mode option in advanced settings (but pretty much useless)
- M3 S<power>: turns on "laser mode": 50Hz PWM, heaters&fan disabled
- M5: restores normal operation mode, 7Hz PWM
<BR/>
- Bugs to solve: preheat from LCD works even in laser mode, M84 without parameter brings up a confirm dialog

Please test this firmware and let me know if it misbehaves in any way.
<BR/>
Please don't forget to disconnect laser before printing :)
<BR/>

Precompiled binary files coming later....


<BR/>


## Disclaimer  

THIS FIRMWARE AND ALL OTHER FILES IN THE DOWNLOAD ARE PROVIDED FREE OF CHARGE WITH NO WARRANTY OR GUARANTEE. SUPPORT IS NOT INCLUDED JUST BECAUSE YOU DOWNLOADED THE FIRMWARE. WE ARE NOT LIABLE FOR ANY DAMAGE TO YOUR PRINTER, PERSON, OR ANY OTHER PROPERTY DUE TO USE OF THIS FIRMWARE. IF YOU DO NOT AGREE TO THESE TERMS THEN DO NOT USE THE FIRMWARE.

## LICENSE
For the license, check the header of each file, if the license is not specified there, the project license will be used. Marlin is licensed under the GPL.
