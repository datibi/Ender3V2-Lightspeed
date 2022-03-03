# Lightspeed+ Firmware for the Creality Ender 3 V2 Printers



## Ender 3 V2 Edition

Forked from Marlin->Miguel Risco-Castillo professional firmware
<BR/>
This fork has:
- Built so far for 4.2.2
- All G-codes required by LaserGRBL in Marlin mode for basic functionality. 
- Engrave LaserGRBL file from SD card (added &lowast;.N&lowast; extension)
- Laser mode option in advanced settings (not sure about it's usefullness), it will activate laser at 1% power.
- M3 S<power>: turns on "laser mode": 60Hz PWM, heaters&fan disabled
- M5: restores normal operation mode, 7Hz PWM
- Removed gcode preview functionality to save on memory.
- Activated autotemp, but it's behaviour is not great, nonprinting moves are not filtered out (Marlin issue).
<BR/>

Please test this firmware and let me know if it misbehaves in any way.
<BR/>
Please don't forget to disconnect laser before printing :)
<BR/>

Precompiled binary files coming later....

<BR/>
Compiling is easy:
<BR/>
- Download the zip file with the sourcecode and extract to "Documents"
<BR/>
- Install Visual Studio Code, it's free
<BR/>
- Within Visual Studio Code in the extension manager search for "Auto build Marlin" and hit install. Leave VSC open, don't do anything for about 15-20 minutes, let the installation finish. When the bottom bar does not show any activity you can go further. It should install automatically PIO too, it may ask you to install it.
<BR/>
- "Open folder" with the whole project
<BR/>
- Open ABM and the top button "STM32F103RE_creality(512K)" probably is your choice but you should check the controller on your mainboard
<BR/>
<BR/>


## Disclaimer  

THIS FIRMWARE AND ALL OTHER FILES IN THE DOWNLOAD ARE PROVIDED FREE OF CHARGE WITH NO WARRANTY OR GUARANTEE. SUPPORT IS NOT INCLUDED JUST BECAUSE YOU DOWNLOADED THE FIRMWARE. WE ARE NOT LIABLE FOR ANY DAMAGE TO YOUR PRINTER, PERSON, OR ANY OTHER PROPERTY DUE TO USE OF THIS FIRMWARE. IF YOU DO NOT AGREE TO THESE TERMS THEN DO NOT USE THE FIRMWARE.

## LICENSE
For the license, check the header of each file, if the license is not specified there, the project license will be used. Marlin is licensed under the GPL.
