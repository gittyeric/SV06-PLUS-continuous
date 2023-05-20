# SV06+ Continuous Printing!

(IN DEVELOPMENT, THIS SECTION IS FUTURE DOCS:)

Mostly just a branch of SV06+'s Marlin code, but supports continuous printing via part ramming and TSC motor driver feedback to sense stuck parts and handle retries.  Simply start a Y home (ex. `G28 Y R0`) starting from the max Y coordinate to trigger a "special" Y homing that will sense ramming a stuck part and pause / retry rams after further cooling.  Every detected bump pauses ramming for 15 minutes until it tries again, with the hope that a cooler part will now bump off.  After an hour of failure the print will be failed and block your continuous print queue until manual intervention.

WARNING!  Ramming your bare extruder head into a stuck part isn't a good idea.  Maybe consider a ram shield (link TODO) and bed slide (link TODO) to safely bump parts without damaging your extruder or jamming your printer with fallen parts.

Below is the original SV06+ branch README docs:

# Introduction

Sovol SV06 PLUS is a 300*300*340 mm large size printer with compact functions. It adopts the movement structure of polished rod and bearings, thus, no wheels on the printer anymore! 
It’s with a High Flow Hotend and a Planetary Gear Direct Drive Extruder, which supports printing at a high speed and printing with soft TPU and high-temperature filament, such as PETG, ABS, Carbon Fiber, etc. 
Touch screen, PEI Plate, 25 point Auto Leveling, 32bit Silent Mainboard, Dual Z axis, and Belt Tensioner are all pre-installed on the SV06 PLUS. Welcome to check more on sovol3d.com
# Related tutorials 

- User Manual. [Click here](https://drive.google.com/file/d/1bJmc2MeOSmn5svG3CuQQvvp3vNMjcOrR/view)

# Learn more

on Sovol Official Website: https://sovol3d.com/products/sovol-sv06-plus

# Source code

This is the official source code for Sovol SV06 PLUS. The damage caused by modifying firmware also using the third party firmware will lose the 1 year warranty. If you need support, it’s recommended to reflash the stock firmware before contacting sovol.

Sovol doesn’t provide tech help for help users to modify source code, but if you need us to add more functions, you are welcome to send us your suggestions via Facebook Messenger or email 
info@sovol3d.com


# Join Sovol Community

- Sovol Facebook page: https://www.facebook.com/sovol3d/
- Sovol Youtube Channel: https://www.youtube.com/c/Sovol/videos
- Sovol Offcial User Group: https://www.facebook.com/groups/sovol3d
- Sovol Forum website: https://forum.sovol3d.com/
- Sovol SV06 PLUS & SV06 Official User Group: https://www.facebook.com/groups/sovolsv06usergroup

