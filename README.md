# Objective: Predict whether a customer will leave the bank.

Retaining existing customers is more cost-effective than acquiring new ones. Therefore, accurately identifying customers at risk of leaving is valuable.

**Problem Type:**
- Binary Classification
- Likely class imbalance

## Skills demonstrated
- Machine Learning
- Learning algorithms
- Scikit-Learn library and metrics
- Exploratory Data Analysis
- Training, validation, and test datasets
- Logistic Regression
- Random Forest
- Accuracy Score
- F1-score
- AUC-ROC

## Tools
Python, pandas, sklearn, accuracy_score, train_test_split

## Results
After exploring different classification models and techniques to address class imbalance, the best performance was achieved using a **Random Forest model trained with upsampling** and an optimized classification threshold of **0.37**.

The model meets the project requirements and provides a balanced and practical solution for churn prediction. It achieves the required F1-score threshold and demonstrates strong discriminative ability as confirmed by the AUC-ROC metric.

**📊 Final results:**
- *F1-score: 0.5939*
- *AUC-ROC: 0.8378*

**🗝️ Key findings:**
- Logistic Regression was very sensitive to imbalance handling, improving recall significantly but failing to achieve a good balance with precision.
- Random Forest consistently provided better trade-offs between precision and recall across all sampling strategies.
- Upsampling improved recall but required threshold tuning to achieve optimal F1 performance.
- AUC-ROC remained consistently high across models, indicating strong overall separability between churn and non-churn customers.

**🏦 Business interpretation**
The final model is effective for identifying customers at risk of leaving the bank. 
By optimizing the decision threshold, the model prioritizes recall, which is critical in churn prevention scenarios where failing to identify at-risk customers is more costly than generating false positives.

This allows the bank to target retention efforts more effectively, reducing customer loss while maintaining a manageable level of marketing interventions.

## Notebook
See model_churn.ipynb
