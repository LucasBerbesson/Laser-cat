
## Laser Tower for the CAT 
Pseudo-randomly moves a servo tower (on X and Y axis) and lights up a laser.

Watch it working : [https://www.youtube.com/watch?v=hHIrxL0giJQ](https://www.youtube.com/watch?v=hHIrxL0giJQ)


## Set up
x_servo is attached to pin 9 (and +5V and GND) and moves in the X plan.

y_servo is attached to pin 6 (and +5V and GND) and moves in the Y plan.

Laser is attached to pin 13 (and GND).

Download the .ino file, open it inside the arduino software and send it to your arduino. 

## How it works : 
The program randomly choose a new position for the laser inside a square you can define in the variables.
It checks the new position is different from the old one of at least "minimal_movement".
It moves the tower to the new position and stays still for a time between min_freeze and max_freeze 
(this aims to reproduce the behaviour of an insect landing somewhere for a bit and then flying off, 
that's the variable you need to increase if your cat is fat...).
Ans starts the process over and over again. 

Created 30 Sep 2016 by Lucas Berbesson for La Fabrique DIY

