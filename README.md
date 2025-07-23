# ARIMA Time-Series Forecasting – AAPL Stock Case Study


![Python](https://img.shields.io/badge/Python-3.9-blue)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)


This project demonstrates how to build and evaluate an ARIMA model using Python to forecast stock closing prices of Apple Inc. (AAPL). The focus is on transforming raw financial time-series data into actionable insights using statistical modeling techniques in Python.

---

## Overview

In this project, we use historical stock price data for Apple (AAPL) over 10 years and apply time-series modeling techniques to forecast future stock movements. We cleaned and resampled weekly AAPL data, tested for stationarity (ADF), and selected ARIMA(3,0,1) using ACF/PACF lag analysis. 
This project was completed as part of a Google Cloud Qwiklabs module in Machine Learning for Finance.

> 🧠 Note: This ARIMA forecasting pipeline could be adapted to model time-series patterns in energy markets such as crude oil, natural gas, or electricity pricing — relevant for trading and risk management applications.

---

## Tasks Performed

- Pulled historical financial data from **Google Cloud Storage** into a Pandas dataframe
- Cleaned and resampled the data to a **weekly frequency**
- Calculated **log returns** to normalize data
- Verified stationarity using the **Dickey-Fuller test**
- Visualized rolling statistics (mean & std dev)
- Plotted **ACF** and **PACF** to determine ARIMA parameters
- Built and evaluated an ARIMA model using **statsmodels**
- Compared **predicted returns vs actual values**
- Forecasted **2 weeks into the future**

---

## Tools Used

- Python (3.9)
- JupyterLab
- Pandas, NumPy, Matplotlib
- Statsmodels (ARIMA)
- Google Cloud Platform (Qwiklabs)

---

## Sample Outputs

- 📉 **Weekly Returns Line Plot:** Cleaned and normalized weekly price changes  
- 📈 **Rolling Mean & Std Dev:** Helps visualize variance and trends  
- 🔍 **Dickey-Fuller Test:** Confirmed data stationarity (p < 0.05)  
- 📊 **ACF & PACF Plots:** Used to select best ARIMA (p, d, q) parameters  
- 🧠 **Model Summary:** ARIMA(3,0,1) fit and evaluation  
- 🟥 **Prediction vs Actual:** Compared model outputs to historical truth  
- 🔮 **2-Week Forecast:** Simulated next 2 weeks of market movement

---

## Forecasting Output Visuals

### 1. Rolling Mean & Standard Deviation  
Shows variance stability and trends in weekly returns.  
![Rolling Mean & Std Dev](Media/rolling_stats.png)

---

### 2. ACF & PACF Plots  
Used to select best ARIMA(3,0,1). Peaks at lags 1–3 were evident.  
![ACF & PACF](Media/acf_pacf.png)

---

### 3. Fitted Values vs Actual Returns  
Red = ARIMA fitted values, Blue = true returns.  
![Predicted vs Actual](Media/pred_vs_actual.png)

---

### 4. 2-Week Forecast  
Green = forecasted returns beyond training data.  
![2-Week Forecast](Media/2week_forecast.png)


---

## Key Learnings

- Developed intuition for time-series modeling workflows
- Gained hands-on experience with **ARIMA model tuning**
- Understood the importance of **stationarity** and how to test for it
- Practiced **reading ACF/PACF plots** to derive lag parameters
- Strengthened understanding of **model evaluation techniques** (e.g. RMSE, fitted vs actual plots)
- Learned how to forecast future values and analyze predictive confidence
- Enhanced notebook documentation and visualization for technical communication

---

## Run This Project Yourself

1. Clone the repo  
2. Open `AAPL_ARIMA_Model.ipynb` in JupyterLab  
3. Run the cells in order  
4. Ensure `AAPL10Y.csv` is in the same directory  

```bash
pip install pandas numpy matplotlib statsmodels
```

---

## Project Structure

```
ARIMA-Financial-Time-Series/
├── Media/                    # Screenshots and result plots (PDFs)
├── AAPL10Y.csv               # 10 years of Apple stock price data
├── AAPL_ARIMA_Model.ipynb    # Main notebook with ARIMA model workflow
├── ARIMA Model Summary.pdf   # Model output summary (PDF)
└── README.md                 # Project documentation
```


---

## 🌟 Author

**Shozab Megatron**  
[LinkedIn](https://www.linkedin.com/in/shozab-n/) • [GitHub](https://github.com/shozab-megatron)

---

## Notes

This project was completed during a **Coursera x Google Cloud Qwiklabs** lab on Machine Learning for Finance.
