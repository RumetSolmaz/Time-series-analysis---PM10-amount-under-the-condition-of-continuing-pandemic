# Time series analysis PM10 amount under the condition of continuing pandemic
 Project Overview:
This project analyzes air pollution (PM10 levels) in Bursa, Turkey, using historical data from the Beyazıt Street air quality monitoring station.
The main objective is to estimate how PM10 levels might have evolved if the COVID-19 pandemic restrictions had continued.
We implemented and compared Prophet, XGBoost, LightGBM, and Random Forest models.

Dataset:
Source: Republic of Türkiye Ministry of Environment, Urbanization, and Climate Change – Air Quality Monitoring
Period: 2018–2021
Variable: PM10 concentration (µg/m³)
Includes both pre-pandemic, pandemic, and post-pandemic periods.

Methodology:
Data Preprocessing
Merging multiple year datasets.
Handling missing values.
Creating lag features.
Extracting date-based features (day, month, day of week).

Model Training:
Prophet: Capturing trend, seasonality, and changepoints.
XGBoost & LightGBM: Gradient boosting decision trees for short-term and sudden change sensitivity.
Random Forest: Stable ensemble of decision trees.

Results:
Prophet performed best for long-term seasonal trends.
XGBoost and LightGBM handled short-term variations well.
Random Forest provided stable but less dynamic predictions.
