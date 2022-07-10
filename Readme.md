# Customer-Attrition-Prediction

# Details of the Project

Predicting the probability of Attrition of new customers based on previous customers data.

# Dataset

- Prediction column : `Customer Attrition`
- Unique ID of customer : `ID`
- Dataset contains 14 features related to telecom data:

      `Sex`, `Aged`, `Married`, `Total Dependents`, `Service Span`, `Mobile Service`, `4G Service`, `Cyber Protection`, `Hardware Support`, `Technical Assistance`, `Film Subscription`, `Settlement Process`, `Quarterly Payment`, `Grand Payment`
- `Quarterly Payment`, `Grand Payment` are *continuous* data columns [In some experiments `Service Span` is also considered as continuous] and remaining are *Categorical* columns.

# Training

- I used `CatBoost`, `XGBoost`, `LightGBM`, `Histogram Gradient Boosting` techniques for training.
- After training based on obtaied feature importances, Various features were removed and experimented with different combination of features.
- Finally the best models are ensembled and achieved 79.06% accuracy on test data samples.


# Conclusion 

- The order of score with various models given same data pipeline is as follows : 
            Cat Boost > Light GBM > XG Boost > Histogram Gradient Boosting
- **Note** :  This order varies with varying Training data and features.

                  
