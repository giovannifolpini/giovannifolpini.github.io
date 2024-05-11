---
title: "Hotplate soldering iron"
excerpt: "Design and construction of a hotplate soldering iron around an old clothes iron <br/><img src='/images/hotplate_thumb.JPG' width='500'>"
collection: portfolio
---

To solder and desolder SMD components one very useful instrument is a hotplate, but since buying it is not an option for a broke student
i managed to build one crude version with salvaged components.

## Circuit design
The circuit needed to create this hotplate is relatively simple, the main power component is a commercial solid state relay to switch the mains voltage on the iron. <br/> This relay is controlled directly by an Arduino, that also manages the input and output devices, a potentiometer and button and an LCD and status LED respectively. <br/>
The temperature feedback is achieved with the use of a thermocouple and relative digital converter. <br/>
The whole circuit is simply connecting these sensor and actuators together in a prototype board. <br/>

<img src='/images/hotplate_iron/circuit.jpg' width='500'> <img src='/images/hotplate_iron/thermocouple.jpg' width='500'> <br/>


## 3D modelling of the enclosures
To protect the mains wiring from accidental touch i designed a fitting enclosure to be 3D printed, with the necessary cutouts for all the wires. <br/>
The control panel and circuit box is also 3D modelled and printed; the panel is tilted by 45 degrees so that the non backlit LCD can be read easily. <br/>

<img src='/images/hotplate_iron/front_panel.jpg' width='500'> 
<img src='/images/hotplate_iron/panel_arm.jpg' width='500'> <br/>
