# 📈 ARIMA Model for Financial Time Series Forecasting


![Python](https://img.shields.io/badge/Python-3.9-blue)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)


This project demonstrates how to build and evaluate an ARIMA model using Python to forecast stock closing prices of Apple Inc. (AAPL). The focus is on transforming raw financial time-series data into actionable insights using statistical modeling techniques in Python.

---

## 🚀 Overview

In this project, we use historical stock price data for Apple (AAPL) over 10 years and apply time-series modeling techniques to forecast future stock movements. We clean and aggregate the data, test for stationarity, and tune an ARIMA model based on ACF/PACF analysis. Finally, we visualize the performance of the model by comparing predicted returns against actual data.

This project was completed as part of a Google Cloud Qwiklabs module in Machine Learning for Finance.

---

## 🧪 Tasks Performed

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

## ⚙️ Tools Used

- Python (3.9)
- JupyterLab
- Pandas, NumPy, Matplotlib
- Statsmodels (ARIMA)
- Google Cloud Platform (Qwiklabs)

---

## 📊 Sample Outputs

- 📉 **Weekly Returns Line Plot:** Cleaned and normalized weekly price changes  
- 📈 **Rolling Mean & Std Dev:** Helps visualize variance and trends  
- 🔍 **Dickey-Fuller Test:** Confirmed data stationarity (p < 0.05)  
- 📊 **ACF & PACF Plots:** Used to select best ARIMA (p, d, q) parameters  
- 🧠 **Model Summary:** ARIMA(3,0,1) fit and evaluation  
- 🟥 **Prediction vs Actual:** Compared model outputs to historical truth  
- 🔮 **2-Week Forecast:** Simulated next 2 weeks of market movement

---

## 🖼️ Media Gallery – ARIMA Time Series Outputs

| 📄 Description                    | 📎 File Link                                     |
|----------------------------------|--------------------------------------------------|
| Head of the Cleaned Data         | [View PDF](Media/Head_of_the_Cleaned_Data.pdf)  |
| Weekly Returns Line Plot         | [View PDF](Media/Weekly_Returns_Line_Plot.pdf)  |
| Rolling Mean & Standard Deviation| [View PDF](Media/Rolling_Mean_and_Std_Dev.pdf)  |
| Dickey-Fuller Stationarity Test  | [View PDF](Media/Dickey_Fuller_Test_Output.pdf) |
| ACF and PACF Correlation Plots   | [View PDF](Media/ACF_and_PACF_Plots.pdf)        |
| ARIMA Model Summary              | [View PDF](Media/ARIMA_Model_Summary.pdf)       |
| Prediction vs Actual Performance | [View PDF](Media/Prediction_vs_Actual_Plot.pdf) |
| 2-Week Forecast Output           | [View PDF](Media/2_Week_Forecast_Plot.pdf)      |

---

## 🎓 Key Learnings

- Developed intuition for time-series modeling workflows
- Gained hands-on experience with **ARIMA model tuning**
- Understood the importance of **stationarity** and how to test for it
- Practiced **reading ACF/PACF plots** to derive lag parameters
- Strengthened understanding of **model evaluation techniques** (e.g. RMSE, fitted vs actual plots)
- Learned how to forecast future values and analyze predictive confidence
- Enhanced notebook documentation and visualization for technical communication

---

## 📦 How to Run

1. Clone the repo  
2. Open `AAPL_ARIMA_Model.ipynb` in JupyterLab  
3. Run the cells in order  
4. Ensure `AAPL10Y.csv` is in the same directory  

```bash
pip install pandas numpy matplotlib statsmodels
```

---

## 🧰 Project Structure

ARIMA-Financial-Time-Series/
├── Media/                    # Screenshots and result plots (PDFs)
├── AAPL10Y.csv               # 10 years of Apple stock price data
├── AAPL_ARIMA_Model.ipynb    # Main notebook with ARIMA model workflow
├── ARIMA Model Summary.pdf   # Model output summary (PDF)
└── README.md                 # Project documentation

---

## 🌟 Author

**Shozab Megatron**  
[LinkedIn](https://www.linkedin.com/in/shozab-n/) • [GitHub](https://github.com/shozab-megatron)

---

## 📌 Notes

This project was completed during a **Coursera x Google Cloud Qwiklabs** lab on Machine Learning for Finance.
