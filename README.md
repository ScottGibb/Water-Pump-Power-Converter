# WaterPumpPowerConverter

# Summary
This repository contains a Switch Mode Power Supply(SMPS) used to power and control the water pumps developed for the various water fountains on Thingiverse. The SMPS module is based around the LM2596 chip. As well as this, a 3D printable case was designed using Fusion 360. The 3D Model of the PCB is shown below:
![3D Render](docs/3D%20PCB%20Model.png)

# Design
As for the design, I designed the circuit to use existing parts that I already had from previous projects; this is why it consists of all through-hole components. There are a lot of improvements that can be made to this design outlined below in the improvement section. As for the design, it was ordered through JLCPCB and is shown below:

![Populated PCB](docs/Water%20Pump%20Power%20Converter%20Assembled.jpg)

# Improvements
There are a lot of improvements that can be undertaken for this PCB. First, there were a couple of issues during its manufacture and population. On the PCB itself, specifically in the top left corner, the board was malformed, resulting in a non-rectangular shape; this didn't change the functionality more than its aesthetics. As well as this, the LM2596 modules I ordered were originally clones, which meant that I had to remove the module from the board, resulting in damage to PCB pin holes, as seen in the picture above.


Layout Improvements include the following:

- Better Ground Stitching, at present, there is not much ground stitching between the top and bottom ground planes. This results in an uneven ground signal across the circuit, further resulting in power instability.
- LM2596 Through hole replacement, the layout is better with the SMT version as this allows the reduction of loop sizes, and thus a reduced EMI design can be created.
- Replacement of the unshielded inductor. Due to available parts, a non-shielded inductor was used. However, this resulted in increased EMI and thus created a noisy output voltage.

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
