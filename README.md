# Online-shoppers-purchasing-prediction-with-classification-models.

This project focuses on data cleaning and visualization to explore online shoppers' purchasing behavior on an e-commerce website. The aim is to identify trends, patterns, and insights from user behavior data.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Insights](#insights)
- [Technologies Used](#technologies-used)
- [References](#references)

## Overview

The project uses the **Online Shoppers Purchasing Intention Dataset** to analyze how various user engagement metrics relate to purchasing decisions. The work involves cleaning the dataset to remove errors and inconsistencies, followed by visualizing key patterns to understand user behavior.

## Dataset

- **Source**: UCI Machine Learning Repository
- **Dataset**: Online Shoppers Purchasing Intention Dataset
- **Size**: 12,330 rows × 18 columns
- **Types**: 
  - Categorical: 8
  - Numerical: 10

## Data Cleaning

1. **Outlier Detection and Removal**:
   - Outliers in the `ProductRelated_Duration` feature were identified and removed to improve data reliability.
   
2. **Null Value Handling**:
   - The dataset had no null values, eliminating the need for imputation.

3. **Redundant Data**:
   - Checked for and confirmed the absence of redundant white spaces and formatting inconsistencies.

4. **Encoding Categorical Data**:
   - Converted categorical features into numerical representations for compatibility with machine learning models.

## Exploratory Data Analysis (EDA)

The analysis focused on identifying patterns and trends across various features using visualizations:

1. **Purchase Behavior**:
   - Only **15.47%** of visitors completed a purchase.
   - Purchases were concentrated in specific months (November, May, and December).

2. **Special Days and Weekends**:
   - **96.96%** of purchases were not made on special days.
   - **73.85%** of purchases occurred on weekdays.

3. **Browser and Operating System Preferences**:
   - Browser #2 accounted for **64.1%** of purchases.
   - Operating System #2 was preferred by **60.53%** of purchasers.

4. **Visitor Type**:
   - Returning visitors made up **77.04%** of purchases.

5. **Region Analysis**:
   - Region #1 had the highest percentage of purchasers (**40.41%**).

6. **Feature Relationships**:
   - Positive correlations were found between `PageValues` and `Revenue`.
   - Negative correlations were identified for `BounceRates` and `ExitRates` with `Revenue`.

## Insights

- **High PageValues Drive Purchases**: Visitors are more likely to convert when interacting with high-value pages like checkout and product pages.
- **Returning Visitors Are Key**: Most purchases are made by returning visitors, highlighting the importance of customer retention.
- **Weekend Effect Is Minimal**: Purchases are not significantly skewed toward weekends.
- **Engagement Matters**: Longer durations on informational and product-related pages positively influence purchase likelihood.

## Technologies Used

- **Python**: Data analysis and visualization
- **Pandas & NumPy**: Data cleaning and manipulation
- **Matplotlib & Seaborn**: Visualizations

## References

1. [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php)
2. [Seaborn Correlation Heatmap Guide](https://medium.com/@szabo.bibor/how-to-create-a-seaborn-correlation-heatmap-in-python-834c0686b88e)
3. [Pandas Resample Techniques](https://towardsdatascience.com/pandas-resample-tricks-you-should-know-for-manipulating-time-series-data-7e9643a7e7f3)

