# Credit Card Fraud Detection using Logistic Regression

This repository contains code for building a simple logistic regression model to detect credit card fraud using scikit-learn.

## Dataset

The dataset used in this project is a CSV file named `creditcard.csv`. It contains transaction data, including features like time, amount, and Class (whether the transaction is fraudulent or not).

## Code Explanation

1. **Loading the Dataset**: We load the dataset into a Pandas DataFrame using `pd.read_csv()`.

2. **Data Exploration**:
    - Check for missing values: We use `credit_card_data.isnull().sum()` to check for missing values in the dataset.
    - Class Distribution: We use `credit_card_data['Class'].value_counts()` to check the distribution of classes (fraudulent vs. legitimate transactions).
    - Summary Statistics: We calculate summary statistics for transaction amounts for both legitimate and fraudulent transactions.

3. **Data Preparation**:
    - We create a balanced dataset by randomly sampling an equal number of legitimate and fraudulent transactions.
    - Concatenate the sampled data to create a new dataset.

4. **Splitting the Data**:
    - We split the data into training and testing sets using `train_test_split()`.

5. **Model Building**:
    - We initialize a Logistic Regression model using `LogisticRegression()` and train it on the training data using `model.fit()`.

6. **Model Evaluation**:
    - We evaluate the model's performance on both the training and testing data using accuracy score (`accuracy_score()`).

## Instructions to Run the Code

1. Make sure you have Python installed on your system.
2. Install the required libraries: `numpy`, `pandas`, and `scikit-learn`.
3. Download the `creditcard.csv` dataset and place it in the same directory as the code.
4. Run the script `credit_card_fraud_detection.py`.
5. The code will output the accuracy score on both the training and testing data.

