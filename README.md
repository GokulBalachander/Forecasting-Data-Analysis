📊 Forecasting Project

📌 Overview

This project focuses on forecasting weekly sales using multiple time series and machine learning models. The goal is to analyze patterns in historical data and compare model performance using standard evaluation metrics.

⚙️ Tools & Technologies

Python
pandas, NumPy
matplotlib
statsmodels (ARIMA, SARIMAX)
scikit-learn
XGBoost

📂 Dataset

train.csv containing historical weekly sales data
Includes features such as Store, Department, Date, Weekly_Sales, and Holiday indicators

Note: Dataset may not be included due to size. Please use your own copy if needed.

📈 Project Workflow

Data loading and preprocessing
Time series creation for a specific Store–Department
Exploratory Data Analysis (EDA)
   . Trend analysis (rolling averages)
   . Seasonality analysis (monthly patterns)
Train/Test split using time-based approach
Model implementation and comparison

🤖 Models Used
Naive Baseline
Rolling Mean Baseline
ARIMA
SARIMAX
XGBoost

📊 Feature Engineering (XGBoost)

Lag features: previous weeks (lag_1, lag_2, lag_4, lag_8, lag_52)
Rolling statistics: moving averages and standard deviation
Calendar features: month, week of year
Holiday indicator

📏 Evaluation Metrics

MAE (Mean Absolute Error)
MSE (Mean Squared Error)
RMSE (Root Mean Squared Error)

📌 Results Summary

XGBoost achieved the best performance on the test set
ARIMA performed better than SARIMAX on this specific series
Baseline models helped validate that models learned meaningful patterns

💼 Business Impact

Enabled more accurate demand forecasting, helping businesses plan inventory and reduce overstock or stockouts.
Identified seasonal trends and holiday effects, supporting better promotional and sales planning.
Provided data-driven insights through model comparison, improving decision-making for selecting forecasting strategies.
Demonstrated how machine learning models like XGBoost can outperform traditional methods in capturing complex patterns.

🚀 Key Learnings
Time-based splits are critical for forecasting tasks
Feature engineering significantly improves machine learning models
Different models perform differently depending on the dataset characteristics

📎 How to Run
Open the notebook in Google Colab or Jupyter
Upload or load train.csv
Run all cells sequentially
