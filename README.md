# credit-risk-classification

## Overview
Purpose:
- Create a model to predict the credit-risk for clients seeking a loan

Dataset and Prediction:
- The financial information used consisted data from current clients, such as loan size, interest rate, borrower income, total debt, debt-to-income ratio, and derogatory remarks
- Attempting to classify clients into one of 2 categories: healthy loan or high-risk loan

Variables:
- Input variables: loan size, interest rate, borrower income, total debt, debt-to-income ratio, and derogatory remarks
- Output variable: loan status (healthy or high-risk)

Methods:
- The dataset was used to train a logistic regression model, to predict loan status
- Created a confusion matrix and classification report to reach conclusions

## Results
Confusion Matrix:

![image](https://github.com/korzenim/credit-risk-classification/assets/148805368/f42e4f12-95d1-483c-bccd-5e5251778a4d)

Classification Report:

![image](https://github.com/korzenim/credit-risk-classification/assets/148805368/55d22f1f-839a-45f3-808d-81fe66ea59d7)


## Summary
- The model predicts loan status with high accuracy:
    - healthy loan f1 score: 100%
    - high-risk loan f1 score: 87%
- The prediction for health loans is more accurate, possibly due to there being more data points (~18,000 compared to ~600 for high-risk loans)
- A total accuracy of 99% suggests the model can be safely used to predict both healthy and high-risk loans

## Requirements
### Split the Data into Training and Testing Sets (30 points)
To receive all points, you must:
- Read the lending_data.csv data from the Resources folder into a Pandas DataFrame. (5 points)
- Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns. (10 points)
- Split the data into training and testing datasets by using train_test_split. (15 points)

### Create a Logistic Regression Model (30 points)
To receive all points, you must:
- Fit a logistic regression model by using the training data (X_train and y_train). (10 points)
- Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model. (5 points)
- Evaluate the model’s performance by doing the following:
    - Generate a confusion matrix. (5 points)
    - Generate a classification report. (5 points)
    - Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels? (5 points)

### Write a Credit Risk Analysis Report (20 points)
To receive all points, you must:
- Provide an overview that explains the purpose of this analysis. (5 points)
- Using a bulleted list, describe the accuracy, precision, and recall scores of the machine learning model. (5 points)
- Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning. (10 points)

### Coding Conventions and Formatting (10 points)
To receive all points, you must:
- Place imports at the top of the file, just after any module comments and docstrings and before module globals and constants. (3 points)
- Name functions and variables with lowercase characters, with words separated by underscores. (2 points)
- Follow DRY (Don’t Repeat Yourself) principles, creating maintainable and reusable code. (3 points)
- Use concise logic and creative engineering where possible. (2 points)

### Code Comments (10 points)
To receive all points, your code must:
- Be well commented with concise, relevant notes that other developers can understand. (10 points)



