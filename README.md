# Hybrid Solar–Diesel–Battery Energy Optimization Dashboard for Nigerian Households

A data-driven renewable energy analytics project that models and evaluates the technical, economic, and environmental performance of a hybrid solar photovoltaic (PV), diesel generator, and battery energy storage system for residential electricity supply in Nigeria.

The project combines Python for energy system modelling and Power BI for interactive dashboard visualization to demonstrate how hybrid renewable energy systems can reduce diesel consumption, lower carbon emissions, improve battery utilization, and support sustainable household electrification.


## Project Overview

Reliable electricity remains a major challenge in many Nigerian communities, resulting in widespread dependence on diesel generators for residential power supply. While diesel generators provide backup electricity, they are associated with high operating costs, fuel price volatility, greenhouse gas emissions, and environmental pollution.

This project investigates the integration of solar photovoltaic (PV) generation, diesel backup generation, and battery energy storage into a hybrid energy system designed for Nigerian households. Using solar irradiation data obtained from the NASA POWER database, the system simulates daily energy production, battery charging and discharging, diesel generator operation, and overall system performance throughout the year.

The simulation results are analysed using Python and visualized through an interactive Power BI dashboard that presents key performance indicators (KPIs), monthly trends, economic metrics, environmental benefits, and battery performance.

The project demonstrates how renewable energy analytics can support evidence-based decision-making for sustainable energy planning.


## Project Objectives

The primary objective of this project is to evaluate the performance of a hybrid solar PV–diesel–battery energy system for residential electricity supply in Nigeria using data-driven simulation and interactive visualization.

Specific objectives include:

- Develop a hybrid energy system model using Python.
- Simulate daily solar energy generation using NASA POWER solar irradiation data.
- Estimate household electricity demand and compare it with renewable energy generation.
- Model battery charging and discharging behaviour throughout the year.
- Determine the amount of diesel energy required to meet unmet electricity demand.
- Evaluate battery utilization and system reliability.
- Estimate the economic benefits of reducing diesel generator usage.
- Quantify the environmental benefits through reduced diesel consumption and CO₂ emissions.
- Design an interactive Power BI dashboard for monitoring technical, economic, environmental, and battery performance indicators.


## Research Questions

This project seeks to answer the following questions:

1. How much household electricity demand can be supplied using solar photovoltaic energy?

2. To what extent can battery storage reduce dependence on diesel generators?

3. What are the annual diesel fuel savings achieved by integrating battery storage?

4. How much carbon dioxide (CO₂) emission can be avoided through hybrid renewable energy adoption?

5. What economic benefits can households obtain from reduced diesel consumption?

6. How can interactive dashboards improve the monitoring and interpretation of hybrid energy system performance?


## Project Features

This project includes the following features:

- Solar photovoltaic energy simulation
- Battery State of Charge (SOC) modelling
- Battery charging and discharging analysis
- Diesel generator optimization
- Monthly energy demand analysis
- Energy deficit assessment
- Diesel fuel consumption estimation
- Diesel cost comparison
- CO₂ emission estimation
- CO₂ reduction analysis
- Solar energy contribution assessment
- Battery utilization analysis
- Interactive Power BI dashboards
- Executive summary dashboard
- Economic analysis dashboard
- Environmental analysis dashboard
- Battery performance dashboard


## Technology Stack

| Technology | Purpose |
|------------|---------|
| Python | Data processing and hybrid energy simulation |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical computation |
| Matplotlib | Data visualization during analysis |
| Jupyter Notebook | Model development and experimentation |
| Power BI | Interactive dashboard development |
| NASA POWER API | Solar irradiation dataset |
| Git | Version control |
| GitHub | Project hosting and collaboration |


## Project Architecture

The project follows the workflow below:

NASA POWER Solar Data

↓

Python Data Processing

↓

Hybrid Energy System Simulation

↓

Battery Charging & Discharging Model

↓

Diesel Generator Optimization

↓

Economic Analysis

↓

Environmental Analysis

↓

CSV Output Dataset

↓

Power BI Dashboard Development

↓

Interactive Decision Support Dashboard


## Dataset

The analysis uses daily solar radiation data obtained from the NASA POWER database for Abuja, Nigeria.

**Dataset Information**

- Source: NASA POWER
- Location: Abuja, Nigeria
- Year: 2025
- Temporal Resolution: Daily
- Main Variable: ALLSKY_SFC_SW_DWN (Daily Solar Irradiance)

Additional variables generated during the simulation include:

- Solar_Output
- Load_kWh
- Battery_SOC
- Battery_Discharge
- Diesel_Liters
- Diesel_Cost_2025
- Diesel_Cost_2026
- Energy_Gap
- Excess_Solar
- Month