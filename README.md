# Sprint Project – Customer Churn Prediction for Beta Bank

This project focused on helping **Beta Bank** retain customers by building a machine learning model that predicts which clients are likely to leave. Since customer acquisition is more expensive than retention, identifying high-risk customers in advance could save the bank money and improve customer loyalty.

### Predicting Who’s Likely to Leave

The goal was to train a classification model that predicts customer churn using banking customer data. To be considered successful, the model needed to achieve an **F1 score of at least 0.59** and would be evaluated using **AUC-ROC** as well.

#### The Data

The dataset provided customer-level information, including:

- **Demographics**: `Age`, `Gender`, `Geography`
- **Banking Activity**: `CreditScore`, `Tenure`, `Balance`, `EstimatedSalary`
- **Target Variable**: `Exited` (1 = churned, 0 = stayed)

#### The Process

1. **Exploratory Data Analysis (EDA)**  
   - Investigated class imbalance and feature distributions.
   - Noted trends: customers with higher age and lower tenure were more likely to churn.

2. **Preprocessing**  
   - Encoded categorical variables.
   - Split data into training, validation, and test sets using stratification to maintain target distribution.

3. **Baseline Modeling**  
   - Started with Logistic Regression and Decision Trees.
   - Evaluated models using **F1 score** and **AUC-ROC**.

4. **Handling Class Imbalance**  
   - Applied **SMOTE** and class weighting to boost performance on the minority class.

5. **Model Tuning & Evaluation**  
   - Improved model performance through hyperparameter tuning.
   - The final model met the F1 score threshold and showed strong ROC curve separation.

### Results & Takeaways

This project taught me how to balance performance metrics when dealing with imbalanced classes. I also gained hands-on experience applying classification techniques, evaluating models beyond accuracy, and using sampling methods like SMOTE to improve recall for critical cases.
