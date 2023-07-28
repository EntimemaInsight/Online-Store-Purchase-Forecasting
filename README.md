# Online-Store-Purchase-Forecasting

## Introduction

This repository contains the code and data for predicting customer behavior in an online store. The main goal of this project is to predict whether a given customer will make a purchase (1) or not (0) in the store. We explore two different classification models: Random Forest and Logistic Regression.

## Objectives 

1. Exploratory Data Analysis (EDA): We investigate the data to gain insights into its characteristics and distributions.
2. Data Preparation: We perform data cleaning and preprocessing, including one-hot encoding and label encoding for categorical features.
3. Model Training: We train two classification models, Random Forest, and Logistic Regression.
4. Model Evaluation: We compare the performance of the models and address class imbalance issues.
5. Model Selection: We select the most suitable model for purchase prediction.

## Requirements 

To run the code in this repository, you need the following dependencies:

Python 3.x
Numpy
Pandas
Matplotlib
Scikit-learn
Imbalanced-learn
Seaborn

## Dataset
The dataset used for this project can be found in the "data.csv" file. It contains information about customer interactions with the online store, including various features like administrative, informational, and product-related activities, traffic type, visitor type, and more.

## Key Insights

1. The "PageValues" feature is the most important in predicting customer purchases, followed by "ProductRelated_Duration" and "ExitRates."
2. Customers who spent more time on the website and viewed more pages (higher "PageValues" and "ProductRelated_Duration") were more likely to make a purchase.
3. The "Weekend" feature had some influence on purchase behavior, indicating that purchases might be more likely on weekends.
4. The "Month" and "VisitorType" features showed varying levels of impact on purchase behavior across different months and types of visitors.
5. The Random Forest model achieved good overall accuracy but struggled with recall and F1-score for predicting the positive class (purchases).
6. The Logistic Regression model showed improved performance after addressing class imbalance through random under-sampling.
7. Cross-validation results for the Logistic Regression model demonstrated stable and consistent performance.
8. The Logistic Regression model, after addressing class imbalance, proved to be the most suitable model for purchase prediction. It showed better precision and recall for the positive class, making it more effective at identifying potential customers likely to make a purchase.

## Results
The trained models' performance and evaluation metrics are discussed in the Jupyter Notebook, including accuracy, precision, recall, F1-score, and cross-validation results.

## Conclusion
In this project, we successfully built and evaluated models to predict customer purchase behavior in an online store. The code and analysis provided in this repository can be used as a starting point for similar purchase forecasting tasks in other domains.

## Credits
This project was created by Aleksandar Dimitrov and is licensed under the MIT License. If you have any questions or comments, feel free to contact me at alexi.zein@gmail.com.
