# retail-sales-forecasting

## Overview
This project focuses on predicting daily retail sales using historical data. The model incorporates time-series feature engineering to capture trends, seasonality and promotional effects.

### Data used:
- Rossman Store Sales Dataset

## Objective
- Forecast daily sales accurately
- Identify key drivers of revenue
- Improve business decision-making

## Methodology 
1. Data Preprocessing
   - Merged store and sales data
   - Handled missing values
   - Removed the closed store records
2. Feature Engineering
   -  Extracted time-based features:
     - Year, Month, Day, Day of Week
   - Created:
     - Lag feature (previous day sales)
     - Rolling mean (7-day average)
     - Weekend indicator
3. Validation Strategy
   - Implemented time-based split (critical for forecasting)
4. Model Used:
   - Random Forest Regressor

## Model Performance
- Baseline MAE: ~1100
- Final MAE: ~303
- Improvement: ~72% reduction in error

## Key Insights
- Promotions significantly increase sales
- Recent sales trends are the strongest predictors
- Store-level differences impact performances
- Seasonality plays a major role in demand

## Visualization
- Actual vs Predicted Sales comparison
- Feature importance analysis

## Business Impact 
- Enables accurate demand forecasting
- Supports inventory planning
- Improves promotion strategy effectiveness

## Tools & Technologies
- Python
- Pandas, Numpy
- Matplotlib, Seaborn
- Scikit-learn
