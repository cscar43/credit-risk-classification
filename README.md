# Credit Risk Analysis README

This repository contains the code and analysis for the Credit Risk Analysis Challenge. The challenge aims to evaluate the performance of a logistic regression model in predicting credit risk.

## Instructions

### Split the Data into Training and Testing Sets

1. Start by opening the provided notebook file, `starter_code.ipynb`.
2. Load the lending data from the `lending_data.csv` file located in the `Resources` folder into a Pandas DataFrame.
3. Create the labels set (`y`) from the "loan_status" column, and then create the features DataFrame (`X`) from the remaining columns.
   - Note: A value of 0 in the "loan_status" column indicates a healthy loan, while a value of 1 indicates a high risk of default.
4. Split the data into training and testing datasets using the `train_test_split` function.

### Create a Logistic Regression Model with the Original Data

1. Utilize your knowledge of logistic regression to create a model by following these steps:
   - Fit a logistic regression model using the training data (`X_train` and `y_train`).
   - Save the predictions for the testing data labels by using the testing feature data (`X_test`) and the fitted model.
   - Evaluate the model's performance by completing the following tasks:
     - Generate a confusion matrix.
     - Print the classification report.
2. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?



# Credit Risk Analysis Report

## Overview

The purpose of this analysis is to evaluate the performance of machine learning models used for credit risk analysis. Credit risk analysis involves assessing the creditworthiness of borrowers to determine the likelihood of loan default. Accurate credit risk assessment is crucial for financial institutions to make informed lending decisions and mitigate potential losses. In this report, we will analyze the performance of the machine learning models employed in this analysis.

## Results

The performance of the machine learning models was evaluated using the following metrics:

- **Accuracy Score**: The accuracy score measures the overall correctness of the predictions made by the model. It is the ratio of correct predictions to the total number of predictions.

- **Precision Score**: The precision score quantifies the proportion of correctly predicted positive cases (credit defaults) out of the total predicted positive cases. It provides insights into the model's ability to avoid false positives.

- **Recall Score**: The recall score, also known as sensitivity or true positive rate, calculates the proportion of correctly predicted positive cases out of the actual positive cases. It indicates the model's effectiveness in capturing all relevant positive cases.

Based on the evaluation, the machine learning models achieved the following results:

- Model 1:
  - Precision Score (weighted avg): 0.99
  - Recall Score (weighted avg): 0.99
  - F1-Score (weighted avg): 0.99
  - Support: 
    - Healthy Loan: 18765
    - High-Risk Loan: 619

The precision score (weighted avg) of 0.99 indicates that Model 1 correctly identifies 99% of both healthy and high-risk loans out of the total predicted cases. The recall score (weighted avg) of 0.99 suggests that Model 1 captures 99% of the actual healthy and high-risk loans. The F1-score (weighted avg) of 0.99 represents the harmonic mean of precision and recall. These results demonstrate that Model 1 performs excellently in predicting both healthy and high-risk loans.

- Model 2:
  - Precision Score (weighted avg): 0.99
  - Recall Score (weighted avg): 0.99
  - F1-Score (weighted avg): 0.99
  - Support: 
    - Class 0: 18765
    - Class 1: 619

The precision score (weighted avg) of 0.99 indicates that Model 2 correctly identifies 99% of both class 0 and class 1 instances out of the total predicted cases. The recall score (weighted avg) of 0.99 suggests that Model 2 captures 99% of the actual class 0 and class 1 instances. The F1-score (weighted avg) of 0.99 represents the harmonic mean of precision and recall. These results demonstrate that Model 2 performs exceptionally well in predicting both classes.

## Summary

After evaluating the performance of Model 1 and Model 2, we can draw the following conclusions:

- Model 1 demonstrates excellent performance with a precision score of 0.99 and a recall score of 0.99 for both healthy and high-risk loans. The F1-score of 0.99 further confirms the model's accuracy in predicting both classes. With an accuracy score of 0.99, Model 1 achieves high correctness in its predictions. These results indicate that Model 1 is highly reliable and effective in credit risk analysis.

- Model 2 also exhibits impressive performance with a precision score of 0.99 and a recall score of 0.99 for both class 0 and class 1 instances. The F1-score of 0.99 demonstrates the model's ability to balance precision and recall. With an accuracy score of 0.99, Model 2 shows a high level of correctness in its predictions. These results indicate that Model 2 is highly accurate and reliable for credit risk analysis.

Considering the results and the objectives of the company, both Model 1 and Model 2 offer strong performance in credit risk assessment. They achieve similar accuracy, precision, and recall scores, indicating their ability to make accurate predictions. Based on specific requirements and considerations such as implementation feasibility, computational complexity, and interpretability, a final decision can be made between Model 1 and Model 2. Further evaluation and comparison can be conducted to select the most suitable model for the company's needs.

It's important to note that additional factors, such as scalability, real-world performance, and interpretability, should be considered when making the final decision on which model to use.
