# Modeling-Car-Insurance-Claim-Outcomes

# Overview/Introduction

Car insurance is a critical component of the automotive industry, with insurance companies investing significant resources in optimizing pricing and accurately predicting the likelihood of claims. This project focuses on building a simple yet effective model to predict whether a customer will make a claim on their car insurance during the policy period. The goal is to identify the single most predictive feature to help On the Road Car Insurance start with a simple model in production.

# Objectives

1. Identify the most predictive feature for determining whether a customer will make a car insurance claim.
2. bBuild a logistic regression model to evaluate the predictive power of individual features.
3. Provide actionable insights to help the insurance company optimize its pricing and risk assessment strategies.

# Data Source

The dataset, car_insurance.csv, contains the following columns:
  - id: Unique client identifier.
  - age: Client's age group (0: 16-25, 1: 26-39, 2: 40-64, 3: 65+).
  - gender: Client's gender (0: Female, 1: Male).
  - driving_experience: Years of driving experience (0: 0-9, 1: 10-19, 2: 20-29, 3: 30+).
  - education: Client's education level (0: No education, 1: High school, 2: University).
  - income: Client's income level (0: Poverty, 1: Working class, 2: Middle class, 3: Upper class).
  - credit_score: Client's credit score (between 0 and 1).
  - vehicle_ownership: Vehicle ownership status (0: Financing, 1: Owned).
  - vehicle_year: Year of vehicle registration (0: Before 2015, 1: 2015 or later).
  - married: Marital status (0: Not married, 1: Married).
  - children: Number of children.
  - postal_code: Client's postal code.
  - annual_mileage: Number of miles driven annually.
  - vehicle_type: Type of car (0: Sedan, 1: Sports car).
  - speeding_violations: Number of speeding violations.
  - duis: Number of driving under the influence (DUI) incidents.
  - past_accidents: Number of past accidents.
  - outcome: Whether the client made a claim (0: No claim, 1: Made a claim).

# Tools Used

- Python Libraries: Pandas, NumPy, Statsmodels
- Modeling: Logistic regression for feature evaluation.
- Data Analysis: Handling missing values, feature selection, and accuracy calculation.

# Insights

1. Feature Importance:
    - The feature driving_experience has the highest predictive power, with an accuracy of 77.71%.
    - Other features like age, credit_score, and past_accidents also show moderate predictive power.
2. Missing Values:
    - The dataset contains missing values in columns like credit_score and annual_mileage, which were filled with the mean values for analysis.
3. Model Performance:
    - Logistic regression models were built for each feature, and their accuracies were compared to identify the best predictor.

# Key Findings

1. Best Predictive Feature:
    - Driving experience is the most predictive feature, with an accuracy of 77.71%.
2. Other Notable Features:
    - Age and past_accidents also show strong predictive power, with accuracies of 77.47% and 74.25%, respectively.
3. Model Simplicity:
    - A single-feature logistic regression model using driving_experience provides a simple yet effective solution for predicting insurance claims.

# Recommendations

1. Focus on Driving Experience:
    - Use driving_experience as the primary feature for initial model deployment, as it provides the highest accuracy.
2. Further Model Development:
    - Explore combining driving_experience with other features like age and past_accidents to improve model performance.
3. Data Collection:
    - Ensure accurate and complete data collection for features like credit_score and annual_mileage to enhance model accuracy.
4. Risk Assessment:
    - Use insights from the model to adjust insurance premiums and risk assessments based on driving experience and other key factors.

# How to Use This Repository

1. Clone the repository.
2. Install the required Python libraries (pandas, numpy, statsmodels).
3. Run the Jupyter Notebook (Modeling Car Insurance Claim Outcomes.ipynb) to reproduce the analysis.
4. Explore the dataset and modify the code to conduct further analysis or build more complex models.
