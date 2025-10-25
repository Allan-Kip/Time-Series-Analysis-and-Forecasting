# Time Series Analysis and Forecasting

## Project Overview
This project demonstrates how to perform **time series analysis and forecasting** using Python within the **Anaconda (Jupyter Notebook)** environment.  
It explores how time-dependent data behaves over time, detects trends and seasonality, and applies forecasting models to predict future values.

The project uses synthetic monthly sales data from **2018 to 2025** to simulate business performance and future projections.

---

## Project Structure
time_series_analysis_and_forecasting/
│
├── Time Series Analysis and Forecasting.ipynb # Main Jupyter Notebook
├── sales_data.csv # Generated dataset (2018–2025)
├── sales_forecast.csv # ARIMA forecast results
├── sarima_forecast.csv # SARIMA forecast results


---

## Tools and Libraries Used
- **Python 3.x**
- **Anaconda / Jupyter Notebook**
- **Pandas** – Data cleaning and manipulation  
- **NumPy** – Numerical computations  
- **Matplotlib** & **Seaborn** – Data visualization  
- **Statsmodels** – ARIMA & SARIMA modeling   

---

## Steps Performed

### Data Generation
A synthetic dataset was created with monthly sales from 2018–2025, incorporating:
- **Trend** – gradual increase over time  
- **Seasonality** – repeating annual patterns  
- **Noise** – random variations for realism  

Saved as `sales_data.csv`.

### Data Exploration
- Visualized the sales trend using line plots.  
- Checked for **stationarity** using the **Augmented Dickey-Fuller (ADF)** test.  
- Applied differencing when needed to stabilize the series.

### ARIMA Modeling
- Built an **ARIMA(1,1,1)** model to forecast future values.  
- Plotted the results and saved them to `sales_forecast.csv`.

### SARIMA Modeling
- Implemented a **SARIMA(1,1,1)(1,1,1,12)** model to account for **monthly seasonality**.  
- Generated forecasts and confidence intervals.  
- Saved results to `sarima_forecast.csv`.

### Model Comparison
- Visualized and compared ARIMA and SARIMA.  
- Observed that SARIMA handled seasonality best.

---

## Outputs
- **Line charts** showing overall sales trends.  
- **Forecast plots** displaying predicted future sales.  
- **Decomposition plots** showing trend, seasonal, and residual components.
