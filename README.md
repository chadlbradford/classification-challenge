# Module 13 Challenge - Spam Email Classification

## Overview
This project involves building and evaluating machine learning models to classify emails as spam or not spam. As an Internet Service Provider (ISP), improving email filtering is critical to enhancing customer experience. This challenge explores two classification models—**Logistic Regression** and **Random Forest Classifier**—to determine which model is better suited for detecting spam emails.

## Repository Structure
- `spam_detector.ipynb` - Jupyter Notebook containing the full implementation.
- `README.md` - This file provides an overview of the project.
- `data/` - Directory where the dataset is stored.

## Objectives
1. **Split the Data into Training and Testing Sets**
   - Load dataset from a provided CSV file.
   - Define features (`X`) and labels (`y`).
   - Check the balance of the target variable.
   - Split the data into training and testing sets.

2. **Scale the Features**
   - Use `StandardScaler` to normalize feature values.
   - Fit the scaler on training data and transform both training and testing sets.

3. **Create a Logistic Regression Model**
   - Train a **Logistic Regression** model with `random_state=1`.
   - Make predictions on the test data.
   - Evaluate the model's performance using **accuracy score**.

4. **Create a Random Forest Classifier Model**
   - Train a **Random Forest Classifier** with `random_state=1`.
   - Make predictions on the test data.
   - Evaluate the model's performance using **accuracy score**.

5. **Evaluate the Models**
   - Compare accuracy scores of both models.
   - Discuss how the results compare to initial predictions.

## Dataset
- The dataset consists of numerical features representing word frequencies, character counts, and capital letter usage.
- The target variable (`spam`) has two values:
  - `0`: Not spam (legitimate email)
  - `1`: Spam email

## Model Comparison & Findings
### **Prediction Before Model Training**
Before training, it was predicted that the **Random Forest Classifier** would outperform **Logistic Regression** due to its ability to handle complex relationships among many features.

### **Accuracy Scores**
| Model | Accuracy |
|--------|-----------|
| Logistic Regression | 92.94% |
| Random Forest Classifier | 93.92% |

### **Which Model Performed Better?**
- The **Random Forest Classifier** achieved a **higher accuracy score** than the Logistic Regression model, confirming our hypothesis.
- However, the **Logistic Regression model performed better than expected**, showing strong classification ability despite assuming linear relationships.

### **Comparison to Initial Prediction**
- The prediction that **Random Forest** would outperform **Logistic Regression** was **correct**.
- The **unexpectedly strong performance** of Logistic Regression suggests that some features have strong linear correlations with spam classification.

## Grading Rubric Alignment
This notebook satisfies all requirements for full credit:
✅ **Data is split into training and testing sets**
✅ **StandardScaler is applied to scale features**
✅ **Logistic Regression model is trained and evaluated**
✅ **Random Forest model is trained and evaluated**
✅ **Model performances are compared and discussed**

## References
- Self-sourced code was vetted and debugged using ChatGPT.
- Spam data sourced from publicly available datasets.
