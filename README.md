# 🚖 Uber India 2024 – NCR Ride Analytics & Decision Lab (Streamlit)

![status](https://img.shields.io/badge/status-production--ready-green)
![python](https://img.shields.io/badge/python-3.10%2B-blue)
![streamlit](https://img.shields.io/badge/streamlit-1.37+-ff4b4b)
![license](https://img.shields.io/badge/license-MIT-lightgrey)

A consulting-grade, single-file Streamlit application for analyzing a **150,001-row Uber-like bookings dataset (NCR, 2024)**, diagnosing **completion/cancellation** drivers, and running **ML/forecasting/segmentation** with **operational simulations**. Built for speed, clarity, and boardroom-ready visuals.

---

## 🧭 Value Proposition

- **Executive Overview**: KPI cards, funnels, time-series revenue/demand, and quick “what’s spiking” insights.
- **Root-Cause**: Breakdowns of completion vs. cancellations across vehicle types, time buckets, and locations.
- **Ops & Finance**: VTAT/CTAT distributions and correlations; ARPR (Average Revenue per Ride), revenue by mix, value-distance dynamics.
- **ML Lab**:
  - **Classification** (`will_complete`): Logistic, Random Forest, XGBoost, LightGBM with **time-aware split**.
  - **Forecasting**: Daily/hourly demand via **ARIMA** and **Prophet**.
  - **Clustering**: Customer segmentation (K-Means default; DBSCAN/GMM optional) with **persona cards**.
  - **Regression**: Predict **Booking Value** with diagnostics (RMSE/MAE/R², residuals).
  - **Risk & Fraud**: Isolation Forest/DBSCAN to flag anomalous patterns.
- **Operations Simulator**: Adjust **driver supply**, **incentives**, and **pricing uplift** to compare **Baseline vs. Scenario** on completion, revenue, and ratings.
- **Exports**: One-click downloads of filtered data, predictions, clusters, and forecasts. Auto-generate a short HTML report.

---

## 📦 Data Schema (STRICT)

**CSV name:** `ncr_ride_bookingsv1.csv` (day-first dates)  
**Columns:**

