# Churn-predictions
# Chance of Churn Prediction with XGBClassifier

## Project Overview
This project aims to predict the chance of clients of a telecom company to churn (cancel the service).
## Results
The model has a **roc_auc_score** of 0.843 but further hyperparameter tuning and validation methods may be applied in the future.


## Methodology

### 1. Data Cleaning & Preprocessing
* Redudant data and non-formataded data were properly dealt with accordinly to need
* Churn was transformed to binary
* **SimpleImputer** was used for numerical data (e.g. tenure)
* **OneHOtEncoder** was used for low diversity categorical data (e.g. PaymentMethod)
* **OrdinalEncoder** was used for high diversity categorical data and binary data (e.g. gender)

### 2. Model Configuration
* **early_stop_rounds** was used to prevent the overfitting of **n_estimators=2000**
* **max_depth=5** was used to how simple the data is
* **learning_rate=0.05** was used to achieve higher precision

---
*Developed by Henrique Varnier Bridi*