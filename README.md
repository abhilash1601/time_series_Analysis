**Summary: Time Series Forecasting for Wikipedia Page Views**

**Problem Statement and Dataset:**
- AdEase aims to optimize ad placement for clients by forecasting page views on Wikipedia pages over 550 days.
- Dataset: Includes two CSV files - `train_1.csv` containing daily page views for 145k Wikipedia pages and `Exog_Campaign_eng.csv` indicating dates with significant events affecting views, limited to English pages.

**Exploratory Data Analysis (EDA):**
- Imported dataset and performed exploratory analysis to understand its structure and characteristics.
- Checked for null values and discerned their reasons.
- Analyzed page name format, extracting information like title, language, access type, and origin.

**Data Preparation and Stationarity Check:**
- Converted data to a format suitable for ARIMA modeling (e.g., pivoting).
- Assessed data stationarity using methods like Dickey-Fuller test, decomposition, and differencing.
- Plotted AutoCorrelation Function (ACF) and Partial AutoCorrelation Function (PACF) plots to understand series characteristics.

**Modeling:**
- Created and trained ARIMA models, considering exogenous variables from `Exog_Campaign_eng.csv`.
- Utilized SARIMAX model incorporating exogenous variables for forecasting.
- Employed Facebook Prophet for time series forecasting.
- Employed grid search or similar techniques to determine optimal parameters for at least one modeling approach.

**Insights and Recommendations:**
- Analyzed forecast results across different languages.
- Derived insights and recommendations based on forecast performance and characteristics of time series data.

**Evaluation:**
- Evaluated model performance using Mean Absolute Percentage Error (MAPE).
- Previous MAPE ranged from 4-8%, indicating good forecasting accuracy.

**Conclusion:**
- Successfully developed and evaluated time series forecasting models to predict Wikipedia page views, facilitating optimized ad placement for AdEase clients across different languages and regions.
