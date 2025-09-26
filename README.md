# Price-prediction Churn-prediction-analysis
## Goal 
Predict Airbnb listing prices based on property features (room type, city, accommodates, bedrooms, reviews, etc.).
## Insights 
Part A: Airbnb Price Prediction
Data Issues:
Many missing values (e.g., bedrooms, beds, reviews).
Strong right skew in price distribution (outliers).
Feature Engineering:
Created price_per_guest feature.
Extracted review year/month from dates.
Used categorical encoding (property_type, room_type, etc.).
Model: Linear Regression.
Evaluation: Measured with RMSE, MAE, and R².
Insights:
Price is highly influenced by room type, property type, and city.
More accommodates/bedrooms → generally higher price.
Outliers exist with very expensive listings, skewing predictions.
Model has moderate predictive power (linear regression may not capture non-linear relationships well).

Part B: Customer Churn Prediction
Data Issues:
TotalCharges was skewed and had missing values (handled with median).
Duplicate rows removed.
Preprocessing:
Label encoding for categorical features.
Standardization applied.
Model: Random Forest Classifier.
Evaluation: Used accuracy, confusion matrix, and classification report.
Insights:
Customers with higher monthly charges and shorter tenure are more likely to churn.
Certain contract types and payment methods strongly affect churn.

Random Forest achieved good performance, meaning feature interactions were well captured.
