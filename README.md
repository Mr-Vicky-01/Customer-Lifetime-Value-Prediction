# Customer Lifetime Value Prediction

![OIP](https://github.com/Mr-Vicky-01/California_housing_price/assets/143078285/d4c4c5c2-3bd4-4bb6-ab06-53e1afd5be7d)

## Dataset Overview

This analysis aims to predict customer lifetime value using the provided dataset from Kaggle. The dataset contains information about customers, their characteristics, and relevant features for predicting their lifetime value.

### Dataset Details

- **Number of Rows:** 9134
- **Columns:**
  - Customer
  - State
  - Customer Lifetime Value
  - Response
  - Coverage
  - Education
  - Effective To Date
  - EmploymentStatus
  - Gender
  - Income
  - Location Code
  - Marital Status
  - Monthly Premium Auto
  - Months Since Last Claim
  - Months Since Policy Inception
  - Number of Open Complaints
  - Number of Policies
  - Policy Type
  - Policy
  - Renew Offer Type
  - Sales Channel
  - Total Claim Amount
  - Vehiclelass
  - Vehicle Size

## Project Outcome

In this analysis, we performed hyperparameter tuning for an XGBoost Regressor using Grid Search. The following hyperparameters were explored:

- Learning Rate: [0.01, 0.1, 0.2]
- Number of Estimators: [100, 200, 300]
- Maximum Depth: [3, 5, 7]

After conducting a Grid Search with cross-validation (cv=3) and using the R-squared score as the evaluation metric, the best combination of hyperparameters was found to be:

- Learning Rate: 0.1
- Number of Estimators: 100
- Maximum Depth: 3

This configuration resulted in the highest R-squared score of approximately 0.6825 on the training data. These hyperparameters can be used to train the final XGBoost Regressor model for accurate predictions on new data.

The next steps in the analysis could involve evaluating the model's performance on a validation or test set, interpreting feature importance, and potentially refining the model further based on specific business requirements or considerations.

## Project Link

[Customer Lifetime Value Prediction GitHub Repository](https://github.com/Mr-Vicky-01/Customer-Lifetime-Value-Prediction.git)
