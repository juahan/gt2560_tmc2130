# gt2560_tmc2130
The plan is to find a way to make Geeetech GT2560 to work with TMC2130.

## Hardware connections
Here more on how to connect the drivers.

## Changes to Marlin
Here will be the description for modifying Marlin config to allow TMC2130 in 
it's full glory with all (or most of the) the functions.


## Work in progress info dump

Some preliminary information and data:
- https://www.geeetech.com/wiki/index.php/GT2560
- https://github.com/MarlinFirmware/Marlin/blob/1.1.x/Marlin/pins_GT2560_REV_A.h
- https://github.com/MarlinFirmware/Marlin/blob/1.1.x/Marlin/Configuration_adv.h
- http://reprap.org/wiki/Geeetech_GT2560

From Youtube discussion (Salander - How to make your 3D printer smart and silent with the TMC2130!)
- "Hello! I have a GT2560(revA+) and i'm planning to upgrade X and Y axle only. Unfortunately 
cs_x {video} goes to the SD card's cs on the Geeetech board (cs_y {video} is on a female header 
of the second stepper driver which is free so its ok). My question is what to modify in Marlin if 
i would like to keep SD-reader working? (using a another pin on atmega chip may be ok as well)"
- "Details: cs_x{video} is on DigitalPin53 (19. physical pin on atmega) which is on SD reader and 
cs_y{video} goes to DigitalPin49 (35. physical pin on atmega) which is free. As an option i'm 
thinking about DigitalPin48 (36. physical) which would be perfect as being lead to another free 
female header. The problem is that i'm not that pro on Marlin."
