# clack-reader-v3
 Esphome component for Clack Ecosoft LESS softener with M5stack TOF sensor saltlevel detection
 
 Relay for control of the chlorinator module from Aqmos.nl / .de
 and Power measurement with ina3221

## Versions / Branches
main: Tof1 sensor (VL53L0X) code without measurement during brine option.

tof1: Tof1 sensor (VL53L0X) code with measurement during brine option.

tof2: Tof2 sensor (VL53L1X) code with measurement during brine option

tof2less: Tof2 sensor (VL53L1X) code for clack Ecosoft LESS from Aqmos. This will be a different PCB then the original Clack reader V3

## Installation
under construction

### General
under construction

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

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/ebbenberg)
