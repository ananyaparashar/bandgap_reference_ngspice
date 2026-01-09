# bandgap_reference_ngspice
CMOS Bandgap Reference Circuit – NGSPICE simulation and Python-based performance analysis
 # CMOS Bandgap Reference Circuit – NGSPICE & Python Analysis

This repository contains the design, simulation, and performance analysis of a CMOS bandgap reference circuit implemented using **NGSPICE** and **Python**.

## Overview
The bandgap reference generates a stable voltage (~1.23–1.25 V) independent of temperature and supply variations. Such circuits are fundamental building blocks in voltage regulators, data converters, and power management ICs.

## Tools Used
- **NGSPICE** – DC, transient, AC, temperature sweep, and PSRR simulations
- **Python (NumPy, Matplotlib)** – Data extraction, analysis, and visualization
- **Analog IC Design Theory** – PTAT & CTAT voltage cancellation

## Circuit Architecture
- BJT pair with area ratio (1:8) for PTAT voltage generation  
- Op-amp feedback to equalize branch currents  
- PMOS current mirror  
- Resistor network to generate final reference voltage  

## Key Performance Metrics
| Parameter | Value |
|---------|------|
| Reference Voltage | 1.23–1.25 V |
| Temperature Coefficient | 38.69 ppm/°C |
| Line Regulation | 6.5 mV/V |
| Startup Settling Time | 230.52 µs |
| PSRR | 80 dB (DC & 1 MHz) |

## Simulation Results
- Temperature stability from -20°C to 100°C  
- Line regulation across supply variations  
- Fast startup transient response  
- Strong PSRR across frequency  

## Repository Structure
- `ngspice/` – Circuit netlists and device models  
- `python/` – Post-processing and plotting scripts  
- `results/` – Generated plots and figures  
- `report/` – Detailed simulation report  

## Author
**Ananya Parashar**  
B.Tech Electronics and Communication Engineering  
Manipal Institute of Technology
