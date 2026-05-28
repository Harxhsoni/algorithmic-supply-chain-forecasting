# Algorithmic Supply Chain & Demand Forecasting Platform

<img width="1166" height="651" alt="dashboard_screenshot" src="https://github.com/user-attachments/assets/8559514a-37ec-4513-ba06-e7a4ea3e8250" />

## 📌 The Business Problem
E-commerce and retail giants lose billions annually due to stockouts (losing sales) and overstocking (tying up capital in dead inventory). Static reorder points fail to adapt to dynamic consumer demand and variable supplier lead times.

## 💡 The Solution
Developed an end-to-end algorithmic pipeline that dynamically calculates Reorder Points and Safety Stock. By leveraging Machine Learning for demand forecasting and Statistical Simulations for risk management, this system ensures a 95% service level while minimizing blocked capital.

## 🛠️ Tech Stack & Architecture
* **Database Engine:** SQLite (Relational Schema Design with strict PK/FK constraints)
* **Data Engineering:** Advanced SQL (CTEs, Window Functions for time-series feature engineering)
* **Machine Learning:** Python, Scikit-Learn (Random Forest Regressor for 7-day demand forecasting)
* **Statistical Optimization:** SciPy (Demand variance and dynamic safety stock calculation)
* **Business Intelligence:** Power BI (Live warehouse health monitoring and reorder alerts)

## 🚀 Workflow Highlights
1. Extracted and transformed daily transaction data entirely within the SQL engine to optimize memory.
2. Handled chronological train-test splitting to prevent future data leakage during ML training.
3. Wrote the final predicted metrics back to the analytical SQL table (`inventory_predictions`).
4. Designed a minimalist, executive-level Power BI dashboard for real-time procurement decisions.
