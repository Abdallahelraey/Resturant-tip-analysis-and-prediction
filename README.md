# Resturant Tips Analysis and Prediction
![download (1)](https://github.com/Abdallahelraey/Tip-prediction/assets/101267806/f6b5abbe-0d67-4e5c-b5b6-171084f30340)


# Restaurant Tips Optimization Project

Welcome to our Restaurant Tips Optimization Project! This project aims to enhance restaurant services and optimize earnings through data analysis and machine learning. Below is a comprehensive guide to the project, highlighting key findings, conclusions, and the modeling process.


# Tip Dataset Key Features

## Overview
- Source: tip.csv file
- Contains 244 rows/samples of tipping data 

## Features
- `total_bill`: the total bill amount
- `tip`: tip amount paid
- `sex`: gender of bill payer (Male/Female)
- `smoker`: whether the bill payer is a smoker (Yes/No)  
- `day`: day of week
- `time`: meal time
- `size`: size of dining party  

## Key Insights
- Provides detailed tipping data across different parties, days, and meal times
- Can analyze differences in tipping behavior by party size, gender, smoking status, and time/day
- Useful for food service business insights and modeling tip percentage prediction

## Project Objectives

1. **Data Analysis:**
   - Explore restaurant tips data.
   - Uncover insights to optimize restaurant processes.

2. **Machine Learning Model:**
   - Develop a model predicting tips based on various factors.
   - Support restaurant owners and staff in improving services and earnings.

## Project Structure

### 0. Problem framing.
### 1. Importing necessary libraries and needed dependencies.
### 2. Data Collection
### 3. Data Preprocessing
### 4. Exploratory Data Analysis
### 5. Feature engineering
### 6. Model engineering



## Key Insights from Data Analysis

1. **Customer Demographics:**
   - The restaurant attracts more male customers than females.
   - Non-smokers significantly outnumber smokers.

2. **Day-wise Analysis:**
   - Saturdays, Sundays, and Thursdays observe higher customer turnout.
   - Fridays have lower attendance, while Mondays, Tuesdays, and Wednesdays are missing data.

3. **Meal Preference:**
   - Dinner is more popular than lunch.
   - Right-skewed total_bill distribution suggests a diverse customer base.

4. **Tip Distribution:**
   - Right skewness in tip amounts implies potential for tip pooling policies.
   - Majority of tables host around 2 customers.

## Key Conclusions from Data Analysis

1. **Tipping Behavior:**
   - Male customers tend to be higher tippers.
   - High tippers prefer dinner service.

2. **Smoking Customers:**
   - Smoking customers do not significantly impact tip amounts.

3. **Tip Policy Recommendation:**
   - Suggested tip range: $1 to $10, with an average of $3.

4. **Dining Timing:**
   - Male customers prefer early-week dining.

5. **Customized Menu Consideration:**
   - Customer groups mainly consist of dinner companions, suggesting a need for a tailored menu.

6. **Total Bill and Table Size Influence:**
   - Both total bill and table size positively impact tip amounts.

## Key Considerations about Our Data

1. Assumption of data representativeness.
2. Ignored limitations, e.g., missing days and assumed absence of breakfast menu.

## Feature Engineering

- Log-transforming tip data to mitigate extreme tipping behavior's impact.
- Feature scaling to ensure equal influence of variables on the model.

## Modeling

1. **Baseline Model (The mean):**
   - MAE: 0.8184

2. **RandomForestRegressor Model:**
   - MAE: 0.5788
   - Outperforms the baseline, showcasing its ability to capture complex relationships.

## Evaluation Results

- **Baseline Model:**
  - Predicts tips based on the mean tip value.
  - MAE: 0.8184

- **RandomForestRegressor Model:**
  - Outperforms the baseline.
  - MAE: 0.5788

The RandomForestRegressor model demonstrates superior predictive accuracy, making it a valuable tool for optimizing restaurant tips.

## Conclusion

This project provides actionable insights and a robust machine learning model to optimize restaurant tips, benefiting both owners and staff. Future improvements may involve refining data assumptions and exploring additional features for model enhancement.
