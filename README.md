# CNC-music-factory
This is my set of upgrades to a baseline 3018 CNC to support machining of wood for guitar necks, organ pipes, and other noisy bits.

The resulting machine has nearly 5x the cutting volume (300mm x 775mm x 50mm instead of the stock volume of 300mm x 180mm x 45mm) and 10 times the power (The spindle has been upgraded from the stock 75W one to a 750W Bosch Colt router).

![Overview image](https://github.com/thecowgoesmoo/CNC-music-factory/blob/main/Images/CNCMF_DiagFull.jpg)

## Overview
Playing music and making/modifying musical instruments has been a lifelong hobby of mine.  Electronic instruments have long been more accessible to DIY hobbyists given the increasing availability of custom printed circuit boards and the relatively low cost of basic electronic assembly tools.  3D printing and affordable hobbyist CNC machines have made construction of custom acoustic and electromechanical instruments more accessible than ever before.  

3D printing has been exciting, but available materials are not ideal for some acoustic applications (relatively high density and low stiffness compared to wood, for instance).  Laser cutting is a strong complementary technology, and K40 lasers have also achieved a <$500 USD price point, but these are largely limited to 2 dimensional cuts.  

A Genmitsu 3018 CNC has opened up new materials and geometries to me and had an initial price that was within my reach (<$200 USD).  The CAD and CAM learning curves proved considerably steeper than the SW tools for 3D printing, where large databases of free designs are readily available online and slicing SW is now relatively mature, general, and user-friendly.  And as I learned to use the 3018, its actual power, geometry, and accuracy proved to be quite constraining.  In particular, I was interested in being able to machine guitar necks from wood in less than a day of machining and without workpiece tiling.  As with lasers, there is a considerable price jump from the entry-level machines (~$200USD) to mid-level hobby machines (>$1000USD). 

My solution has been incremental upgrades, first to improve accuracy, then power, then machining volume.  The resulting machine appears to fill a capability and price point gap in the current commercial offerings (~$250USD beyond the baseline 3018 cost for 10x spindle power and a 1 meter y axis), so I've decided to share my set of upgrades for others to use if they please.  

## Assembly
1. Start with assembled and tested Genmitsu 3018 CNC
- a. Assuming Candle for pushing g code
- b. Assuming Fusion 360 for CAM
2. Build waste board
- a. Screw 1"x2" lumber to sides of melamine cut to dimensions
- b. Drill and countersink for mounting to aluminum plate
- c. Drill and mount aluminum side rails
- d. Bevel ends
3. Install lengthened Y axis:
- a. Remove existing Y axis v rail, linear bearing rails, and lead screw
- b. Install longer Y axis v rail, linear bearing rails (on plywood ends), and lead screw
- c. Mount extended waste board
- d. Install extension cable for stepper motor
4. Build new spindle carriage
- a. Cut profiles from plywood with laser
- b. Print assembly guides
- c. Glue, stack, and bolt with guides in place
- d. After drying, install antibacklash nut and linear bearings
- e. Mount new carriage on lead screw and linear rails and couple to stepper motor
5. Final bits
- a. Install 608 rollers under bed
- b. Print and install guide rollers for side/top
- c. Install carriage and check full range of travel for all axes
- d. Print and install meter mount
- e. Update GRBL setting for Y axis scaling
- f. Check bed leveling with meter
- g. Attach pen and draw shapes CW and CCW to check for backlash
6. First cut
- a. Run circle diamond square test
