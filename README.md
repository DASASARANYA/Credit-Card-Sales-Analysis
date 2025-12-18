# 📊 Credit Card Financial Dashboard (Tableau)

## Project Overview

This project presents an interactive **Credit Card Financial Dashboard** built using **Tableau** to analyze customer demographics, spending behavior, credit utilization, payment risk, and customer satisfaction. The dashboard helps identify high-risk customers, overspending patterns, and opportunities for targeted financial and customer engagement strategies.

---

## Objectives

* Analyze customer spending patterns across expense types
* Evaluate credit utilization and identify potential credit risk
* Understand payment behavior and delinquency trends
* Assess customer satisfaction in relation to financial behavior
* Provide actionable insights for banking and financial decision-making

---

## Data Source

The dataset consists of two sheets:

### 1️⃣ Customer Details Sheet

Contains customer demographic and profile information:

* Client_Num
* Customer_Age
* Gender
* Dependent_Count
* Education_Level
* Marital_Status
* State_Code
* Zipcode
* Car_Owner
* House_Owner
* Personal_loan
* Contact
* Customer_Job
* Income
* Customer_Satisfaction_Score

### 2️⃣ Card Details Sheet

Contains credit card usage and financial behavior data:

* Client_Num
* Card_Category
* Annual_Fees
* Activation_30_Days
* Customer_Acq_Cost
* Week_Start_Date
* Corrected_Week_Start_Date
* Week_Num
* Qtr
* Current_Year
* Credit_Limit
* Total_Revolving_Balance
* Total_Trans_Amount
* Total_Trans_Volume
* Avg_Utilization_Ratio
* Use Chip
* Exp Type
* Interest_Earned
* Delinquent_Account

---

## Data Preparation & Cleaning

* Established a **relationship join** between the two sheets using `Client_Num`
* Corrected data types for numeric, categorical, and date fields
* Standardized categorical values (Gender, Card_Category, Expense Type, etc.)
* Handled missing values in income and satisfaction scores
* Removed duplicates where applicable

---

## Calculated Fields Created

To enhance analysis, the following calculated fields were created in Tableau:

* **Utilization Band** (Low / Medium / High)
* **Overspending Flag** (Over Limit / Within Limit)
* **Income Segment** (Low / Middle / High Income)
* **Age Group** (Under 30, 30–45, 46–60, 60+)
* **Payment Risk Status** (Delinquent / Non-Delinquent)
* **Satisfaction Category** (Low / Medium / High Satisfaction)
* **High Value Customer Flag**

These fields help in segmentation, risk assessment, and customer profiling.

---

## Key Visualizations

The dashboard includes the following visual components:

* **KPI Summary**: Total Customers, Avg Credit Limit, Avg Utilization Ratio, Total Transaction Amount
* **Spending Analysis**: Expense Type vs Total Transaction Amount
* **Credit Utilization Analysis**: Customer distribution by Utilization Band
* **Delinquency Analysis**: Delinquent vs Non-Delinquent customers by card category
* **Demographic Analysis**: Gender-wise and age-wise card usage
* **Customer Satisfaction Analysis**:

  * Satisfaction vs Avg Credit Utilization
  * Satisfaction vs Delinquency
  * Satisfaction vs Average Transaction Amount

---

## Dashboard Features

* Interactive filters for Gender, Card Category, Income Segment, and State
* Clean and intuitive layout for easy navigation
* Beginner-friendly visualizations with clear business interpretation

---

## Key Insights

* Customers with **low satisfaction scores** tend to show **higher credit utilization** and **higher delinquency rates**
* **Middle-income customers** exhibit higher utilization ratios
* **Premium card holders** generate higher transaction values
* Highly satisfied customers contribute more to overall spending

---

## Business Recommendations

* Proactively engage low-satisfaction customers with repayment reminders and offers
* Offer credit limit enhancements to low-risk, high-value customers
* Design targeted campaigns based on expense type and income segment
* Improve customer experience initiatives to reduce delinquency risk

---

## Tools & Technologies

* **Tableau Desktop** (Dashboard creation & analysis)
* **Excel / CSV** (Data source)

---

## How to Use the Dashboard

1. Open the `Credit Card Financial Dashboard.twbx` file in Tableau
2. Use filters to explore customer segments
3. Hover over visuals for detailed tooltips
4. Analyze patterns and insights across demographics and financial behavior
