# Forecasting Under-5-Mortality-Rate in Kenya
### _U5MR Forecast_

## Overview

The U5MR Forecast project aims to analyze and forecast under-five mortality rates (U5MR) using statistical models. This project utilizes the Lee-Carter model and the CBD (Cohort-Based Decomposition) model to estimate mortality rates for different age groups.

## Project Structure

The project includes the following components:
- **Data Processing**: Filtering and preparing data for analysis.
- **Modeling**: Applying the Lee-Carter and CBD models to the filtered data.
- **Results**: Storing and presenting the results of the analyses.

## Code Explanation

The main script processes infant and under-five mortality data over specified lookback windows. The key steps are:

1. **Filtering Data**: The data is filtered based on the year range specified in `lookback_windows`.
2. **Applying Models**:
   - For the 0-1 age group (infants):
     - **Lee-Carter Model**: Estimates mortality parameters.
     - **CBD Model**: Provides additional mortality estimates.
   - For the 1-4 age group (children under five):
     - Similar modeling steps are applied.
3. **Handling Missing Data**: If no data is available for a specific year range, NaN values are assigned to the results.
4. **Storing Results**: The results are collected in a list for further analysis or visualization.

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





