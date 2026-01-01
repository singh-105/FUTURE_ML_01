# 📈 AI-Powered Retail Sales Forecasting & Inventory Dashboard

## 📝 Project Overview
This project was developed during my Data Analytics internship to solve a critical retail challenge: **Predicting future demand to optimize inventory levels.** By leveraging historical sales data (Price, Stock, and Volume), I built an end-to-end pipeline that cleans data with Python, forecasts 90 days of sales using the **Facebook Prophet Machine Learning model**, and visualizes actionable insights in **Power BI**.

---

## 🖼️ Dashboard Preview
![Retail Sales Forecast Dashboard](dashboard_preview.png)
*Figure 1: Final Interactive Dashboard showing Historical Sales vs. AI Predictions.*

---

## 💡 Key Features & Business Insights
* **Actual vs. Forecasted Trend**: A unified view of historical sales and 90-day future predictions ($yhat$).
* **Inventory Risk Alert**: Integrated analysis comparing `Stock Levels` vs. `Predicted Demand` to prevent stock-outs.
* **Price Elasticity Mapping**: A scatter plot analysis showing how price changes correlate with sales volume.
* **Seasonality Detection**: Automatically identified weekend sales spikes and monthly trends using Prophet's additive model.

---

## 🛠️ Tech Stack & Methodology
- **Python (Pandas)**: Used for data preprocessing, handling missing values, and feature engineering (extracting month/day/year).
- **Facebook Prophet**: Chosen for its robustness in handling seasonality, holidays, and trend changepoints in time-series data.
- **Power BI Desktop**: Used for data modeling (creating 1:1 relationships) and designing a professional UX/UI for business stakeholders.
- **Git/GitHub**: For version control and project documentation.

---

## 📁 Project Structure
- `data/`: Contains `mock_kaggle.csv` (raw), `cleaned_sales_data.csv`, and `forecast_results.csv`.
- `notebooks/`: 
    - `1_Data_Cleaning.ipynb`: Data preprocessing and formatting.
    - `2_Forecasting_Prophet.ipynb`: Training the ML model and exporting results.
- `dashboard/`: The `Retail_Sales_Dashboard.pbix` file.
- `requirements.txt`: Python dependencies (`prophet`, `pandas`, `matplotlib`).

---

## 🚀 How to Run this Project
1. **Setup Environment**:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows use: .venv\Scripts\activate
   pip install -r requirements.txt