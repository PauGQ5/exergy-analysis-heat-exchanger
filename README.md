# exergy-analysis-heat-exchanger

# Thermal Performance and Exergy Analysis of a Sensible Heat Exchanger

## Overview
This project is a Python-based simulation that evaluates the thermal performance and thermodynamic inefficiencies of a sensible heat exchanger over a 720-hour (1 month) operational period. The model analyzes how variations in fluid flow rates impact the system's efficiency and calculates the corresponding exergy destruction.

## Thermodynamic Model
The simulation applies foundational energy and exergy balance equations. For the purpose of this model, it is assumed that the heat capacity rates of both the hot and cold fluids are equal ($C_h = C_c$).

The exergy destruction ($E_d$) during the heat transfer process is calculated using the following equation, with a reference environment temperature ($T_0$) of 298.15 K:

$$ E_d = T_0 \cdot \left[ \ln\left(\frac{T_{h,out}}{T_{h,in}}\right) + \ln\left(\frac{T_{c,out}}{T_{c,in}}\right) \right] $$

## Technologies Used
* **Python 3:** Core programming language.
* **Pandas:** For time-series data generation and structured data manipulation.
* **NumPy:** For vectorization and mathematical operations (e.g., natural logarithms).
* **Matplotlib:** For rendering high-quality data visualizations.

## Results & Conclusions

![Thermal Analysis Graphs](analisis_termico_graficas.png)

The visualizations reveal two main operational insights:
1. **Dynamic Response:** The cold fluid's outlet temperature continuously tracks the input fluctuations of the hot fluid.
2. **Exergy Destruction Trend:** There is a clear, positive correlation between the fluid flow rate and thermodynamic inefficiency. As the flow rate increases (L/min), the system experiences higher exergy destruction. This highlights a crucial engineering trade-off between operational throughput and the conservation of energy quality.

## Transparency Note
The core thermodynamic design, mathematical modeling, and data interpretation in this repository are my original work. AI-assisted tools were utilized strictly to accelerate Python syntax generation and optimize the Matplotlib graphical rendering.
