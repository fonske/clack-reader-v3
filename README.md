# clack-reader-v3
 Esphome component for Clack WS1 softener with M5stack TOF sensor saltlevel detection
 
 Relay for control of the chlorinator module from Aqmos.nl / .de
 and Power measurement with ina219


## Installation
A dutch installation manual is written by [ViezeVis](https://github.com/ViezeVisNL). Visit his [webpage](https://bashoogers.nl/2024/01/11/clack-reader-v3-instructie-installatie-home-assistant/) for the document.
The englisch version, you can find [here](https://bashoogers.nl/2024/01/22/clack-reader-v3-en-installation-manual-home-assistant/)

For installation of this module you need to open the clack cover, this can be achieved by gently pulling on the 2 clips on the side. 

Once open, there is just enough space on the right side inside the Clack for the Clack reader PCB, but the chlorinator PCB is designed to be on the bottom

For the Distance sensor, first install the 4-wire cable through the hole were the power supply goes through, after that the wire of the power supply.
The flex cable will not be in the way, when inserted first, instead of the other way around.

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

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/ebbenberg)
