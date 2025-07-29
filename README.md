# Customer Churn Analysis

## Project Overview
This project focuses on analyzing customer churn behavior for a telecommunications company. The goal is to identify the key drivers of churn and develop machine learning models to predict customers who are likely to leave. Understanding churn patterns allows the business to take proactive retention measures and improve overall customer satisfaction and profitability.

## Business Objective
Customer churn directly impacts revenue and long-term growth. By identifying churn-prone customers early, the company can design targeted retention strategies, such as offering discounts, improving customer service, or personalizing plans. This analysis helps answer:

- What demographic and service-based factors influence churn?
- How can these insights support data-driven decision-making?

## Data Overview
The dataset includes 7,000+ customer records with features like:
- Demographics: Gender, SeniorCitizen, Partner, Dependents
- Account Info: Tenure, Contract, Payment Method, PaperlessBilling
- Services: InternetService, StreamingTV, OnlineSecurity, TechSupport
- Charges: MonthlyCharges, TotalCharges
- Target: Churn (Yes/No)

## Exploratory Data Analysis (EDA)

Key findings:
- Contract Type: Month-to-month customers churn the most.
- Senior Citizens: Show slightly higher churn rates.
- Services: Lack of security or support services correlates with churn.
- Tenure: Customers with longer tenure are less likely to churn.
- MonthlyCharges: Higher monthly charges are associated with churn.

Visuals: Stacked bar charts, KDE plots, and correlation maps supported these insights.

## Modeling & Evaluation
Multiple machine learning models were applied using Stratified K-Fold Cross-Validation, including Logistic Regression, Decision Tree, Random Forest, XGBoost, SVM, and K-Nearest Neighbors. Each model was evaluated on its ability to correctly classify customer churn, with a particular focus on recall, as identifying churners is crucial for retention strategies.

**Final Evaluation on Test Set**
- Model retrained on full training data
- Evaluated on hold-out test data
- Metrics printed using a reusable function
- Confusion matrix and classification report included


**Chosen Model:** Although XGBoost showed strong balanced performance, Logistic Regression was ultimately chosen due to its solid recall and interpretability. This makes it an effective and explainable solution for businesses aiming to proactively reduce customer churn.

## Key Insights
- Customers with month-to-month contracts, no tech support, and higher monthly charges are more likely to churn.
- Tenure is one of the strongest indicators — newer customers are more at risk.
- Dependents and Partners seem to reduce churn likelihood, possibly due to higher engagement or shared utility.


## Business Recommendations
- Offer loyalty incentives to new users to extend tenure early.
- Promote annual/biennial contracts with bundled offers.
- Improve technical support and security services as value add-ons.
- Use the churn prediction model to flag high-risk customers for retention teams.










