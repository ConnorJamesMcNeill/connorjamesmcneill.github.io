---
title: EV Porsche 356 | Motor Mount FEA
date: 2024-03-10 12:00:00 -0700
categories: [Work Experience, EV Underground Inc.]
tags: [solid_mechanics, failure_analysis, material_science, automotive_engineering, problem-solving]

image:
  path: /assets/img/Work Experience/EVU/Simulation/Screenshot 2024-03-10 221656.png
  alt: SolidWorks FEA factor of safety plot on the 356 rear end mount assembly
---

### The chassis bracket for the Tesla drive unit mount is the primary structural interface between the tube frame cradle and the 356 body. It carries the full weight of the drive unit plus road-induced dynamic loading, transferred into the original chassis pickup points. Before anything went to fabrication, the design needed to be validated. I ran FEA in SolidWorks Simulation across three design iterations to confirm adequate factor of safety and identify any stress concentrations worth addressing. The bracket is 11ga A1008 cold rolled steel, with a yield strength of approximately 247 MPa and UTS of 340 MPa. The peak torque load case was 4,000 Nm at the wheel, consistent with the Tesla SDU's ~430 Nm motor output stepped through its 9.73:1 gearbox.

### The study progressed from the original geometry through Rev A and Rev B. Each revision was assessed for both stress distribution and mass, tracking that weight did not creep up as geometry was modified to address high-stress regions. The final Rev B assembly came in at 2,729g versus 2,679g for the original, a marginal mass increase for meaningfully better stress distribution across the part.

#### The original design under load. The simulation flagged elevated stress at a few of the cutout regions and the lower mounting tab geometry.

![SolidWorks FEA strain map on original rear end mount design showing stress concentrations](/assets/img/Work Experience/EVU/Simulation/Screenshot 2024-03-10 220034.png){: width="100%" }

<br>

#### Mass properties of the original rear end mount. 2,679g at 0.01 g/mm³ density, used as the baseline for subsequent revisions.

![SolidWorks mass properties panel for original rear end mount showing 2679g mass](/assets/img/Work Experience/EVU/Simulation/Screenshot 2024-03-10 215636.png){: width="100%" }

<br>

#### Rev A single part FEA. The geometry changes brought stress down significantly across most of the part, with only minor concentration remaining at one cutout.

![SolidWorks FEA strain map on Rev A rear end mount](/assets/img/Work Experience/EVU/Simulation/Screenshot 2024-03-10 213217.png){: width="100%" }

<br>

#### Rev A mass properties. 2,200g, a noticeable reduction from the original while improving the structural result.

![SolidWorks mass properties panel for Rev A showing 2200g mass](/assets/img/Work Experience/EVU/Simulation/Screenshot 2024-03-10 213547.png){: width="100%" }

<br>

#### Rev B assembly FEA. Running the full assembly simulation rather than just the isolated part gives a more realistic picture of how loads distribute through the joint.

![SolidWorks FEA strain map on Rev B rear end mount assembly](/assets/img/Work Experience/EVU/Simulation/Screenshot 2024-03-10 214348.png){: width="100%" }

<br>

#### Rev B assembly mass properties. 2,729g for the full assembly, a modest increase over Rev A reflecting the additional hardware in the assembly model.

![SolidWorks mass properties panel for Rev B assembly showing 2729g mass](/assets/img/Work Experience/EVU/Simulation/Screenshot 2024-03-10 213707.png){: width="100%" }

<br>

#### Rev B assembly FEA, alternate view. The stress distribution across the lower face is even and well within limits.

![SolidWorks FEA strain map on Rev B assembly from alternate angle](/assets/img/Work Experience/EVU/Simulation/Screenshot 2024-03-10 221656.png){: width="100%" }

<br>

#### Factor of safety plot on the Rev B assembly under peak torque loading (4000Nm). Minimum FOS sits comfortably above 3.0, confirming the design is adequate for fabrication.

![SolidWorks factor of safety plot on Rev B assembly showing FOS above 3.0](/assets/img/Work Experience/EVU/Simulation/Screenshot 2024-04-29 163354.png){: width="100%" }
