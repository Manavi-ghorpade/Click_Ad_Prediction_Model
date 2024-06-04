# Advertising Click Prediction Project

Welcome to the Advertising Click Prediction project! This repository showcases an end-to-end process of data analysis and predictive modeling using various machine learning techniques. The goal is to predict whether a user will click on an advertisement based on certain features like age, area income, and daily internet usage.

## Project Overview

### 1. Data Loading and Initial Exploration
- The dataset `advertising.csv` is read into a Pandas DataFrame.
- Initial exploration includes checking the head of the data and basic info about the dataset.

### 2. Exploratory Data Analysis (EDA)
Visualizations are created using Seaborn and Matplotlib to understand the data distribution and relationships between features.

#### **Histogram of Age**
- Shows that most users are around the age of 30.


#### **Jointplot of Age vs. Area Income**
- Indicates users aged 20-40 belong to areas with higher average income.


#### **Jointplot of Age vs. Daily Time Spent on Site (KDE)**
- Highlights that users aged 25-35 spend more time on the site.


#### **Jointplot of Daily Time Spent on Site vs. Daily Internet Usage**
- Shows users with higher daily internet usage tend to spend more time on the site.


#### **Pairplot with 'Clicked on Ad' Hue**
- Provides insights into feature interactions differentiated by whether the ad was clicked.


### 3. Model Training and Evaluation
- The data is split into training and testing sets using `train_test_split`.
- A Logistic Regression model is trained and evaluated. Different values for the regularization parameter `C` are used to demonstrate overfitting, underfitting, and best fitting models.

#### **Best Fit Model**
- Achieved with `C=0.0001`.

### 4. Additional Models
- A Linear Support Vector Classifier (SVC) is trained and evaluated.

- A Gaussian Naive Bayes classifier is trained and evaluated.

## Key Takeaways
- **Regularization in Logistic Regression**: Demonstrates how adjusting the `C` parameter can prevent overfitting or underfitting, providing the best model performance.
- **Data Visualization**: Highlights the importance of visualizing data to understand underlying patterns and relationships.
- **Model Comparison**: Compares multiple models (Logistic Regression, SVC, Naive Bayes) to evaluate their performance on the same dataset.

## Conclusion
This project demonstrates the full cycle of data exploration, visualization, model training, and evaluation. By adjusting key parameters and comparing different models, it provides a comprehensive understanding of machine learning techniques for binary classification problems.

## Future Work
- Test other machine learning algorithms like Decision Trees and Random Forests.
