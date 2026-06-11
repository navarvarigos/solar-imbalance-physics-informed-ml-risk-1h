# Solar-Imbalance-Physics-ML: Cloud-Ramp Risk Forecasting

This repository contains a Colab-ready notebook for a physics-informed solar PV forecasting project focused on imbalance-risk analytics.

## What the project does

- Forecasts PV generation 15 minutes ahead and 1 hour ahead.
- Compares persistence, standard ML and physics-informed ML.
- Shows that 15-minute forecasts are strongly persistence-driven.
- Adds a 1-hour horizon to study when persistence weakens.
- Defines large negative PV ramps as risk events.
- Translates forecast errors into scenario-based imbalance-cost exposure.

## Dataset

Download:
https://www.kaggle.com/datasets/cdaclab/unisolar?resource=download

The notebook expects the UNISOLAR/Kaggle files:

- `Solar_Energy_Generation.csv`
- `Weather_Data_reordered_all.csv`
- `Solar_Site_Details.csv`

Place the required dataset files inside the 'data/' directory before executing the notebook.

## Transparency note

The dataset includes PV output and weather data, but not measured irradiance or plant-level market settlement prices. Physics-informed features are therefore proxy features, and imbalance costs are scenario-based estimates rather than exact realised settlement costs.
