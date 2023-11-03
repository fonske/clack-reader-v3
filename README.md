# clack-reader-v3
 Esphome component for Clack WS1 softener with M5stack TOF sensor saltlevel detection
 
 Relay for control of the chlorinator module from Aqmos.nl / .de
 and Power measurement with ina219


## Installation
For installation of this module you need to open the clack cover, this can be achieved by gently pulling on the 2 clips on the side. 

Once open, there is just enough space on the right, but this module is designed to be on the bottom

For the Distance sensor, you might want to drill a hole in the back of the module so you can pull the wire trough (a 10 MM hole will work)

Connecting the module:

### General
The power brick/adapter from the clack module will go in the middle in the `power IN`
A new small cable (provided to you) will go from `power OUT` to the clack head. (This should now power up again)

Connect the cable with the 3 loose strands to the connector on the right side with the names `RLY1`, `COM` and `RLY2`.

From here you have to make a choice: (it is one or the other)

#### DP-SW
This will enable you to start or postphone a regen of the wax cylinder.

For this you have been supplied a 2 pin molex cable and can be connected only on their respective spots.

#### Chlorinator
This will enable you to measure the power used by the chlorinator, but also to turn the chlorinator off (This hopefully prolongs the lifespan of the titanium chlorine cell)

For this you need to take the cable that is connected to the PCB of the chlorinator and connect it to the chlorinator port of your V3. The chlorinator will now remain off
In order to turn it on you need to programm the V3 (the relais is NC or Normally Closed)

```
NOTE: 
In normal conditions this cell needs to be replaced once in a while: BE: 2 years max, NL: 3/4 years max.
With this choice hopefully it will last longer.
```

ToDo: Add wire diagram


## Contact
Purchase: alphonsuijtdehaag at gmail dot com, if you are interested in a PCB with wemos s3 mini

Help: Please open a issue on this git project.

