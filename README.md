![Hall Effect Thruster — Magnetic Field Model](Banner Asset/Screenshot 2026-03-31 001319.png)
[README.md](https://github.com/user-attachments/files/28595937/README.md)
# Hall Effect Thruster (HET) — Research & Design Project

Scaling analysis, magnetostatic modeling, and CAD design of a Hall Effect Thruster, with an accompanying research manuscript currently under peer review at the **Journal of Engineering and Applied Sciences, Springer Nature**.

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

---

## Tools Used

| Tool | Purpose |
|------|---------|
| FEMM | Magnetostatic finite element analysis |
| SolidWorks | 3D part and assembly modeling |
| Microsoft Excel | Scaling law calculations |

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
