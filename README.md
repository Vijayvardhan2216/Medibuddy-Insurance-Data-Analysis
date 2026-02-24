# Medibuddy-Insurance-Data-Analysis
An Exploratory Data Analysis and Machine Learning project identifying key drivers of insurance claims to enable risk-based pricing and wellness incentives.

**Project Overview :-** This project conducts an in-depth Exploratory Data Analysis (EDA) and Machine Learning initiative on the MediBuddy insurance dataset. The primary goal is to identify the key demographic, lifestyle and health factors that significantly influence medical insurance claim amounts. The insights derived from this analysis and the developed predictive model are intended to support the company in implementing data-driven policy pricing, accurate risk assessment and effective wellness-based incentive programs.

**Objective:** To analyze MediBuddy insurance data to identify the key factors influencing medical insurance claim amounts. The analysis aims to support data-driven decisions for policy pricing, risk assessment and wellness-based incentives, ultimately leading to a more profitable and fair underwriting process.

**Key Findings:** The analysis of the insurance dataset revealed that lifestyle and health factors are the strongest predictors of high insurance costs, with a machine learning model achieving an R² score of 0.86. The service failures (high claims) are concentrated around specific risk profiles:

| Factor | Primary Issue | Root Cause | Impact on Charges | Model Metric |
| --- | --- | --- | --- | --- |
| **Smoking Status** | High Claim Payouts | Lifestyle Choice | **2–3x higher** claims than non-smokers. | Strongest Predictor |
| **BMI** | Increased Medical Expenses | Health Condition (Obesity) | Strong positive correlation; Obese individuals have significantly higher average charges. | High Correlation |
| **Age** | Gradual Cost Increase | Natural Aging Process | Consistent, gradual increase in claims, especially after middle age. | Moderate Correlation |
| **Gender** | Minimal Impact | No statistical difference | Should not be used as a policy constraint. | Low Correlation |

**Actionable Recommendations :-**

Based on the root causes identified, the following targeted interventions are recommended to balance profitability and fairness:

**1. Implement Risk-Based Pricing**

- **Dynamic Pricing:** Use smoking status and BMI as the primary factors for premium calculation, as they are the strongest predictors of high claims.

- **Predictive Model Integration:** Deploy the Random Forest Regressor model to enable dynamic, accurate and personalized premium estimation for new customers.

**2. Promote Wellness and Preventive Health**

- **Wellness Incentives:** Offer health-based discounts and incentives to customers with normal BMI and non-smoking status to encourage preventive health measures and reduce future claim risk.

**3. Ensure Fair Underwriting**

- **Non-Discriminatory Policy:** Avoid using gender as a factor in policy approval or pricing, aligning with the finding that it has minimal impact on claim costs.

**Methodology and Tools :-**

The analysis followed a structured Exploratory Data Analysis (EDA) approach, culminating in a Machine Learning model for prediction.

**1. Data Wrangling:** Merging two datasets (personal and health data) on 'Policy no.', renaming columns, standardizing categorical values and handling duplicates/missing values.

**2. Exploratory Analysis (UBM Rule):** Conducting Univariate, Bivariate, and Multivariate analysis to understand data distributions, variable relationships and the impact of factors like smoking and BMI on the target variable (Charges).

**3. Feature Engineering & Modeling:** Categorical variables were encoded and a Random Forest Regressor was trained and evaluated using R² and MAE.

**Tools Used:**

- **Python:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Jupyter Notebook:** For data processing and visualization logic.
- **Excel:** For initial data inspection and validation.

**Conclusion :-** The analysis highlights that MediBuddy's operational challenges are primarily due to predictable health and lifestyle risk factors rather than random chance. By leveraging these insights, the company can significantly improve profitability, customer satisfaction and long-term sustainability through risk-based pricing and proactive health promotion.