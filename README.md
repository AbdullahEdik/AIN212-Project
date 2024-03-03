# AIN212 Course Project

## Contributors:
- Ender Orman (ID: 2210765011)
- Abdullah Edik (ID: 2220765031)

## Introduction:
This repository contains the code for the AIN212 course project. The project focuses on data preprocessing, imputation, exploratory data analysis, and machine learning modeling of airline reviews.

## Requirements:
- Python 3
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, nltk

## Usage:
1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/AIN212-Course-Project.git
    cd AIN212-Course-Project
    ```

2. Run the Python script `main.py` to execute the data preprocessing, imputation, exploratory data analysis, and machine learning modeling steps:

    ```bash
    python main.py
    ```

## Data Collection:
- The data is collected from the provided URL and loaded into a pandas DataFrame.

## Data Preprocessing and Cleaning:
- Missing values are checked and redundant columns are dropped.
- Categorical variables are encoded to binary form and ordinal variables are converted to numerical form.
- Mode imputation is performed for missing variables with no more than 500 missing values.
- KNN classifier imputation is performed for missing variables with more than 500 missing values.

## Data Exploration and Analysis:
- Various exploratory data analysis techniques are applied, including bar plots of categorical columns and analysis of the most common words in review headers.
- Sentiment analysis is conducted using the NLTK library, and sentiment scores are calculated for each review.

## Machine Learning Modeling:
- Correlation matrix and bar plots are generated to visualize the relationships between variables.
- Data is standardized using MinMaxScaler and the Elbow method is used to determine the optimal number of clusters for K-Means clustering.
- Principal Component Analysis (PCA) is performed for dimensionality reduction, and the Elbow method is again used to determine the optimal number of clusters for K-Means clustering on the PCA-transformed data.
- K-Nearest Neighbors (KNN) classifier and Logistic Regression models are trained and evaluated for predicting the 'Recommended' label.
- Receiver Operating Characteristic (ROC) curves are plotted to compare the performance of the models.

## Results:
- Both KNN classifier and Logistic Regression models achieve high rates for precision, recall, and accuracy.
- Logistic Regression slightly outperforms the KNN classifier in terms of the area under the ROC curve.
