# Task-1: Exploratory Data Analysis (EDA)

## Overview
This task involves conducting an exploratory data analysis (EDA) to understand the structure and characteristics of the dataset. The analysis will help uncover patterns, relationships, and potential data issues before proceeding with further modeling or decision-making.

## Steps in EDA

### 1. Overview of the Data
- Load the dataset and examine its structure.
- Check the number of rows and columns.
- Identify data types of each feature.

### 2. Summary Statistics
- Compute basic statistics such as mean, median, standard deviation, min, and max values.
- Analyze the distribution shape of numerical features.

### 3. Distribution of Numerical Features
- Visualize the distribution using histograms and density plots.
- Identify patterns, skewness, and potential outliers.

### 4. Distribution of Categorical Features
- Analyze the frequency and variability of categorical variables.
- Use bar plots and count plots for visualization.

### 5. Correlation Analysis
- Compute correlation coefficients between numerical features.
- Visualize relationships using heatmaps and scatter plots.

### 6. Identifying Missing Values
- Detect missing values in the dataset.
- Decide on appropriate imputation strategies (mean, median, mode, or predictive models).

### 7. Outlier Detection
- Use box plots to identify and visualize outliers.
- Decide whether to remove or transform extreme values.

## Tools & Libraries
The following Python libraries will be used for analysis:
- `pandas` for data manipulation
- `numpy` for numerical operations
- `matplotlib` and `seaborn` for visualization
- `scipy` for statistical analysis


# Task-3: Feature Engineering

## Overview
Feature engineering is the process of transforming raw data into meaningful features that improve the performance of machine learning models. This includes creating aggregate features, extracting temporal features, encoding categorical variables, handling missing values, and normalizing numerical data.

## Steps in Feature Engineering

### 1. Create Aggregate Features
- **Total Transaction Amount**: Sum of all transaction amounts for each customer.
- **Average Transaction Amount**: Average transaction amount per customer.
- **Transaction Count**: Number of transactions per customer.
- **Standard Deviation of Transaction Amounts**: Variability of transaction amounts per customer.

### 2. Extract Features
- **Transaction Hour**: The hour of the day when the transaction occurred.
- **Transaction Day**: The day of the month when the transaction occurred.
- **Transaction Month**: The month when the transaction occurred.
- **Transaction Year**: The year when the transaction occurred.

### 3. Encode Categorical Variables
- **One-Hot Encoding**: Converts categorical values into binary vectors.
- **Label Encoding**: Assigns a unique integer to each category.

### 4. Handle Missing Values
- **Imputation**: Filling missing values using:
  - Mean
  - Median
  - Mode
  - KNN imputation
- **Removal**: Dropping rows or columns with missing values if they are sparse.

### 5. Normalize/Standardize Numerical Features
- **Normalization**: Scales data to a range of [0,1].
- **Standardization**: Scales data to have a mean of 0 and a standard deviation of 1.

## Weight of Evidence (WOE) and Information Value (IV)
- **Weight of Evidence (WOE)**: Measures the predictive power of a categorical feature.
- **Information Value (IV)**: Helps identify the most predictive features.

## Expected Outcomes
- Improved dataset with meaningful features.
- Reduced dimensionality and better feature selection.
- Enhanced model performance through transformed and encoded features.

# Tak-4: Credit Scoring System using RFMS

## Overview
The objective of this credit scoring system is to classify users into **high-risk (bad)** and **low-risk (good)** groups using the **RFMS (Recency, Frequency, Monetary, and Stability)** formalism. High-risk users have a high likelihood of default, meaning they fail to pay their loan principal and interest on time.

## Steps to Construct the Default Estimator

### 1. Visualize Transactions in RFMS Space
- Plot all transactions in the **RFMS** space.
- Establish a **boundary** to classify users into high and low RFMS scores.
- Users with **high RFMS scores** are classified as **good** (low-risk), while those with **low RFMS scores** are classified as **bad** (high-risk).

### 2. Assign User Labels
- Based on RFMS scores, assign users the labels:
  - **Good (Low-Risk)**: Users with high RFMS scores.
  - **Bad (High-Risk)**: Users with low RFMS scores.

### 3. Perform Weight of Evidence (WoE) Binning
- Apply **Weight of Evidence (WoE) binning** to transform categorical and continuous features for better predictive modeling.
- WoE helps in quantifying risk and improving model interpretability

## Implementation
### Install Dependencies

## Expected Outcomes
- A **default estimator (proxy)** that classifies users into **good** and **bad** credit risk categories.
- Visual representations of transactions in **RFMS space**.
- Optimized features using **WoE binning**.
- A robust dataset for training predictive models for credit risk assessment.

