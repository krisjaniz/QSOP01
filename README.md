# QSOP01
Project #01 with the Boldport Club QSOP and 0805 breakout and soldering practice board

[Boldport Club QSOP and 0805 breakout and soldering practice board] (http://www.boldport.club/shop/product/437246682)

Practice project 01
Level SOIC14+16x0805

Disclaimer - I am a complete newbie, anything I say could be completely wrong or just stupid.

In this "project" we solder a NE556D SOIC14 dual timer to the QSOP breakout. That in itself is both easier and harder than soldering proper QSOP ICs. It is easier because there are fewer pins and they are not so close together. Harder, because the pins are wider, which makes positioning and critical and bridging more of a problem.

I chose this chip because it was one that satisfied my criteria for practice soldering better than any other I could find:

1. cheap;
2. sturdy (will survive abuse);
3. you can see it (somewhat) working even if you make a lot of mistakes;
4. mistakes are easy to find and limit troubleshooting to a fairly small number of connections.

Practice is useless if you don't know if you have succeeded - or if making a mistake means you have to go around desoldering and resoldering connections until it works. I had that with PissOff - my first SMD soldering "practice". The LED would light up but there was no function. I must have went around the board with the iron at least three times accidentally bridging connections and desoldering components until I got it working. I still don't know what I did wrong the first time or how I could have found that by looking. If you, like me, are unsure of your SMD soldering skills, this project should help you in the right direction.

First, the components (the product names and numbers in parenthesis are just what I used, it is not critical to use the same products or even the same values, this circuit is not picky):

| Count | Name | Product code | Notes |
| ---- | ---- | ------------ | ----- |
| 1 | NE556D timer | TEXAS INSTRUMENTS  NE556D  TIMER DUAL PRECISION, SOIC14, 556 | NE556D | |
| 4 | LEDs | MULTICOMP  OVS-0801  LED, White, SMD, 1.25mm x 1.4mm, 20 mA, 3.2 V | OVS-0801 | |
| 2 | 1µF capacitors | MULTICOMP  MC0805F105Z160CT  SMD Multilayer Ceramic Capacitor, 0805 [2012 Metric], 1 µF, 16 V, +80%, -20%, Y5V, MC Series | MC0805F105Z160CT | |
| 2 | 0.01µF capacitors | MULTICOMP  MC0805B103K500CT  SMD Multilayer Ceramic Capacitor, 0805 [2012 Metric], 0.01 µF, 50 V, ± 10%, X7R, MC Series | MC0805B103K500CT | these are optional but don't cost anything so why not, they are good for practice |
| 2 | 100kOhm resistors | MULTICOMP  MC01W08051100K  SMD Chip Resistor, Thick Film, 100 kohm, 150 V, 0805 [2012 Metric], 100 mW, ± 1%, MC Series | MC01W08051100K) | |
| 2 | 220kOhm resistors | MULTICOMP  MC01W08051220K  SMD Chip Resistor, 220 kohm, 150 V, 0805 [2012 Metric], 100 mW, ± 1%, MC Series | MC01W08051220K) | |
| 4 | 180Ohm resistors | MULTICOMP  MC01W08051180R  SMD Chip Resistor, Thick Film, 180 ohm, 150 V, 0805 [2012 Metric], 100 mW, ± 1%, MC Series | MC01W08051180R) | Value depends on the LEds you use|

Total cost for the components (even taking into account that some can only be ordered 10 at a time): EUR 3.65 (LEDs are the single most expensive item on the list at 2.80EUR for 10).

Here are all the connections:
![] (https://github.com/krisjaniz/QSOP01/blob/master/qsop_project_01.png)

Start with soldering the NE556D. Check that there are no solder bridges (this is easy by checking adjacent through-hole component holes for continuity with your tester (note that initially only the rows closest to the IC are connected to the IC!). Also check that the pins of the NE556D are all connected (this, again, needs only continuity testing by touching one multimeter probe to the leg of the IC and the other to a through-hole component hole attached to that leg.
The QSOP breakout gives you all the test points you need to do these tests. Nice!

I don't care much in what order you solder the components afterwards. It doesn't matter. It will be easier to solder the components first and then do the connections between pads - but you can do it in any order you like.
Here I soldered up enough to have one LED blinking:
![](https://github.com/krisjaniz/QSOP01/blob/master/20161126_021910-ANIMATION.gif)

You can probably apply any voltage from 4.5V to 16V to the project after it is completed. Check NE556D [datasheet] (http://www.ti.com/lit/ds/symlink/ne556.pdf) for specifics.
All 4 leds should be blinking now.

I originally used tantalum capacitors on this (according to the example circuits in the datasheet, capacitors are polarized) but it seems that's not necessary.

Here is a short movie of it working:
![link](https://goo.gl/photos/m7Y6cHpjvFfkDMJM6)