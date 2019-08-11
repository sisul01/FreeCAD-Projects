Anet A6 Fan Duct
================

Since the original fan channel is directed directly at the nozzle, I redesigned it. The airflow is now more directed against the nozzle tip.
I created two versions of the fan duct, one with lamellas (FanDuctLaminar.stl) and one with inner supports only (FanDuctStd.stl).

In order to minimize the air turbulences and to achieve an airflow directed towards the surface, I used the principle of laminar flow.
I achieved this by introducing several lamellas into the duct. This has reduced the total volume flow somewhat, but the better alignment of the flow means that more air reaches the surface of the printed part.

-----------------------------------
###Note: 04.06.2019:
After using the lamella duct (_FanDuctLaminar.stl_) for some time, I noticed some problems with it. 
On the one hand, the cooling effect on very thin-walled components is so great that the layers do not stick to each other. The only solution is to reduce the fan power.
On the other hand, there is a reduced cooling performance on the opposite side of the fan. This is because of the lack of air turbulence due to the well directed flow on the other side.
Therefore I can recommend the fan with the lamellas only in very limited cases. But with the improved normal version (_FanDuctStd.stl_) I made good experiences.

-----------------------------------

I did tests with salt to illustrate the difference. In both cases the nozzle is 1mm above the surface.

![original fan duct](https://thingiverse-production-new.s3.amazonaws.com/assets/79/bf/4c/78/a8/20190213_160619.jpg)
![new version with lamellas](https://thingiverse-production-new.s3.amazonaws.com/assets/45/82/da/42/9f/20190213_161602.jpg)

_Printer settings:_
-------------------
Material: PLA, ABS, PETG, ...
Resolution:  0.2mm
Wall thickness: 1.2mm
Infill: doesn't matter
Support: no
