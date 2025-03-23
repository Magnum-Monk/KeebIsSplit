### Keeb is Split v1 Build Guide


![plate](https://github.com/Magnum-Monk/KeebIsSplit/blob/buld_guide_v1/DOC/assets/plate_render.png)

1) First, break/cut the panels off in places, marked here

![cut](https://github.com/Magnum-Monk/KeebIsSplit/blob/buld_guide_v1/DOC/assets/cuts.png)

2) Next - soldering. I would suggest starting with hotswap MX sockets. Follow the footprint markings on PCB

![footprints](https://github.com/Magnum-Monk/KeebIsSplit/blob/buld_guide_v1/DOC/assets/footprints.png)
![footprints_soldered](https://github.com/Magnum-Monk/KeebIsSplit/blob/buld_guide_v1/DOC/assets/footprints_soldered.png)

3) Now solder the SMD Diodes. You got multiple options here.
 - Using soldering paste with hot air gun
 - Using regular solder wire with soldering iron
   
 I won't go in depth on this here, but you can easily find more info on SMD soldering online, [for example](https://www.instructables.com/A-Complete-Beginners-Guide-to-SMD-Soldering/)                                                                                                                   

 I went with the second option. Little tip:
 First put some solder on one of the pads, pick up the Diode with some tweezers. Position it correctly - the markings on the diode should have a stripe, that should be aligned with marking on the pcb itself.
 Next, heat up the pad with solder on it, and carefully slide in the diode leg into solder. Reheat the solder and tweak the positioning of the diode if necessary.
 Here's an image for more clarity: 

![diode](https://github.com/Magnum-Monk/KeebIsSplit/blob/buld_guide_v1/DOC/assets/diode.png)

After all's done, it should look something like this:

![SMD](https://github.com/Magnum-Monk/KeebIsSplit/blob/buld_guide_v1/DOC/assets/SMD.png)

4) Next step is to solder through-hole parts. That being USB-A sockets and reset buttons. Nothing crazy here, just follow the PCB footprint markings.
Little notice - depending on the components you might want to cut off its legs, that extend more than 2mm from the PCB, since they might collide with the case bottom otherwise

5) Soldering the MCU Boards.

If you are planning to use the case, provided with this build, I would highly suggest bying exact pin sockets, mentioned in BOM list in main readme.md file, since the case is designed around using them.

First, cut off the sockets to 12-pin size, You'll need 4 of those. Then prepare some pins of your choice (do not use pins that come with the MCU itself, since they're not compatible with MCU sockets used here). I used spare through hole diode legs, some 0.6mm copper wire would work too. In some previous builds I used copper wire from twisted pair internet cable, that would do too.
Then insert sockets into PCB holes, or better yet - use some "breadboard" if you have one, since there would be no play, and MCU alignment would be much better. Put the MCU board facing down on the sockets, insert your pins through MCU board into sockets.

Should look like this:

![MCU](https://github.com/Magnum-Monk/KeebIsSplit/blob/buld_guide_v1/DOC/assets/MCU.png)

Next. Solder the pins on the MCU. While soldering, keep checking if there are no gaps between MCU and the sockets. I would suggest soldering outermost pins first, and then reseating the MCU (if needed) by reheating said pins while pressing down on the MCU slightly. Try to solder the pins in "cross" pattern, to minimize the unnecessary tension caused by thermal extention of the board. I usually go with top-right -> bottom-left -> top-left -> bottom-right, then center pins, then repeat until all pins are soldered.

Flip the PCB and repeat the same process with socket pins. Again, try to keep the socket headers pushed into the PCB as much as possible to have no gaps between them.

6) Flash the firmware if you haven't already, and you're good to go.

#### Case assembly
Next steps are only needed if you opted for using provided case.

7) First, you need to install m2x5 standoffs into the top case. Mounting holes for them are reasonably spacious, but fitting might be inconsistent depending on print quality/plastic e.t.c. 
Try to insert a standoff into each hole to check how it fits. In my case outermost holes shrunk too much after printing, and I had to use some sanding on the standoffs to fit them in. Those could be tight-fit, no additional adhesive needed.
The rest were fitting nicely, but I still opted for super glue to hold them in place. Little tip: pick up a standoff, screw in an m2 screw into it, apply thin coating of glue on the side of a standoff, carefully insert in into the case, use the screw as a handle to position a standoff inside the case, check if glue has set, then unscrew and repeat. You can install them flush, or slightly "submerged", just check if they're not protruding, to avoid gaps between top and bottom cases.

![TOP](https://github.com/Magnum-Monk/KeebIsSplit/blob/buld_guide_v1/DOC/assets/TOP.png)

8) Screw in m2x5 standoffs to the bottom case with m2x5 screws.

7) (optional) Put in bottom dampening foam in the case, using previously installed standoffs as a guide.

8) Next, place the assembled PCB into the case.

9) (optional) Put in the middle dampening foam on the PCB

10) Screw in switch mounting plate to the standoffs on the bottom case.

Here's a simplified assembly to use as a rough guide:

![assembly](https://github.com/Magnum-Monk/KeebIsSplit/blob/buld_guide_v1/DOC/assets/assembly.png)

In this stage it is a good idea to check if everything fits nicely together. Try on the top case and check if all the USB-C / USB-A holes are positioned correctly. It is essential to follow step 5 thoroughly to be sure that MCU USB-C port is aligned vertically with the case opening for it, as it could be tricky to fix it after sockets are already soldered onto the PCB. Moreover, some ProMicro clones have inconsistent USB-C port positioning, so that is something you should keep in mind too. In the worst scenario you can always use a file to adjust the case opening, noone is gonna judge you :)

11) If everything is okay, put in your favorite switches and keycaps and screw the top case to the bottom case using m2x6 ~ m2x8 screws.

Et voila!








