# HRIM-Swallow-Biomechanics
This repository contains MATLAB scripts developed for my UC San Diego Bioengineering Senior Design project analyzing high-resolution impedance manometry (HRIM) swallow data.  
The scripts demonstrate how raw impedance and pressure recordings can be transformed into quantitative biomechanical features for comparison across patients and swallow conditions.

## Overview

HRIM provides synchronized multichannel impedance and pressure signals along the esophagus.  
From these raw measurements, the analysis pipeline computes biomechanical features commonly used to evaluate swallow function, including:

- **Cross-sectional area (CSA)**
- **Tension (from impedance + pressure)**
- **CSA–tension loops**
- **Work** (integral of tension–CSA curve)
- **Modulus** (slope of tension–CSA)
- **Power**
- **Channel heatmaps** ( pressure/impedance visualization)

These steps convert noisy physiological measurements into interpretable summary metrics at the patient, condition, and swallow levels.

## Repository Contents

### `swallow_metrics_pipeline.mlx`
Main pipeline for processing HRIM swallow recordings.  
This script includes:

- Loading and organizing multichannel impedance/pressure data  
- Automated preprocessing and physiological baseline extraction  
- Computing CSA and tension from synchronized channels  
- Generating **CSA–tension loops**  
- Calculating **Work**, **Modulus**, and related metrics  
- Plotting **heatmaps** for multichannel spatiotemporal patterns  
- Saving per-patient and per-condition results

### `work_prepost_boxplot.mlx`
Generates group-level Work comparisons (e.g., channel 12) across  
**pre/post treatment** and  **10+ patients × 6 swallow conditions × 5 swallows per condition**.  
Outputs boxplots and summary statistics.

---

## Notes

- HRIM clinical recordings cannot be included due to privacy restrictions.  
- The scripts illustrate the analysis workflow, metric calculations, and visualization steps used in the project.

---

## Contact
If you have questions about this project, feel free to reach out.

