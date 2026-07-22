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


## Mathematical Model

The hybrid energy system was modelled using a rule-based energy management approach that prioritizes solar photovoltaic (PV) generation, followed by battery storage, and finally diesel generation whenever renewable energy is insufficient to satisfy the household load.

The model follows these steps for each day of the simulation:

1. Estimate solar energy generation from daily solar irradiance.
2. Compare the generated solar energy with the household electricity demand.
3. Supply the load directly from solar energy whenever available.
4. Store excess solar energy in the battery until the battery reaches its maximum capacity.
5. When solar energy is insufficient, discharge the battery to supply the remaining load.
6. If the battery becomes depleted, use the diesel generator to satisfy the remaining electricity demand.

The following equations were applied during the simulation.

### Solar Energy Output

Solar Output = Solar Irradiance × System Size × System Efficiency

### Energy Gap

Energy Gap = Load − Solar Output

### Battery Charging

Battery SOC = Previous SOC + Excess Solar

where Battery SOC cannot exceed the battery capacity.

### Battery Discharging

Battery Discharge = Minimum (Battery SOC, Energy Gap)

### Diesel Energy Requirement

Diesel Required = Maximum (Energy Gap − Battery Discharge, 0)

This sequential energy management strategy minimizes diesel generator operation while maximizing the utilization of renewable energy and battery storage.


## Dashboard Overview

The simulation results were visualized using Microsoft Power BI through an interactive dashboard consisting of four analytical pages.

### Executive Dashboard

Provides a high-level summary of the hybrid energy system using Key Performance Indicators (KPIs), monthly trends, and interactive filtering.

Key indicators include:

- Solar Generation
- Energy Demand
- Battery Output
- Diesel Output
- Diesel Required
- Average Battery SOC
- Maximum Battery SOC



### Economic Dashboard

Evaluates the financial performance of the hybrid energy system through:

- Diesel Cost
- Battery Investment Cost
- Cost Savings
- Payback Analysis



### Environmental Dashboard

Measures environmental sustainability using:

- CO₂ Emissions
- CO₂ Reduction
- Solar Energy Contribution
- Diesel Reduction



### Battery Performance Dashboard

Monitors battery behaviour throughout the simulation period, including:

- Battery State of Charge (SOC)
- Battery Charging
- Battery Discharging
- Battery Utilization
- Remaining Energy Gap


## Results & Discussion

The simulation demonstrates the effectiveness of integrating solar photovoltaic generation with battery storage to reduce dependence on diesel generators for residential electricity supply.

Key findings include:

- Solar PV supplied the majority of the annual household energy demand.
- The battery successfully stored excess solar energy during high-generation periods and supplied electricity during periods of insufficient solar production.
- Diesel generator usage decreased significantly after battery integration.
- Increasing battery capacity reduced diesel energy requirements, although the rate of improvement decreased at higher battery capacities.
- Environmental analysis showed a reduction in diesel-related carbon dioxide (CO₂) emissions.
- Economic analysis indicated that although larger batteries require higher initial investment, they contribute to long-term reductions in diesel operating costs.

The interactive Power BI dashboard provides decision-makers with an intuitive platform for monitoring technical performance, economic benefits, and environmental impacts of hybrid renewable energy systems.


## Repository Structure

```text
Hybrid-Solar-Diesel-Battery-Optimization/

├── Data/                  # Input and processed datasets
├── notebooks/             # Jupyter Notebook analysis
├── scripts/               # Python scripts
├── powerbi/               # Power BI dashboard
├── outputs/               # Simulation outputs
├── images/                # Dashboard screenshots
├── docs/                  # Project documentation
├── README.md
├── requirements.txt
└── LICENSE
```


## Installation Guide

Clone the repository:

```bash
git clone https://github.com/Innocentaniekan/Hybrid-Solar-Diesel-Battery-Optimization.git
```

Navigate to the project folder:

```bash
cd Hybrid-Solar-Diesel-Battery-Optimization
```

Install the required Python libraries:

```bash
pip install -r requirements.txt
```

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Launch the notebook located in the `notebooks` folder and run the cells sequentially to reproduce the analysis.

The Power BI dashboard can be opened using Microsoft Power BI Desktop.


## Future Improvements

Potential future enhancements include:

- Integration of real-time weather data.
- Machine learning models for solar energy forecasting.
- Electricity demand forecasting using historical consumption data.
- Battery degradation modelling.
- Multi-objective optimization of cost, reliability, and emissions.
- Web-based dashboard deployment.
- Integration with IoT-enabled smart energy systems.


## About the Author

**Innocent Aniekan**

Mechanical Engineering Technologist with interests in renewable energy systems, hybrid power systems, energy analytics, data visualization, and sustainable development.

This project demonstrates practical experience in:

- Python Programming
- Data Analysis
- Renewable Energy Modelling
- Battery Energy Storage Systems
- Power BI Dashboard Development
- Git & GitHub


## License

This project is distributed under the MIT License.

See the LICENSE file for additional information.