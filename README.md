# Wine Quality Prediction Model

## Overview
This project aims to predict wine quality based on various attributes using machine learning techniques. Three classification models are implemented and evaluated for their ability to classify wine as either good or bad quality.

## Dataset
The dataset used is "winequality-red" sourced from Kaggle, containing various attributes of red wine samples along with quality ratings.

## Tools and Technologies
- RapidMiner for data preprocessing, model building, and evaluation.
- Python (optional) for additional analysis and visualization.

## Model Development Process

### Step 1: Data Import and Cleaning
- Import the dataset into RapidMiner.
- Remove missing values using the "Filter Example" operator.

### Step 2: Data Transformation
- Generate a new attribute "Grade" based on wine quality:
  - 0 for bad quality (quality <= 6)
  - 1 for good quality (quality > 6)
- Convert the Grade attribute to binomial data type.
- Normalize numerical data to standardize between 0 and 1.

### Step 3: Model Building
- Split the cleaned data into training (80%) and testing (20%) sets.
- Build three classification models:
  - Logistic Regression
  - Random Forest
  - Gradient Boosted Trees

### Step 4: Model Evaluation and Scoring
- Apply trained models to the test data.
- Evaluate model performance metrics:
  - Accuracy
  - Precision
  - Recall
  - ROC-AUC

### Step 5: Cross Validation and ROC Analysis
- Perform cross-validation to validate model accuracy and robustness.
- Compare ROC curves to assess classification performance.

### Step 6: Feature Importance and Correlation Analysis
- Analyze feature importance and attribute correlations using the "Correlation Matrix" operator.

## Results
- Each model's performance metrics are compared and analyzed.
- Insights into feature importance and correlations provide understanding of wine quality factors.
