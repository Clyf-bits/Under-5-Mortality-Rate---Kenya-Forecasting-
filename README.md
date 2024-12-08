# [ONGOING] Forecasting Under-5-Mortality-Rate in Kenya
### _U5MR Forecast_

## Overview

The U5MR Forecast project aims to analyze and forecast under-five mortality rates (U5MR) using statistical models. This project utilizes the Lee-Carter model and the CBD (Cohort-Based Decomposition) model to estimate mortality rates for different age groups.

## Objectives

- To estimate and forecast U5MR for different age groups (0-1 years and 1-4 years).
- To analyze historical mortality data and identify trends over specified time windows.
- To provide a framework for understanding the factors influencing mortality rates in early childhood.

## Project Structure

The project includes the following components:
- **Data Processing**: Filtering and preparing data for analysis. Preparing data for infants and children under five from `infant_totals` and `u5mr_totals`.
- **Statistical Modeling**:
  - **Lee-Carter Model**: A widely used model for forecasting mortality rates, which captures the underlying trends and fluctuations in mortality data.
  - **Cohort-Based Decomposition Model**: A model that further analyzes mortality rates by breaking down the data into cohorts, providing additional insights.
- **Results Compilation**: The results of the models are compiled into a structured format for easy analysis and visualization.

## Code Explanation

The main script processes infant and under-five mortality data over specified lookback windows. The key steps are:

1. **Filtering Data**: The data is filtered based on the year range specified in `lookback_windows`.
2. **Applying Models**:
   - For the 0-1 age group (infants):
     - **Lee-Carter Model**: Estimates mortality parameters.
     - **CBD Model**: Provides additional mortality estimates for model comparison.
   - For the 1-4 age group (children under five):
     - Similar modeling steps are applied.
3. **Storing Results**: The results are collected in a list for further analysis or visualization.

## Requirements

To run this project, you need:
- Python 3.x
- Required libraries:
  - `numpy`
  - `pandas`
  - `sklearn`
  - `matplotlib`

## Usage

1. Clone the repository:
```bash
git clone https://github.com/Clyf-bits/U5MR-Forecast.git
cd U5MR-Forecast
```
2. Install required libraries:

```bash
pip install numpy
pip install pandas
pip install sklearn
pip install matplotlib
```
3. Run the main script:
```bash
python U5MR_Forecast.py
```





