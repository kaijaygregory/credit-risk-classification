# __Credit Risk Classification Project__

## __Overview__

This project focuses on training and evaluating a machine learning model for credit risk analysis using historical lending activity data. The goal is to build a model that can identify the creditworthiness of borrowers using a dataset from a peer-to-peer lending services company.

### __Background__
In this challenge, various techniques were employed to train and evaluate a logistic regression model to predict loan risk. The dataset includes information where a '0' indicates a healthy loan, while '1' signifies a high risk of default.

## __Instructions and Tasks__
The project tasks were divided into several sections:

1. __**Splitting Data**:__ Segregation of data into training and testing sets.

2. __**Logistic Regression Model**:__ Building and evaluating a Logistic Regression model.

3. __**Credit Risk Analysis Report**:__ Summary and analysis of the model's performance.

## __Project Progress and Results__

### __Splitting the Data__

- The dataset was loaded into a Pandas DataFrame.

- Labels (`y`) were created from the 'loan_status' column, while features (`X`) were created from other columns.

- The data was split into training and testing datasets using `train_test_split`.

### __Logistic Regression Model__

- A Logistic Regression model was fitted with the original data.

- Predictions were generated and the model's performance was evaluated:
  - Confusion matrix and classification report were generated.
  - Analysis was performed to assess the model's prediction for healthy and high-risk loans.

For detailed analysis and code implementation, refer to the Jupyter Notebook [`credit_risk_classification.ipynb`](https://github.com/kaijaygregory/credit-risk-classification/blob/main/Credit_Risk/credit_risk_classification.ipynb).

## __References and Data Source__
- Data: Generated by edX Boot Camps LLC for educational purposes only.

## __Credit Risk Analysis Report__

__Overview of the Analysis__

The objective of this analysis was to develop and evaluate a machine learning model for credit risk assessment based on historical lending data. The dataset comprised financial information on past lending activities, where '0' indicated healthy loans and '1' signified a high risk of default. Our aim was to predict the creditworthiness of borrowers by employing logistic regression.

Basic insights into the data involved a value_counts assessment indicating the distribution of healthy and high-risk loans within the dataset. The stages of the machine learning process encompassed data preprocessing, feature selection, model training using logistic regression, and model evaluation.

Resampling methods were employed to address the class imbalance within the dataset, specifically utilizing the RandomOverSampler from the imbalanced-learn library.

__Results__

The performance metrics of the machine learning models are summarized below:

- **Logistic Regression Model with Original Data:**
  - **Accuracy:** 0.99
  - **Precision (Label 0 - Healthy Loans):** 1.00
  - **Precision (Label 1 - High-Risk Loans):** 0.87
  - **Recall (Label 0 - Healthy Loans):** 1.00
  - **Recall (Label 1 - High-Risk Loans):** 0.89

- **Logistic Regression Model with Oversampled Data:**
  - **Accuracy:** 1.00
  - **Precision (Label 0 - Healthy Loans):** 1.00
  - **Precision (Label 1 - High-Risk Loans):** 0.87
  - **Recall (Label 0 - Healthy Loans):** 1.00
  - **Recall (Label 1 - High-Risk Loans):** 1.00
  
  #__Summary__

The logistic regression models demonstrate consistent and robust performance in distinguishing between healthy and high-risk loans. Both models exhibit perfect precision and recall for healthy loans, ensuring accurate identification of these loans. For high-risk loans, the models maintain a high precision of 87%, correctly identifying a substantial portion of high-risk loans while maintaining a high accuracy level for healthy loans.

The performance might vary depending on the context of the problem. If the focus is primarily on accurately identifying high-risk loans, both models showcase satisfactory performance. However, if precision and recall balance is critical, the oversampled data model might provide a slight advantage in identifying high-risk loans.

Therefore, based on the overall performance and the balance between precision and recall, I recommend utilizing the logistic regression model trained on the oversampled data for credit risk assessment. It demonstrates a consistent and balanced performance in identifying both healthy and high-risk loans.

