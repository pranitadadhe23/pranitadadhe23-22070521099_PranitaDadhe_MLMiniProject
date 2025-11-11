
# ⚡ Coal Stock Forecasting using Machine Learning and Deep Learning

### 🧠 Mini Project — Machine Learning (Section C)

**By:** Pranita Dadhe (PRN: 22070521099)
**Institute:** Symbiosis Institute of Technology, Nagpur
**Email:** [pranita.dadhe.btech2022@sitnagpur.siu.edu.in](mailto:pranita.dadhe.btech2022@sitnagpur.siu.edu.in)

---

## 📖 Project Overview

This project focuses on analyzing and forecasting coal stock levels of Indian thermal power plants using data obtained from the **India Data Portal**. The aim is to monitor stock sufficiency, identify shortage patterns, and forecast future stock levels using various **machine learning and deep learning models**.

The dashboard and models help optimize coal distribution and ensure uninterrupted power generation through data-driven insights.

---

## 📊 Dataset Details

**Source:** [India Data Portal - Coal Stock Data](https://indiadataportal.com/p/power/r/mop-coal_stock-pl-dl-aaa)
**Coverage:** National (India)
**Time Period:** 2018 – 2025
**Total Records:** 3,62,035
**Attributes:** 22

### 🔑 Key Variables

* `date` – Record date
* `state_name`, `state_code` – State information
* `power_station_name` – Name of the power plant
* `sector`, `utility`, `mode_of_transport` – Coal supply details
* `capacity`, `daily_requirement`, `daily_receipt`, `total_stock` – Stock statistics
* `plf_prcnt`, `stock_days`, `is_critical` – Performance indicators

---

## 🧹 Data Cleaning & Preprocessing

✔️ Removed missing and duplicate records
✔️ Converted date columns to datetime objects
✔️ Standardized column names
✔️ Handled nulls using mean/median imputation
✔️ Created derived features such as **expected_stock**, **month**, and **day**

---

## ⚙️ Machine Learning Techniques Implemented

| **Technique**                       | **Type**      | **Result Summary**                                                        |
| ----------------------------------- | ------------- | ------------------------------------------------------------------------- |
| **Simple Linear Regression**        | Supervised    | Accurate predictions for total stock vs expected stock (R² ≈ 0.97)        |
| **Multiple Linear Regression**      | Supervised    | Incorporated multiple predictors (month, day) with improved trend capture |
| **Random Forest Regressor**         | Supervised    | High accuracy and robustness against outliers                             |
| **K-Means Clustering**              | Unsupervised  | Grouped similar plants based on coal stock behavior                       |
| **Prophet Forecasting**             | Time Series   | Provided 7-day and 30-day stock forecasts                                 |
| **ANN (Artificial Neural Network)** | Deep Learning | Moderate performance (R² ≈ 0.97, RMSE ≈ 33.6)                             |
| **LSTM (Long Short-Term Memory)**   | Deep Learning | Captured temporal trends (R² ≈ 0.98, RMSE ≈ 891.6)                        |

---

## 📈 Model Results Summary

| **Model**         | **R² Score** | **MAE** | **RMSE** | **Performance**                       |
| ----------------- | ------------ | ------- | -------- | ------------------------------------- |
| Linear Regression | 0.973        | 6.18    | 33.63    | ✅ Excellent                           |
| Random Forest     | 0.982        | 5.32    | 28.10    | ✅ Excellent                           |
| ANN               | 0.974        | 6.18    | 33.63    | ✅ Good                                |
| LSTM              | 0.978        | 776.89  | 891.61   | ⚠️ Average                            |
| Prophet Forecast  | –            | –       | –        | ✅ Conclusive (Forecast Visualization) |

---

## 💻 Streamlit Dashboard

A Streamlit-based web dashboard was created to visualize:

* 📉 **Days of Supply over Time**
* 🔁 **Total Stock Trends**
* 📅 **7-Day Forecasting using Linear Regression**

**Features:**

* Real-time filtering by state, transport mode, and sector
* Interactive charts for stock monitoring
* Easy visualization of forecasted vs actual stock levels

---

## 📂 Repository Structure

```
📦 Coal-Stock-Forecasting/
 ┣ 📜 data/
 ┃ ┗ coal_stock.csv
 ┣ 📜 notebooks/
 ┃ ┣ 01_DataCleaning.ipynb
 ┃ ┣ 02_RegressionModels.ipynb
 ┃ ┣ 03_Clustering.ipynb
 ┃ ┣ 04_DeepLearning.ipynb
 ┣ 📜 app.py  # Streamlit Dashboard
 ┣ 📜 requirements.txt
 ┣ 📜 README.md
 ┗ 📜 report.pdf
```

---

## 🧠 Key Learnings

* Preprocessing large, structured time-series data
* Applying ML and DL models for forecasting
* Model evaluation using R², MAE, and RMSE
* Deploying interactive dashboards with **Streamlit**

---

## 🚀 Conclusion

This project successfully demonstrated how machine learning and deep learning can forecast coal stock levels efficiently.
While **Linear Regression, Random Forest, and Prophet** gave conclusive results, **LSTM** showed potential for further improvement with more granular time data.
The Streamlit dashboard enhanced interpretability and made the model insights accessible to decision-makers.

---

## 🌟 Author

**👩‍💻 Pranita Dadhe**
B.Tech — Computer Science
Symbiosis Institute of Technology, Nagpur
📧 [pranita.dadhe.btech2022@sitnagpur.siu.edu.in](mailto:pranita.dadhe.btech2022@sitnagpur.siu.edu.in)
🔗 [GitHub Profile](https://github.com/pranitadadhe23)

