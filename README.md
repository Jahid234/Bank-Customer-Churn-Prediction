## Purpose 

This project aims to develop a machine learning model that predicts whether a bank customer is likely to churn (leave the bank). The bank can identify at-risk customers by analyzing various customer attributes like credit score, age, balance, and account activity. The insights gained from this model can help the bank take proactive measures, such as offering personalized services or incentives, to retain customers and reduce churn rates. Ultimately, the project aims to enhance customer retention and improve the bank's profitability.

## Methodology

# Data Collection and Loading:

The dataset consists of 10,000 bank customers with features such as credit score, country, gender, age, tenure, balance, number of products, credit card status, active membership status, estimated salary, and whether the customer churned.

## Data Exploration and Preprocessing:

## Outlier Detection and Handling:
Outliers in credit_score and age were detected using the interquartile range (IQR) method and were capped within acceptable limits.

## Data Cleaning:
No missing values or duplicate records were found in the dataset.

## Encoding:
Categorical variables such as country and gender were encoded using one-hot encoding to convert them into numerical form, suitable for model training.

## Data Splitting:
The data was split into a training set (75%) and a test set (25%) using train_test_split.

## Data Scaling:
Feature scaling was applied using StandardScaler to normalize the range of the features, ensuring that they are on a similar scale, which helps improve model performance.

## Model Training:
A Logistic Regression model was trained on the preprocessed data.
The features used include credit score, age, tenure, balance, number of products, credit card status, active membership status, estimated salary, and encoded variables for country and gender.

## Model Evaluation:

## Accuracy: 
The model was evaluated using the accuracy score on the test set, yielding 81.04% accuracy.
## Recall: 
The recall score, which measures the proportion of actual churned customers that were correctly identified, was 60.38%.

## Result:
The logistic regression model could predict customer churn with an accuracy of 81%, meaning the model correctly classified 81% of the test set.
A recall of 60.38% shows that the model identified approximately 60% of the customers who churned, balancing false negatives and ensuring that most churned customers are detected.
