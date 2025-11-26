# 🇬🇧 UK Tourism Forecasting using Facebook Prophet

An end-to-end **AI Time Series Forecasting Project** that predicts **future tourism arrivals in the United Kingdom** using the *International Tourism Arrivals* dataset from the **World Bank (via Kaggle)**.

This project cleans real-world data, reshapes it, trains a forecasting model using **Facebook Prophet**, and visualizes both historical and predicted values.

---

## 📌 **Project Overview**
Tourism forecasting is essential for planning, budgeting, and resource allocation in the travel and hospitality industry. This project builds a **yearly forecasting model** from 1995–2019 UK tourist arrival data and predicts future arrivals up to 2030.

---

## 📁 **Dataset Information**
- **Source:** Kaggle – *International Tourism, Number of Arrivals* (World Bank)
- **Original format:** Wide format (each year as a column)
- **Selected country:** United Kingdom
- **Period:** 1960–2019
- **Final usable range:** Years with non-null values

---

## 🛠️ **Technologies Used**
- **Python**
- **Pandas** (data cleaning & reshaping)
- **Prophet** (forecasting model)
- **Matplotlib** (visualizations)
- **Jupyter Notebook / VS Code Notebook**

---

## 📊 **Forecasting Pipeline**
### ✔ Step 1: Load the dataset
Convert dataset from Kaggle to CSV and load using Pandas.

### ✔ Step 2: Filter UK data
Select the row corresponding to "United Kingdom".

### ✔ Step 3: Clean the data
- Drop non-year columns
- Convert wide format → long format (Year, Arrivals)
- Remove missing values
- Convert Year to datetime
- Rename columns for Prophet: `ds` (date), `y` (value)

### ✔ Step 4: Build and train Prophet model
Prophet automatically learns:
- Long-term trend
- Yearly seasonality

### ✔ Step 5: Forecast the next 10 years (2020–2030)
Generate predictions and confidence intervals.

### ✔ Step 6: Visualize results
- Forecast plot (actual + predicted values)
- Trend plot
- Yearly seasonality plot

---

## 📈 **Forecast Results (Sample)**
| Year | Predicted Arrivals (yhat) |
|------|----------------------------|
| 2020 | ~37.8 million |
| 2021 | ~38.5 million |
| 2022 | ~39.2 million |
| 2023 | ~40.0 million |
| 2024 | ~40.5 million |
| 2025 | ~41.2 million |
| 2026 | ~41.9 million |
| 2027 | ~42.6 million |
| 2028 | ~43.2 million |
| 2029 | ~44.0 million |

The model predicts a **steady growth** in tourism for the UK.

---

## 🖼️ **Visualizations Included**
- `forecast_plot.png` → Full forecast timeline
- `forecast_components.png` → Trend + Yearly seasonality

---

## 🧠 **Model Insights**
- UK tourism shows a **strong upward trend** across decades.
- Seasonal component indicates cyclical patterns in tourist arrivals.
- Model is robust despite missing early years.

---

## 📦 **Project Structure**
```
AI_Tourism_Forecasting_UK/
│
├── forecast.ipynb
├── tourism.csv
├── uk_tourism_forecast.csv
├── forecast_plot.png
├── forecast_components.png
└── README.md
```

---

## ▶️ **How to Run the Project**
### 1. Clone the repository
```
git clone <repository-url>
```

### 2. Create virtual environment
```
python -m venv venv
venv\Scripts\activate
```

### 3. Install dependencies
```
pip install pandas prophet matplotlib jupyter
```

### 4. Run the notebook
Open `forecast.ipynb` in VS Code or Jupyter and run all cells.

---

## ⭐ **Future Improvements**
- Add monthly granularity (if data available)
- Build an interactive dashboard using Plotly or Streamlit
- Compare Prophet with ARIMA/LSTM

---

## 💡 **Why This Project is Valuable**
- Uses **real-world data**
- Demonstrates **data cleaning**, **reshaping**, and **visualization**
- Builds an **AI-based forecasting model**
- Perfect for **GitHub portfolios**, **resumes**, and **data science roles**

---

## 👩‍💻 **Author**
Created by Valentina — built with ❤️, persistence, and lots of coffee ☕.

---

