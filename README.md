![Hall Effect Thruster — Magnetic Field Model](Banasset)

[README.md](https://github.com/user-attachments/files/28627607/README.md)
# Hall Effect Thruster (HET) — Research & Design Project

Scaling analysis, magnetostatic modeling, and CAD design of a Hall Effect Thruster, with an accompanying research manuscript currently under peer review at the **Journal of Engineering and Applied Sciences, Springer Nature**.

![Status](https://img.shields.io/badge/Status-Research%20%2F%20Experimental-blue)
![Power Class](https://img.shields.io/badge/Power%20Class-200W-orange)
![Propellant](https://img.shields.io/badge/Propellant-Xenon-purple)
![Tools](https://img.shields.io/badge/Tools-FEMM%20%7C%20SolidWorks-gray)
![Under Review](https://img.shields.io/badge/Manuscript-Under%20Review%20%40%20Springer%20Nature-green)
![License](https://img.shields.io/badge/License-All%20Rights%20Reserved-red)

---

## Repository Structure

```
├── CAD/                  # SolidWorks part and assembly files
├── FEMM/                 # Magnetic field simulation files (FEMM format)
├── Scaling/              # Thruster scaling analysis spreadsheet (.xlsx)
├── Gallery/              # Miscellaneous project images and visuals
└── REFERENCES.md         # Full list of papers and resources used
```

---

## Project Overview

### 1. Scaling Analysis
Thruster dimensions and operating parameters were derived from Hall thruster scaling laws. The scaling methodology closely follows the work of **Mahajan et al. (2025)** on 500W-class Hall thruster development. The spreadsheet in `Scaling/` documents the computed parameters used to size the thruster geometry, including discharge channel dimensions, propellant flow rates, and power estimates.

### 2. Magnetic Modeling
Magnetostatic simulations were performed using [FEMM (Finite Element Method Magnetics)](https://www.femm.info/wiki/HomePage). The `.FEM` files in `FEMM/` contain the magnetic circuit geometry, material definitions, and boundary conditions used to shape and optimize the radial magnetic field profile across the discharge channel.

### 3. CAD Design
A 3D model of the thruster was developed in **SolidWorks** based on the scaled parameters and magnetic modeling results. The `CAD/` folder contains individual part files and the full assembly.

### 4. Gallery
The `Gallery/` folder contains miscellaneous project visuals including simulation plots, design iterations, and reference images.
<p align="center">
  <img src="Gallery/Screenshot 2026-03-31 001319.png" width="45%" alt="FEMM Magnetic Field Topology"/>
  &nbsp;&nbsp;
  <img src="Gallery/WhatsApp Image 2026-03-14 at 23.33.11.jpeg" width="45%" alt="SolidWorks Section View"/>
</p>
<p align="center">
  <em>Left: FEMM 2D axisymmetric magnetic field topology near channel exit &nbsp;|&nbsp; Right: SolidWorks section view of thruster assembly</em>
</p>

<p align="center">
  <img src="Gallery/WhatsApp Image 2026-03-06 at 12.50.04.jpeg" width="45%" alt="Isometric CAD View"/>
  &nbsp;&nbsp;
  <img src="Gallery/Screenshot 2026-04-10 111342.png" width="45%" alt="Channel Length vs Magnetic Field Strength"/>
</p>
<p align="center">
  <em>Left: Isometric external view of thruster assembly &nbsp;|&nbsp; Right: Channel length vs magnetic field strength regression</em>
</p>
---

## Tools Used

| Tool | Purpose |
|------|---------|
| FEMM | Magnetostatic finite element analysis |
| SolidWorks | 3D part and assembly modeling |
| Microsoft Excel | Scaling law calculations |

---

## Results & Key Findings

### Scaling Output — Channel Geometry

A regression-based scaling approach derived from a compiled dataset of 18 low-power Xenon Hall Effect Thrusters was applied to the target operating point of **200 W** and **250 V**. The procedure yielded the following discharge channel dimensions:

| Parameter | Value |
|-----------|-------|
| Mean channel diameter | 38 – 40 mm |
| Channel length | 19 – 21 mm |
| Channel width (height) | ~9 mm |
| Discharge voltage | 250 V |
| Discharge power | 200 W |
| Propellant | Xenon (SPT-type) |

These dimensions place the thruster within the geometric range of compact low-power Xenon HETs, consistent with the SPT-50M and KHT-50 class devices used as reference configurations in the scaling dataset.

### Magnetic Circuit — FEMM Results

A 2D axisymmetric FEMM simulation was used to develop and refine the magnetic circuit. The circuit used an AISI 1020 soft magnetic steel core with inner and outer poles arranged to concentrate the radial magnetic field near the channel exit — the region where electron confinement and Hall current formation are most critical for stable discharge. The design ensured:

- Radial magnetic field concentrated near the channel exit plane
- Inner pole operating below saturation threshold (verified against the AISI 1020 B-H curve)
- Electron Larmor radius much smaller than the channel length (re ≪ L)
- Ion Larmor radius large enough to allow axial acceleration without premature wall contact (ri ≫ L)

### CAD Design — Representative Model

A SolidWorks assembly was developed to verify that all thruster components could be integrated within the 200 W class envelope. Key material selections:

| Component | Material |
|-----------|----------|
| Discharge channel | Boron Nitride (BN) |
| Magnetic core & poles | AISI 1020 soft magnetic steel |
| Structural base plate | Aluminium |
| Electromagnet windings | Copper (0.8 mm diameter) |

### Predicted Performance

Theoretical performance was estimated from the finalised geometry using scaling relations from Lee et al. (2019):

| Parameter | Value |
|-----------|-------|
| Anode mass flow rate | 1.08 mg/s |
| Thrust force | 15.24 mN |
| Specific impulse (Isp) | 1440.28 s |

> **Note:** These are theoretical estimates derived from empirical scaling relations and have not yet been experimentally validated. The design is intended as a preliminary baseline for future fabrication and vacuum testing.

---

## Key References

This project draws heavily from the following works. A complete reference list of all 116 sources is in [`REFERENCES.md`](./REFERENCES.md).

**Primary methodology reference:**
> Mahajan, B., Troise, L., Giannetti, V., Ferrato, E., & Andreussi, T. (2025). *Development of a 500W-class high-voltage argon-fed Hall thruster.* Journal of Electric Propulsion.

**Scaling laws & design:**
> Dannenmayer, K., & Mazouffre, S. (2008). *Sizing of Hall Effect Thrusters with Input Power and Thrust Level: An Empirical Approach.*

> Shagayda, A. A., & Gorshkov, O. A. (2013). *Hall-thruster scaling laws.* Journal of Propulsion and Power, 29(2), 466–474. https://doi.org/10.2514/1.B34650

> Andrenucci, M., Battista, F., & Piliero, P. *Hall Thruster Scaling Methodology.*

**Foundational textbook:**
> Goebel, D. M., & Katz, I. *Fundamentals of Electric Propulsion: Ion and Hall Thrusters.* JPL Space Science and Technology Series.

---

## Related Publications

### Review Paper — *Published Preprint*
**Review of Electric Propulsion Technologies with Emphasis on Hall Effect Thruster for Satellite Operations**
Ayushmaan Badola, Drishya Sarilla
*Engineering Archive (engrXiv), April 2026*
🔗 [https://doi.org/10.31224/6806](https://doi.org/10.31224/6806)

A comparative review of five electric propulsion technologies — PPTs, Electrospray Thrusters, Gridded Ion Engines, Vacuum-Arc Thrusters, and Hall Effect Thrusters — evaluated across thrust-to-power ratio, specific impulse, system complexity, and flight heritage. Establishes HETs as the most viable baseline technology for small satellite propulsion.

---

### Research Manuscript — *Under Peer Review*
An original research manuscript based on this design project has been submitted to the **Journal of Engineering and Applied Sciences, Springer Nature**, and is currently under peer review.

---

## References & Resources

A complete list of all 116 papers, textbooks, and resources used throughout this project is available in [`REFERENCES.md`](./REFERENCES.md).

> The full reference library (~800MB of PDFs) could not be hosted here due to file size. The reference list links to original sources and DOIs wherever available.

---

## Author

**Ayushmaan Badola**
