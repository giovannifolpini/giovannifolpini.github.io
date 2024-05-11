---
title: "VFD clock"
excerpt: "Design and construction of a clock around a vintage VFD tube<br/><img src='/images/VFD_thumb.jpg' width='500'>"
collection: portfolio
---

An old calculator found in an electronics fair contained a vacuum fluorescent display (VFD) tube, with six "7 segments" digits.
Since the calculator was broken i decided to test whether the display was still functional and to my surprise it was, so
what else could i do if not make it into a clock?

## Multiplexing
Displaying information on a 7-segment display is commonly done with the technique of multiplexing. <br/>
This approach consists of tieing all the same segments of different digits together, while the anodes/cathodes of the single digits remain separated. This configuration allows to turn on a segment for all digits but then to only turn on a single digit, with the help of persistence of vision we can then switch this process fast enough so that it looks like the necessary segments are lit at the same time on all digits. <br/>
On a hardware level this is done with the help of a shift register and transistors. 
The shift register shifts out a string of bits corresponding to the segments, the transistors then switch the voltage at the desired anode of the tube. <br/>
The software is relatively simple once we create an array that relates the combinations of bits to be shifted out and the associated number to display on the VFD. We can then use functions that accepts the number to display as an argument and it'll display it on the corresponding digit. By alternating the six functions, one for every digit, we achieve the desired result.

<img src='/images/VFD_clock/full_clock.jpg' width='500'> <img src='/images/VFD_clock/solder_joints.jpg' width='500'> <br/>


