# Airline Passenger Demand Forecasting

This repository contains an academic project completed at **Boston University** focused on forecasting airline passenger demand using machine learning and time-series analysis for BA810: Supervised Machine Learning course .

## Project Overview

The objective of this project was to forecast monthly **Revenue Passenger Miles (RPM)** for the U.S. domestic airline market, a key metric representing airline demand and economic activity.

RPM is calculated as:
Passenger Miles = Paying Passengers × Distance Flown

We built predictive models to estimate future demand and generate insights for operational and business decision-making.

## Business Context

Accurate demand forecasting is critical for:

- Capacity planning (fleet allocation and route management)
- Revenue optimization (dynamic pricing strategies)
- Operational efficiency (staffing and airport resource planning)

## Dataset

- Source: U.S. DOT BTS T-100 Domestic Segment dataset
- Time range: 2022–2025 (partial 2025)
- Final dataset: ~26,000 rows and 37 features :contentReference[oaicite:0]{index=0}

## Methodology

### Data Processing
- Cleaned and standardized raw data
- Removed irrelevant variables (cargo, mail)
- Eliminated data leakage features
- Engineered features capturing seasonality and capacity trends

### Exploratory Data Analysis
Key insights included:
- Strong seasonality with peak demand in summer months
- Dominance of major carriers (WN, AA, DL, UA)
- Consistent yearly demand patterns :contentReference[oaicite:1]{index=1}

### Modeling Approach
Implemented and compared multiple models:

- Linear Regression
- Ridge Regression
- Decision Trees
- Random Forest
- Support Vector Regression (SVR)
- Stacking Regressor

### Model Performance

- Linear models achieved strong performance (R² ≈ 0.997)
- Random Forest captured nonlinear relationships effectively
- Best performance achieved using **Stacking Regressor** combining linear and ensemble models :contentReference[oaicite:2]{index=2}

## Key Findings

- Passenger demand is highly predictable due to strong linear relationships with capacity variables
- Seasonal trends play a significant role in demand fluctuations
- Ensemble models improve robustness but linear models already provide near-optimal performance

## Business Insights

- Improved capacity planning through accurate demand forecasting
- Enhanced pricing strategies based on seasonal demand trends
- Reduced operational inefficiencies by minimizing underutilized capacity :contentReference[oaicite:3]{index=3}

## Files in This Repository

- `Airline_Passenger_Demand_Forecasting.ipynb` — full data analysis and modeling
- `README.md` — project overview

## Academic Context

This project was completed as part of a graduate-level analytics course at **Boston University**.

## Team Members

- Kaixin Gao  
- Kang Ni  
- Shanmathi Sivakumar  
- Mike Allieri

## Tools Used

- Python  
- pandas  
- NumPy  
- scikit-learn  
- matplotlib / seaborn  
