# EV Charging Demand Forecasting and Optimal Energy Management

## Project Overview

This project focuses on analysing Electric Vehicle (EV) charging demand, forecasting future charging loads using machine learning, and optimizing EV charging schedules to reduce peak station demand.

The project uses the **ACN-Data Caltech Garage dataset** and applies data preprocessing, exploratory data analysis, machine learning forecasting, and Linear Programming-based optimization.

## Objectives

- Analyse historical EV charging patterns.
- Reconstruct charging demand at 15-minute intervals.
- Develop machine learning models for EV charging demand forecasting.
- Compare Random Forest, XGBoost, and two-stage XGBoost models.
- Investigate optimized EV charging schedules.
- Evaluate the potential reduction in peak station demand.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas and NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- SciPy
- Linear Programming

## Dataset

The project uses the ACN-Data dataset collected from the Caltech Garage charging station.

Dataset source: https://ev.caltech.edu/dataset

## Forecasting Models

The following models were evaluated:

| Model | Forecasting MAE |
|---|---:|
| Random Forest (15 min) | 0.615 kW |
| XGBoost (15 min) | 0.581 kW |
| Two-stage XGBoost (15 min) | 0.543 kW |

The two-stage XGBoost model achieved the lowest 15-minute MAE among the evaluated models.

## Optimization Results

A Linear Programming-based charging optimization approach was evaluated using four case studies.

- September 20: 52.91% peak demand reduction
- October 19: 2.52% peak demand reduction
- October 30: 0% peak demand reduction
- December 1: 0% peak demand reduction

The results demonstrate that charging flexibility and background demand influence the effectiveness of optimized charging.

## Project Structure

- `EV_Load_Demand_Analysis.ipynb` – Main project notebook
- `data/` – Dataset and processed files
- `results/` – Forecasting and optimization results
- `figures/` – Generated graphs and visualizations

## Future Scope

- Real-time EV charging demand forecasting
- Weekly and monthly demand prediction
- Renewable energy integration
- Battery energy storage integration
- Dynamic electricity pricing
- Practical charging station implementation

## Author

**Mohammed Suheyl**
**Kavide Vijay Bhargav**
**Vankdoth Karthik**
**Nematuri Ramcharan**

B.Tech – Electrical and Electronics Engineering  
Anurag University, Hyderabad  
Academic Year: 2026–2027

## Acknowledgement

This project uses the ACN-Data open EV charging dataset for academic research and analysis.
