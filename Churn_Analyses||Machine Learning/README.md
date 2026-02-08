📊 Customer Churn Analysis & Prediction

End-to-End Analytics, BI & Machine Learning Project

🔗 Live Dashboard

👉 View Power BI Report

📌 Project Overview

This project demonstrates an end-to-end customer churn analytics pipeline, going beyond traditional dashboards by integrating data engineering, business intelligence, and machine learning.

The goal was not only to understand why customers churned, but also to predict which customers are most likely to churn in the future and provide insights that support data-driven retention strategies.

🚧 Constraints That Became Learning Opportunities

This project was developed entirely using Power BI Web (Service) on macOS, without access to Power BI Desktop. This introduced real-world constraints such as:

No “Enter Data” option

Limited UI compared to Desktop

Semantic modeling directly in the service

Strict handling of data types and aggregations

Rather than working around these limitations, they were used as learning opportunities to gain a deeper understanding of:

Semantic models vs visuals

Data grain and aggregation behavior

Implicit vs explicit measures

Relationship management in Power BI Service

🔄 End-to-End Data Pipeline
1️⃣ Data Source

Customer churn data stored in Azure SQL Database

2️⃣ Data Engineering

Data cleaning and preparation in Azure SQL

Analytical views created for reporting

Export of ML-ready datasets

3️⃣ Machine Learning (Python)

Used Python for churn prediction:

Data preprocessing with pandas

Model training with scikit-learn

Prediction of future churn likelihood

Generated churn probabilities and predictions

Exported prediction results as CSV

4️⃣ Business Intelligence (Power BI)

Integrated prediction results back into Power BI

Built a two-page interactive dashboard:

Page 1: Descriptive churn analysis

Page 2: Predictive churn analysis

📊 Dashboard Pages
🔹 Page 1 – Churn Analysis Summary

Total customers

New joiners

Total churn

Churn rate

Churn by:

Demographics

Contract type

Payment method

Internet and service usage

Geography

🔹 Page 2 – Churn Prediction & Insights

Predicted churners

Churn probability distribution

High-risk customer identification

Service-level insights for retention

Actionable insights on what to improve to reduce churn

🧠 Key Takeaway

This project goes beyond visualization by answering:

What happened? (Descriptive analytics)

Why did it happen? (Diagnostic analytics)

Who is likely to churn next? (Predictive analytics)

🛠 Technology Stack

Azure SQL Database

Power BI Service (Web)

Power BI Semantic Modeling

DAX (Measures & Calculations)

Python

pandas

scikit-learn

Machine Learning (Churn Prediction)


🚀 What This Project Demonstrates

End-to-end analytics thinking

Strong understanding of BI semantics

Ability to work within platform constraints

Integration of ML outputs into BI tools

Focus on actionable business insights

📬 Feedback & Collaboration

Feedback, suggestions, and collaboration ideas are always welcome.
Feel free to open an issue or connect with me on LinkedIn.
