# Store Sales - Time Series Forecasting

## Project Overview

This project uses machine learning techniques, specifically the Random Forest Regressor, to predict future sales for different product types in stores. By analyzing historical sales data, including store IDs, product families, sales numbers, holidays, and oil prices, the model helps stores optimize inventory management, reduce stock shortages, and improve profitability.

## Dataset

The dataset for this project is sourced from Kaggle, titled **Store Sales - Time Series Forecasting**. It contains the following key columns:
- **Store IDs**: Identifies the different stores.
- **Product Families**: Categories of products sold.
- **Sales Numbers**: The number of units sold.
- **Holidays**: Dates when sales may be affected by special events.
- **Oil Prices**: Historical oil prices, which could influence sales.
- **Store Transactions**: Details of store activity.

## Methodology

1. **Data Preprocessing**:
   - **Data Cleaning**: Missing values were checked (none found) and outliers were addressed.
   - **Feature Engineering**: Created new time-based features (month, day, and weekday) and lag features for temporal dependencies.
   - **Categorical Encoding**: Used one-hot encoding for product family categories.
   
2. **Exploratory Data Analysis (EDA)**:
   - Visualized sales distributions and trends over time.
   - Detected seasonal patterns in sales.

3. **Model Building**:
   - Selected **Random Forest Regressor** for predicting sales.
   - Split the data into training and testing sets (80% for training, 20% for testing).
   - Trained the model using 100 decision trees.

4. **Model Evaluation**:
   - Evaluated the model using **Mean Absolute Error (MAE)**, which quantifies the average error between predicted and actual sales.
   - The MAE value was found to be 104.47, indicating reasonable prediction accuracy.

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Store-Sales-Time-Series-Forecasting.git
