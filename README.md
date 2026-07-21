# Customer Churn Prediction using Logistic Regression

## Objective

The objective of this project is to build a **Logistic Regression** model that predicts whether a customer is likely to leave a telecommunications company (customer churn). By analyzing customer demographics and service-related information, the model helps identify customers who are at risk of churning, enabling businesses to take proactive retention measures.

---

## Dataset Link

**Telco Customer Churn Dataset**

Kaggle: https://www.kaggle.com/datasets/blastchar/telco-customer-churn

> **Note:** The dataset is not included in this repository. Please download it from the Kaggle link above before running the notebook.

---

## Libraries Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

---

## Methodology

1. Loaded the Telco Customer Churn dataset using Pandas.
2. Explored the dataset by displaying the first five records and identifying numerical, categorical, and target variables.
3. Checked for missing values and handled missing data in the `TotalCharges` column.
4. Removed the `customerID` column as it does not contribute to prediction.
5. Encoded categorical variables using one-hot encoding.
6. Split the dataset into **80% training** and **20% testing** sets.
7. Standardized the numerical features using `StandardScaler`.
8. Trained a **Logistic Regression** model on the training dataset.
9. Predicted customer churn on the test dataset.
10. Evaluated the model using Accuracy, Precision, Recall, F1-Score, and Confusion Matrix.

---

## Results

The Logistic Regression model was evaluated using the following performance metrics:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

The model demonstrated good predictive performance and was able to classify most customer churn cases correctly. The confusion matrix showed that the majority of customers were correctly classified, with only a limited number of misclassifications.

---

## Conclusion

This project successfully developed a Logistic Regression model to predict customer churn using customer demographic and service-related features. Data preprocessing, categorical encoding, feature scaling, and model training resulted in a model capable of identifying customers likely to leave the company. Features such as tenure, contract type, monthly charges, internet service, and payment method significantly influenced churn prediction. While Logistic Regression provides a simple, interpretable, and efficient solution, its assumption of a linear relationship between features and the target variable limits its ability to capture complex patterns. More advanced machine learning models, such as Random Forest or XGBoost, may achieve higher predictive accuracy for this problem.
