# House Price Prediction

A machine learning project that predicts house prices using **Linear Regression** on the **USA Housing** dataset.  
This project covers the full beginner-friendly regression workflow, including **exploratory data analysis (EDA)**, **feature preprocessing**, **feature scaling**, **correlation analysis**, **model training**, and **performance evaluation**.

---

## Project Overview

The goal of this project is to build a regression model that can estimate house prices based on important housing features such as:

- Average Area Income
- Average Area House Age
- Average Area Number of Rooms
- Average Area Number of Bedrooms
- Area Population

The project is implemented in a Jupyter Notebook and demonstrates how to move from raw data to a trained and evaluated predictive model.

---

## Dataset

The dataset used in this project is **USA Housing** and contains the following columns:

- `Avg. Area Income`
- `Avg. Area House Age`
- `Avg. Area Number of Rooms`
- `Avg. Area Number of Bedrooms`
- `Area Population`
- `Price`
- `Address`

### Target Variable
- `Price`

### Notes
- `Address` is not useful for numerical regression modeling and is excluded during preprocessing.

---

## Workflow

The notebook follows this pipeline:

1. **Import Libraries**  
   Uses NumPy, Pandas, Matplotlib, Seaborn, and Scikit-learn.

2. **Load the Dataset**  
   Reads the housing dataset into a Pandas DataFrame.

3. **Exploratory Data Analysis (EDA)**  
   - Displays dataset head
   - Checks data types and missing values
   - Generates descriptive statistics
   - Examines feature relationships

4. **Correlation Analysis**  
   Studies how strongly each feature is related to house price.

5. **Feature Preprocessing**
   - Removes unnecessary columns
   - Selects numerical features
   - Applies **StandardScaler** for feature scaling

6. **Train-Test Split**
   - Splits the data into **70% training** and **30% testing**

7. **Model Training**
   - Trains a **Linear Regression** model using Scikit-learn

8. **Prediction & Evaluation**
   - Makes predictions on test data
   - Evaluates model performance using:
     - **R² Score**
     - **Mean Absolute Error (MAE)**
     - **Mean Squared Error (MSE)**

9. **Feature Importance / Selection Exploration**
   - Reviews coefficient values
   - Explores removing weakly correlated features for improvement

---

## Model Performance

The notebook reports the following results:

- **R² Score:** `0.9199`
- **MAE:** `79,912.71`
- **MSE:** `9,831,074,697.74`

### Interpretation
- The model explains about **92% of the variance** in house prices.
- The average prediction error is around **$79.9K**.
- Overall, the model performs well for a basic linear regression baseline.

---

## Tech Stack

- **Python**
- **Jupyter Notebook**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
