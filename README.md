🚀 Telecom Customer Churn Analysis | Power BI + SQL + Python

An end-to-end Customer Churn Analytics Dashboard project designed to analyze customer behavior, identify churn patterns, and generate actionable business insights using Power BI, SQL, Python, and Power Query.

This project transforms raw telecom customer data into an interactive business intelligence solution that helps understand why customers leave, which customer segments are at risk, and how businesses can improve customer retention strategies.

📊 Dashboard Preview

🎯 Project Objective

Customer churn is one of the biggest challenges in subscription-based businesses.
The objective of this project is to:

Analyze customer churn behavior
Identify high-risk customer segments
Discover factors influencing churn
Build interactive dashboards for business decision-making
Generate actionable insights to improve customer retention
⚡ Tech Stack
Tool	Purpose
Power BI	Dashboard Development & Visualization
SQL	Data Cleaning, Exploration & Analysis
Python	Data Processing & Exploratory Analysis
Power Query	Data Transformation & Feature Engineering
Excel/CSV	Data Source
📌 Key Dashboard Features
✅ Executive KPI Overview
Total Customers
Total Churn
Churn Rate
New Joiners
✅ Customer Segmentation Analysis
Churn by Gender
Churn by Age Group
Churn by Tenure Group
Customer Behavioral Insights
✅ Service-Based Churn Analysis
Internet Type Analysis
Streaming Services Analysis
Online Security Impact
Premium Support Impact
✅ Contract & Payment Insights
Contract-wise Churn Trends
Payment Method Analysis
Monthly Charge Range Analysis
✅ Geographic Insights
State-wise Churn Distribution
High Churn Regions
Geographic Performance Comparison
✅ Interactive User Experience
Dynamic Filters
Cross Filtering
Drill-through Analysis
Responsive Dashboard Design
🔍 Key Business Insights

📌 Customers with Month-to-Month Contracts had the highest churn rate.

📌 Customers using Fiber Optic Internet showed significantly higher churn compared to DSL users.

📌 Users without Online Security and Premium Support were more likely to leave the service.

📌 Short-tenure customers showed higher churn probability compared to long-term customers.

📌 Certain geographic regions contributed disproportionately to overall churn.

📌 Customers with higher monthly charges demonstrated increased churn behavior.

🛠️ Data Engineering & Processing
SQL Data Processing

Performed:

Data Cleaning
Null Value Handling
Data Exploration
View Creation
Business Aggregations

Example SQL Query:

SELECT Contract,
       COUNT(Contract) AS TotalCount,
       COUNT(Contract) * 1.0 /
       (SELECT COUNT(*) FROM stg_Churn) AS Percentage
FROM stg_Churn
GROUP BY Contract;
⚙️ Power Query Transformations
Feature Engineering
Created Churn Status Column
Monthly Charge Bucketing
Age Group Mapping
Tenure Group Segmentation
Data Modeling
Unpivoted Service Columns
Created Mapping Tables
Optimized Data Relationships
📈 DAX Measures
Total Customers = COUNT(prod_Churn[Customer_ID])

New Joiners =
CALCULATE(
    COUNT(prod_Churn[Customer_ID]),
    prod_Churn[Customer_Status] = "Joined"
)

Total Churn = SUM(prod_Churn[Churn Status])

Churn Rate = [Total Churn] / [Total Customers]
📂 Project Structure
📁 Telecom-Customer-Churn-Analysis
│
├── 📊 Dashboard
│   ├── Telecom_Churn_Analysis.pbit
│   └── Churn_Dashboard.png
│
├── 📁 Dataset
│   └── Customer_Data.csv
│
├── 📁 SQL
│   └── SQL Queries.docx
│
├── 📁 PowerQuery
│   └── Power Query Transformations & Measures.docx
│
└── README.md
📊 Project Highlights

✔ Built an interactive Power BI dashboard with KPI-driven insights
✔ Processed and analyzed telecom customer data end-to-end
✔ Applied SQL for advanced data exploration and transformation
✔ Designed reusable Power Query transformations and DAX measures
✔ Generated actionable business recommendations from churn behavior analysis

💡 Skills Demonstrated
Data Analytics
Business Intelligence
Power BI Dashboarding
SQL Analytics
Data Visualization
Exploratory Data Analysis (EDA)
KPI Reporting
Customer Segmentation
Data Cleaning & Transformation
Business Problem Solving
📚 Dataset Information
Dataset Source: Kaggle
Domain: Telecom Industry
Records Analyzed: 6,000+ Customer Records
🔗 Connect With Me
👨‍💻 Vangari Akhil
LinkedIn: www.linkedin.com/in/your-link
GitHub: github.com/your-github
