# WaterPumpPowerConverter

# Summary
This repository contains a Switch Mode Power Supply(SMPS) that is used to power and control the water pumps developed for the various water fountains on Thingiverse. The SMPS module is based around the LM2596 chip. As well as this, a 3D printable case was developed using Fusion 360. The 3D Model of the PCB is shown below:

![3D Render](docs/3D%20PCB%20Model.png)

# Design
As for the design, I designed the circuit to use existing parts that I already had from previous projecs, this is why it consists of all through hole components. There is a lot of improvements that can be made to this design which are outlined below in the improvement section. As for the design, it was ordered through JLCPCB and is shown below:

![Populated PCB](docs/Water%20Pump%20Power%20Converter%20Assembled.jpg)

# Improvements
There is a lot of improvements that can be undertaken for this PCB. First off there was a couple of issues during its manufacture and population. On the PCB itself, specifically the top left corner the PCB was malformed resulting in a non rectangular shape, this didnt functionally change the PCB more its aesthetics. As well as this the Lm2596 modules I ordered were originally clones, which mean that i had to remove the module from the board resulting in damaged to PCB pin holes, as seen in the picture above.

Layout Improvements include the following:

- Better Ground Stitching, at present there is not many ground stitching between the top and bottom ground planes, this results in an uneven ground signal.
- LM2596 Through hole replacement, the layout is better done with the SMT version as this allows the reduction of loop sizes and thus a reduced EMI design can be created.
- Replacement of the unsheilded inductor. Due to available parts a non shielded inductor was used, however this resulted in increased EMI and thus created a noisy output voltage.

# Software Requirements:

The following software packages are required for this project:
- [Eagle](https://www.autodesk.co.uk/products/eagle/overview?term=1-YEAR&tab=subscription)
- [Fusion 360](https://www.autodesk.com/products/fusion-360/overview?term=1-YEAR&tab=subscription)

# Useful Links
- [Thingiverse Case](https://www.thingiverse.com/thing:4596788)
- [Case Exploded View](https://www.youtube.com/watch?v=MiPNAOpEotw)
- [JLCPCB](https://jlcpcb.com/)
- [Water Pump](https://www.thingiverse.com/thing:4594864)
- [Water Fountain](https://www.thingiverse.com/thing:4594351)
