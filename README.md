# 📊 Telco Customer Churn Analysis

## 📌 Business Problem

Customer churn is a major challenge for telecommunication companies because losing customers directly impacts revenue and profitability.

The objective of this project is to identify the factors associated with customer churn and provide actionable recommendations to improve customer retention.

---

## 🎯 Project Objectives

- Analyze customer churn behavior
- Identify the strongest churn drivers
- Explore customer characteristics associated with churn
- Create custom features to better understand churn risk
- Generate business recommendations to improve retention

---

## 🛠 Tools & Technologies

- Python 
- Pandas 
- NumPy 
- Matplotlib 
- Seaborn
- Jupyter Notebook 

---

## 📂 Dataset

Dataset: Telco Customer Churn

The dataset contains information about 7,043 customers, including:

- Customer demographics
- Internet services
- Contract details
- Billing information
- Customer churn status

Target Variable:

```text
Churn
```

- Yes → Customer left the company
- No → Customer stayed

---

## 🧹 Data Cleaning

The following cleaning steps were performed:

- Checked dataset structure and data types
- Identified invalid values in TotalCharges
- Replaced blank values with NaN
- Converted TotalCharges from object to float
- Verified dataset consistency

---

## 📈 Exploratory Data Analysis

The following business questions were investigated:

### 1. What percentage of customers churned?

Result:

- 26.5% of customers churned
- 73.5% remained with the company

---

### 2. How does contract type affect churn?

Key Finding:

Customers with Month-to-Month contracts exhibit substantially higher churn rates than customers with longer-term contracts.

---

### 3. How does customer tenure affect churn?

Key Finding:

Customers who churn typically have much shorter tenure compared with retained customers.

---

### 4. Do higher monthly charges increase churn risk?

Key Finding:

Churned customers tend to have higher monthly charges on average.

---

### 5. Does internet service type influence churn?

Key Finding:

Fiber Optic customers show significantly higher churn rates than DSL customers.

---

### 6. Does technical support reduce churn?

Key Finding:

Customers without technical support are substantially more likely to churn.

---

## ⚙️ Feature Engineering

### ServiceCount Feature

A custom feature was created to measure the number of active services used by each customer.

Finding:

Customers subscribed to more services generally exhibit lower churn rates.

---

### HighRiskProfile Feature

A custom High-Risk Profile was created based on:

- Month-to-Month Contract
- Fiber Optic Internet
- No Technical Support

Finding:

Customers matching this profile exhibited a churn rate of:

```text
57.5%
```

compared with:

```text
15.9%
```

for all other customers.

---

## 🔍 Key Findings

- Contract type is one of the strongest churn drivers.
- Customer tenure is strongly associated with retention.
- Fiber Optic customers show elevated churn risk.
- Technical support significantly reduces churn.
- Customers using more services are less likely to churn.
- A custom High-Risk Profile successfully identified a highly vulnerable customer segment.

---

## 💡 Business Recommendations

### 1. Encourage Long-Term Contracts

Promote annual and multi-year contracts to reduce churn.

### 2. Increase Technical Support Adoption

Encourage customers to use support services through onboarding and promotional campaigns.

### 3. Focus on High-Risk Customers

Prioritize retention initiatives for customers matching the High-Risk Profile.

### 4. Promote Additional Services

Cross-sell relevant services to increase customer engagement and retention.

---

## 📊 Visualizations

The project includes:

- Churn Distribution
- Contract vs Churn
- Tenure vs Churn
- Monthly Charges vs Churn
- Internet Service vs Churn
- Technical Support vs Churn
- Service Count vs Churn
- High Risk Profile vs Churn

---

## 📂 Project Structure

```text
Telco-Customer-Churn-Analysis/
│
├── Telco_Customer_Churn_Analysis.ipynb
├── README.md
├── images/
└── data/
```

---

## 🚀 Conclusion

Customer churn is primarily associated with contract type, tenure, technical support adoption, and internet service type.

The analysis demonstrates how exploratory data analysis and feature engineering can be used to uncover actionable business insights and support customer retention strategies.
