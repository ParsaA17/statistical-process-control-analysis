# Statistical Process Control (SPC) & Process Capability Analysis

## Project Overview
This project implements Statistical Process Control (SPC) techniques to monitor a precision manufacturing process (shaft diameter, nominal target: 50.00 mm). The study evaluates process stability over time using control charts and assesses capability against engineering specifications.

## Sampling Plan & Specifications
- **Target Dimension:** 50.00 mm
- **Engineering Tolerances:** USL = 50.15 mm, LSL = 49.85 mm
- **Subgroups:** 20 rational subgroups (sample size $n = 5$ per subgroup)

## Control Chart Parameters & Formulations
- **Grand Mean ($\bar{\bar{X}}$):** 50.011 mm
- **Average Range ($\bar{R}$):** 0.047 mm
- **$\bar{X}$-Chart Control Limits ($A_2 = 0.577$):**
  - $\text{UCL}_{\bar{X}} = \bar{\bar{X}} + A_2 \bar{R} = 50.038\text{ mm}$
  - $\text{CL}_{\bar{X}} = 50.011\text{ mm}$
  - $\text{LCL}_{\bar{X}} = \bar{\bar{X}} - A_2 \bar{R} = 49.984\text{ mm}$
- **$R$-Chart Control Limits ($D_3 = 0, D_4 = 2.114$):**
  - $\text{UCL}_R = D_4 \bar{R} = 0.099\text{ mm}$
  - $\text{CL}_R = 0.047\text{ mm}$
  - $\text{LCL}_R = D_3 \bar{R} = 0.000\text{ mm}$

## Process Capability Analysis
- **Estimated Standard Deviation ($\hat{\sigma} = \bar{R} / d_2$):** 0.0202 mm ($d_2 = 2.326$)
- **Potential Capability ($C_p$):** 2.47
- **Actual Capability ($C_{pk}$):** 2.30

## Key Findings & Conclusions
- **Statistical Control:** All 20 subgroup means and ranges fall strictly within the 3-sigma control limits, indicating a stable process driven solely by common cause variation.
- **Process Capability:** With a $C_{pk} > 2.0$, the process exceeds the Six Sigma capability benchmark, confirming near-zero expected defect rates against design limits.

## Tools Used
- Microsoft Excel (Statistical Modeling, Line Charts, Capability Index Formulation)
