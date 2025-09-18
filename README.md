# Total_Cost_Forecast
A simple forecasting tool built for Mercedes-Benz to model individual cost drivers (Electricity, PPI, Gas, Wages, EUR/TL). Uses Prophet for time-series forecasting. Future updates will compare AI-based models and allow dynamic total cost simulation with interactive weight controls.


# 🧮 Forecast-Based Cost Indexing for Procurement Data

This project was developed during my internship at Mercedes-Benz Türk to support strategic purchasing decisions using cost forecasting and dynamic indexing.

## 🔍 What It Does
- **Forecasts** 5 key cost features using Facebook's Prophet:
  - Electricity (`Electricindex`)
  - Producer Price Index - PPI (`ppi`)
  - Natural Gas (`Gastl` + `gi`)
  - Minimum Gross Wage (`wage_index`)
  - EUR/TL Exchange Rate (`eurtli`)
- **Normalizes** index values dynamically: Set any month (e.g., March 2019) as the base = 100, and view index evolution over time.
- **Calculates** a dynamic **Total Cost Index** using weighted combinations of forecasted values (weights adjustable via sliders).
- **Visualizes** all results with clean Matplotlib charts and interactive widgets.

## 📁 Data
Input file: `pure_data.xlsx`  
Time range: **Jan 2016 – Mar 2025 (historical)** + **Apr 2025 – Mar 2026 (forecasted)**  
All data anonymized for internal use.

## 📦 Dependencies
- `pandas`
- `numpy`
- `prophet`
- `matplotlib`
- `ipywidgets`

## ✅ Next Steps
- Add export options (CSV, PNG)
- Develop summary comparison reports
- Optional: Deploy as a web dashboard

---

*Developed with real-world data and use case scenarios from a corporate environment (Mercedes-Benz Türk).*
