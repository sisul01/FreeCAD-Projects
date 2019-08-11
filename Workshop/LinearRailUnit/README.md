MGN15_Rail&Block
================

While exploring Thingiverse I came across the constructions of [3DPRINTINGWORLD](https://www.thingiverse.com/3DPRINTINGWORLD/). This inspired me to design my own linear rails. I wanted to know exactly how I could do it and if it was possible to print the rail in multiple segments and still get a bumpless movement.

Since it's all printed in PLA, I don't expect the resulting linear motion to be too accurate. I suspect that the deviation along an imaginary axis will be +/- 0.1-0.2mm in all dimensions. Unfortunately I have no way to measure this.

This design requires a very high precision of the printed parts. It is therefore imperative to calibrate the printer accurately. 
This starts with the extruder, the steps/mm and the flow rate. The printed line width should correspond as closely as possible to the values in the slicer. Then the steps/mm in X and Y can be adjusted. As a result, a calibration cube should deviate max. 0.00 - 0.03mm from the target dimension.

I have oriented myself on existing commercial designs, but made my own adjustments to profile and dimensions. It corresponds approximately to an MGN15.

For my own customizations I have included the FreeCAD file. Adjustments of the dimensions should only be done in the MasterSketchs, otherwise the models might be destroyed.

Slices:
All STL files are already oriented the right way around.

_Print_settings:_
---------------
Material: PLA
Resolution: 0.1mm
Wall Line Count: 3
Infill: 20%
Support: Not required, the block can be switched on from buildplate to get a better interface.

Translated with www.DeepL.com/Translator