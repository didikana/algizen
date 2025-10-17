[README_ALGi-zen.md](https://github.com/user-attachments/files/22978206/README_ALGi-zen.md)
# 🧪 ALGi-zen: Computational Modeling of Algae-Based Façade Systems  

**Author:** Doğukan Arısan  
**Languages:** Python, MATLAB, C  
**Lines of Code:** ~12,000  
**Status:** Research prototype recognized by TÜBİTAK (3rd Place, National Research Project Competition – Chemistry Category)

## 🌱 Overview  

**ALGi-zen** is a computational sustainability project that models microalgae-based façade panels for **carbon capture** and **biostimulant reuse**.  
The system simulates **photosynthetic efficiency**, **CO₂ absorption**, and **light diffusion** using **coupled differential equations** and **real-time sensor feedback** from a custom photoreactor.

The main objective is to determine **optimal algae replacement intervals** that maximize CO₂ sequestration while minimizing energy and nutrient costs.

## ⚙️ Core Features  

- **Differential Equation Solver:** Simulates biomass growth and CO₂ uptake using Runge–Kutta and Euler integration methods.  
- **Photoreactor Simulation:** Interfaces with sensors (light, pH, temperature) through a C-based embedded controller.  
- **Optimization Engine:** Uses nonlinear curve fitting and gradient-based optimization to identify high-efficiency growth cycles.  
- **Visualization Tools:** Provides time-series plots of CO₂ concentration, photosynthetic rate, and spectral absorption.  
- **Data Interface:** Connects Python modules with embedded C control systems via serial communication.

## 🧮 Mathematical Model  

The system models both CO₂ concentration and photosynthetic biomass over time as:

$$
\frac{dC}{dt} = -k_1 P(t) A + D(C_{\text{in}} - C)
$$

$$
\frac{dP}{dt} = k_2 I(t)\left(1 - \frac{P}{P_{\text{max}}}\right) - k_3 P
$$

Where:  
- \(C\): CO₂ concentration (ppm)  
- \(P\): Photosynthetic biomass density (g/L)  
- \(I(t)\): Light intensity (W/m²)  
- \(A\): Effective surface area of the façade (m²)  
- \(k_1, k_2, k_3\): Empirical growth constants  
- \(D\): Diffusion rate constant  
- \(C_{\text{in}}\): Ambient CO₂ concentration  

## 🖥 Architecture  

**Key Directories**  
- `src/simulation.py` – Implements the differential equation solvers  
- `src/optimization.py` – Handles nonlinear optimization and curve fitting  
- `src/visualization.py` – Generates dynamic plots and heatmaps  
- `src/photoreactor.c` – Controls embedded sensors and actuators  
- `data/` – Stores calibration curves and experimental logs  
- `notebooks/algi_analysis.ipynb` – Interactive data analysis  

## 📈 Example Outputs  

- Predicted vs. experimental CO₂ absorption cycles  
- Photosynthetic rate curves across varying light intensities  
- Efficiency heatmaps over time and nutrient levels  

## 🧩 Impact  

- Demonstrated measurable CO₂ capture efficiency in prototype façades  
- Integrated environmental chemistry, differential modeling, and software automation  
- Recognized nationally by TÜBİTAK for innovation in sustainable material design  

## 📜 Citation  

**Arısan, D. (2024).** *ALGi-zen: Computational Optimization of Algae-Based Carbon Capture Systems.* TÜBİTAK High School Research Project Competition.
