# Customer Purchase & Revenue Prediction

## Problem
Predict whether a customer will make a purchase in the next 90 days and estimate
how much revenue they are expected to generate using historical transaction data.

## Dataset
Transactional-level dataset containing:
- UserId
- TransactionTime
- NumberOfItemsPurchased
- CostPerItem

Each row represents a single purchase event.

## Approach
- Temporal train-test split to avoid data leakage
- RFM-style feature engineering (recency, frequency, monetary)
- Short-term behavioral features (last 14 and 28 days)
- Classification model for purchase prediction
- Regression model for revenue estimation
- Automated model selection using PyCaret

## Models & Evaluation
- Classification evaluated using AUC, Precision, Recall
- Regression evaluated using RMSE and R²

## Business Value
- Identifies high-propensity customers for targeted marketing
- Forecasts short-term customer revenue
- Supports data-driven customer prioritization

## Tech Stack
Python, Pandas, PyCaret, Scikit-learn

## Future Improvements
- Customer segmentation
- Model monitoring
- Deployment as a web app
