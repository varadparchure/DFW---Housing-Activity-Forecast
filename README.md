# Dallas - Fort Worth - Arlington Region Housing Activity Forecast

## Project Overview

This project aims to forecast **median home prices** and **monthly sales** in the **Dallas-Fort Worth-Arlington** metropolitan area using **historical data** from the Texas A&M Real Estate Research Center and key **economic indicators**. By leveraging advanced forecasting techniques, this project provides **actionable insights** into the housing market, assisting stakeholders like real estate professionals, investors, and policymakers in making informed decisions.

## Data Sources

- **Texas A&M Real Estate Research Center**: Provides historical data on housing sales, prices, and other related metrics for the Dallas-Fort Worth-Arlington region.
- **Exogenous Variables**:
  - **Mortgage Rates**: Impact on housing affordability and demand.
  - **Federal Interest Rates**: Influences mortgage rates and broader economic conditions.

## Forecasting Models

We used a variety of machine learning and statistical models to forecast the housing activity:

1. **SARIMA/SARIMAX (Seasonal ARIMA with exogenous variables)**:
   - A time series model that captures seasonal trends and patterns in the housing market.
   - Exogenous variables like mortgage and interest rates are incorporated to refine predictions.

2. **LSTM (Long Short-Term Memory)**:
   - A deep learning-based model designed to capture long-term dependencies and complex patterns in sequential data.
   - Utilizes historical data to make future predictions while accounting for fluctuations in the market.

3. **XGBoost**:
   - A gradient boosting algorithm used for both regression and classification tasks.
   - Applied in two scenarios:
     - **Without Economic Factors**: Focused solely on historical housing data.
     - **With Economic Factors**: Incorporated mortgage and federal interest rates to enhance predictive power.

## Approach

1. **Data Collection**:
   - Gathered monthly housing activity data from the Texas A&M Real Estate Research Center.
   - Included external economic indicators such as mortgage rates and federal interest rates.
   
2. **Data Preprocessing**:
   - Cleaned and transformed the data to ensure compatibility with the forecasting models.
   - Applied necessary feature engineering, including handling missing data and creating lagged variables for time-series analysis.

3. **Modeling**:
   - Trained multiple models using historical housing data and exogenous variables.
   - Tuned hyperparameters to improve model performance and reduce overfitting.
   
4. **Evaluation**:
   - Evaluated the models using appropriate metrics (e.g., RMSE, MAE) to assess forecast accuracy.
   - Validated models using a holdout test period to simulate future predictions.

5. **Forecasting**:
   - Generated future predictions for median home prices and monthly sales.
   - Analyzed forecast results to identify trends and potential opportunities for market participants.

## Results & Insights

- The **SARIMA/SARIMAX** model effectively captured the seasonal nature of the housing market and the impact of external economic factors.
- **LSTM** provided more nuanced predictions, reflecting market complexity, especially during periods of volatility.
- **XGBoost** proved robust when integrating economic factors, improving the model’s generalization and accuracy.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/dfw-housing-forecast.git
