Inventory Stock Forecasting using Time Series & Machine Learning

🚀 Overview
This project focuses on forecasting inventory stock levels using a combination of time series models and machine learning algorithms. It helps in making better supply chain decisions by predicting future stock and evaluating lead time demand.

🎯 Objective
- Forecast stock for each part number for future months
- Compare multiple models and select the best one dynamically
- Avoid flat predictions using improved feature engineering
- Support inventory planning using lead time calculations

📊 Models Used
- ARIMA
- SARIMA
- Random Forest Regressor
- XGBoost Regressor

🧠 Methodology

1. Data Preprocessing
- Cleaned and formatted dataset
- Converted date columns
- Sorted data by part and time

2. Feature Engineering
- Lag Features (lag1, lag2)
- Rolling Mean
- Trend Feature
- Seasonal Encoding using Sin & Cos

3. Model Training
- Models trained on historical stock data
- Last 3 months used for validation

4. Model Evaluation
- Metric used: Mean Absolute Percentage Error (MAPE)
- Best model selected based on lowest MAPE

5. Forecasting
- Forecast generated for next 12 months
- Controlled variation added to lag features to avoid constant predictions

6. Lead Time Demand Calculation
- Daily demand derived from historical consumption
- Internal and external lead time demand calculated

📈 Key Features
- Multi-model comparison
- Dynamic model selection
- Fix for constant prediction issue
- Time series + ML hybrid approach
- Business-oriented output format

📂 Dataset Columns Used
- Part_number
- Period_month
- Consumption
- Stock_end_of_month
- Internal_leadtime
- External_leadtime

📊 Output Format
The final output includes:

- Historical + Forecast data
- Forecast values from all models
- MAPE for each model
- Best model selection
- Final forecast
- Lead time demand metrics

🧠 Key Learning
- Importance of feature engineering in time series ML
- Difference between demand and stock forecasting
- Handling flat predictions in tree-based models
- Model evaluation using validation data

⚠️ Challenges Faced
- Constant predictions from ML models
- Handling missing/zero values in MAPE
- Feature engineering for future forecasting

✅ Solutions Applied
- Added trend and seasonal features
- Introduced controlled lag variation
- Used validation-based model selection

🚀 Future Improvements
- Hybrid ARIMA + ML error correction
- Safety stock & reorder point calculation
- Hyperparameter tuning
- Dashboard visualization

🛠️ Tech Stack
- Python
- Pandas, NumPy
- Statsmodels
- Scikit-learn
- XGBoost

📌 Conclusion

This project demonstrates a practical approach to inventory forecasting by combining statistical and machine learning models, making it suitable for real-world supply chain applications.

This project demonstrates a practical approach to inventory forecasting by combining statistical and machine learning models, making it suitable for real-world supply chain applications.
