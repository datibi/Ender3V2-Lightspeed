# Lightspeed+ Firmware for the Creality Ender 3 V2 Printers



## Ender 3 V2 Edition

Forked from Marlin->Miguel Risco-Castillo professional firmware
<BR/>
This fork has the additional features:
<li>LaserGRBL works in specific conditions via USB and SDcard: Marlin mode, importing with "Line to line tracing" and "1bit BW dithering"
<li>Laser mode option in advanced settings (not sure about it's usefullness), it will activate laser at about 1% power.
<li>M3 S[power]: turns on "laser mode": 60Hz PWM, heaters&fan functions set 0 in menu.
<li>M5: restores normal operation mode, 7Hz PWM
<li>Removed gcode preview functionality to save on memory.
<li>Autotemp possible to activate, see mMarlin docs. It's behaviour is not great, nonprinting moves will drive temperature high.
<li>Adjusted some feedrates when loading-uloading filaments
<li>Simple acceleration, way faster rampup than S-curve, more realistic speed, more reliable when pushing acceleration to machine capabilities.
<BR/>
<BR/>
<BR/>
Problems:
<li>Built so far for 4.2.2 with ABL, this is what i have
<li>LaserGRBL in general generates Gcodes that the Marlin parser can not process except the modes enlisted above
<li>No beta testers yet
<BR/>
<BR/>
Please test this firmware and let me know if it misbehaves in any way.
<BR/>
Please don't forget to disconnect laser before printing :)
<BR/>

Precompiled binary files coming later....

<BR/>
Compiling is easy:
<li>Download the zip file with the sourcecode and extract to "Documents"
<li> Install Visual Studio Code, it's free
<li> Within Visual Studio Code in the extension manager search for "Auto build Marlin" and hit install. Leave VSC open, don't do anything for about 15-20 minutes, let the installation finish. When the bottom bar does not show any activity you can go further. It should install automatically PIO too, it may ask you to install it.
<li> "Open folder" with the whole project
<li> Open ABM and the top button "STM32F103RE_creality(512K)" probably is your choice but you should check the controller on your mainboard
<BR/>
<BR/>
## Disclaimer  

THIS FIRMWARE AND ALL OTHER FILES IN THE DOWNLOAD ARE PROVIDED FREE OF CHARGE WITH NO WARRANTY OR GUARANTEE. SUPPORT IS NOT INCLUDED JUST BECAUSE YOU DOWNLOADED THE FIRMWARE. WE ARE NOT LIABLE FOR ANY DAMAGE TO YOUR PRINTER, PERSON, OR ANY OTHER PROPERTY DUE TO USE OF THIS FIRMWARE. IF YOU DO NOT AGREE TO THESE TERMS THEN DO NOT USE THE FIRMWARE.

## LICENSE
For the license, check the header of each file, if the license is not specified there, the project license will be used. Marlin is licensed under the GPL.
