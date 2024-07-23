Small 3D-Printed PCB-CNC

This is a small, mainly printed small table router for anyone who just wants to try out whether a CNC router or engraving machine is something for them. Ideally, you already have some of the required parts such as stepper motors, power supplies etc. lying around.

I have wanted to build a CNC milling machine or a CNC engraving machine for a long time. Simply out of technical curiosity, I couldn't imagine any real use other than engraving PCBs. So I wanted it to be inexpensive, but with the best possible features.
So I came up with the idea of designing a CNC machine with as many 3D printed parts as possible to keep costs down. All the parts fit on the print bed (220 mm x 220 mm) of my 3D printer.

The result is a machine with the following data:

Work volume (xyz)mm: 120 x 120 x 60
Frame (xyz)mm: 275 x 275 x 320
Motor: DC motor, 24V, 200W, 52mm diameter
Spindle: 10000rpm
Axes: 3 x NEMA17
Controller: Arduino Uno with GRBL shield
Firmware: GRBL 1.1
Special features: backlash prevention, end stop, cable management
Supported materials: Acrylic, wood, PVC, PCB and possibly soft metals

Cost if you have to buy everything: approx. 160$ - 200$

The current version is relatively rigid, I used PLA for the frame, which is a stable, hard plastic. The thermal impact of these components is low, so PLA is well suited and also an inexpensive material. The guide rods with a diameter of 10 mm in the X and Y axes and the short length also contribute to stability.
For the first version, I decided to insert the screws directly into the plastic without heatset inserts. With the smaller threads, the screws can be screwed directly into the plastic without first using a tap. As the screws heat up relatively strongly when they are first screwed in, I recommend waiting a moment for cooling down before finally tightening them. The M5 threads should be pre-cut. 

I attached the (optional) limit switches with adapter plates. This makes it relatively easy to set the trigger point. If limit switches other than the ones I chose are used, it is possible to modify the adapter plates with little effort. Practice has shown that the limit switch cables are very susceptible to interferences. I did this by using shielded audio cable for the wiring and also galvanically isolated the signal with optocouplers in accordance with the instructions ['Wiring Limit Switches'](https://github.com/gnea/grbl/wiki/Wiring-Limit-Switches) in the GRBL wiki.

The use of the backlash prevention nuts is also optional. If these are used, I have found that the spring supplied is rather weak. Ideally, the spring should be replaced by a stronger version with the same diameter.

The cable management is realized by a cable chain on the X-axis and feedthroughs for cable ties on the side panels.

I used an Arduino Uno with GRBL shield and A4988 stepper motor drivers as the controller. I will not provide any further information on wiring here. I assume that anyone who builds a machine like this knows what they are doing or is able to follow the countless instructions on the Internet.

For the mechanically stressed 3D printed parts, you should ensure that the wall thickness is sufficient, i.e. the perimeter thickness should be 1.6mm - 2mm. Not to be forgotten are the horizontal layers, which should also have these dimensions. The mechanically stressed parts include: Base-Frame, SidePanel_Left, SidePanel_Right, RearStrut, Y-Sled, X-Sled, Z-Sled, X-Sled_BottomPlate and X-Sled_TopPlate. PLA can be used for most parts. This results in the required rigidity for the frame construction due to the material properties of PLA. I printed the X-, Y- and Z-sleds in PETG, as this is where most of the vibrations occur and this material can absorb them better.

All printed parts are available as STL and STEP files. The STL files are already aligned for printing. Also published is a parts list and an assembly in STEP format with all parts including screws, so that a good overview of the project is possible. You are also welcome to use the STEP files for your own modifications and remixes


Tags
cnc, CNC Machine, cnc mill, cnc router, diy cnc router, mill, milling, router, engraving machine, engraving, pcp cnc, pcb milling, pcb