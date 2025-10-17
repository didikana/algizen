# algizen
ALGi-zen: Computational Modeling of Algae-Based Façade Systems
Author: Doğukan Arısan
Languages: Python, MATLAB, C
Lines of Code: ~12,000
Status: Research prototype recognized by TÜBİTAK (3rd Place, National Research Project Competition – Chemistry Category)
Overview
ALGi-zen is a computational sustainability project that models microalgae-based façade panels for carbon capture and biostimulant reuse.
The system simulates photosynthetic efficiency, CO₂ absorption, and light diffusion using coupled differential equations and real-time sensor feedback from a custom photoreactor.
The main objective is to determine optimal algae replacement intervals that maximize CO₂ sequestration while minimizing energy and nutrient costs.
Core Features
Differential Equation Solver: Simulates biomass growth and CO₂ uptake using Runge–Kutta and Euler integration methods.
Photoreactor Simulation: Interfaces with sensors (light, pH, temperature) through a C-based embedded controller.
Optimization Engine: Uses nonlinear curve fitting and gradient-based optimization to identify high-efficiency growth cycles.
Visualization Tools: Provides time-series plots of CO₂ concentration, photosynthetic rate, and spectral absorption.
Data Interface: Connects Python modules with embedded C control systems via serial communication.

​
Computer Architecture
Key Directories
src/simulation.py – Implements the differential equation solvers
src/optimization.py – Handles nonlinear optimization and curve fitting
src/visualization.py – Generates dynamic plots and heatmaps
src/photoreactor.c – Controls embedded sensors and actuators
data/ – Stores calibration curves and experimental logs
notebooks/algi_analysis.ipynb – Interactive data analysis
Example Outputs
Predicted vs. experimental CO₂ absorption cycles
Photosynthetic rate curves across varying light intensities
Efficiency heatmaps over time and nutrient levels
mpact
Demonstrated measurable CO₂ capture efficiency in prototype façades
Integrated environmental chemistry, differential modeling, and software automation
Recognized nationally by TÜBİTAK for innovation in sustainable material design
