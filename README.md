💰 SpendLens – Student Expense Analytics Dashboard

```
📌 Overview
```
SpendLens is a data analytics and visualization project built using Power BI to help students track, analyze, and optimize their spending behavior. The dashboard provides actionable insights into financial habits, helping users make better budgeting decisions.

This project focuses on real-world financial analysis, transforming raw transaction data into meaningful insights such as spending patterns, category distribution, and savings feasibility.

Expense tracking systems help users “record, categorize, and analyze expenses to make informed financial decisions.”
```
🎯 Objectives
Analyze student spending behavior
Identify high-expense categories
Detect spending patterns (daily, weekly, monthly)
Evaluate savings feasibility
Provide actionable recommendations
```
```
🛠️ Tools & Technologies
Power BI – Dashboard & visualization
Python (Pandas, NumPy) – Data cleaning (optional)
Excel/CSV Dataset – Transaction data
DAX (Data Analysis Expressions) – Measures & calculations
```
```
📂 Dataset Description

The dataset contains student transaction details such as:

Date
Amount
Category (Food, Transport, Utilities, etc.)
Merchant Name
Payment Mode
📊 Key Features
📌 1. KPI Metrics
Total Spending
Monthly Average Spending
Top Spending Category
📊 2. Spending Analysis
Category-wise breakdown
Share of wallet (Donut chart)
Monthly spending trend
Day-wise spending behavior
🔍 3. Advanced Insights
Highest & lowest spending day/month
Weekend vs weekday spending
Merchant-level analysis
Payment mode distribution
Average transaction value
📈 4. Advanced Visuals
Heatmap (Week vs Day spending)
Running total (cumulative spending)
Budget vs actual (Gauge chart)
Treemap (Category → Merchant hierarchy)
💡 5. Smart Insights
Spending concentration analysis
Behavioral patterns (weekend overspending)
Savings feasibility check
Dynamic recommendations
🎛️ 6. Interactive Features
Filters (Month, Category, Day)
What-if parameter for savings projection
Dynamic insight generation using DAX
⚙️ Key DAX Measures
Total Spent = SUM(cleaned_transactions[Amount])

Monthly Avg = 
AVERAGEX(
    VALUES(cleaned_transactions[Month]),
    CALCULATE([Total Spent])
)

Savings = 15000 - [Monthly Avg]

Savings Status = 
IF(
    [Savings] < 0,
    "⚠ Not Feasible",
    "✔ Feasible"
)
```
📊 Sample Insights
Majority of spending is concentrated in Utilities and Food categories
Weekend spending is higher, indicating lifestyle-driven expenses
Spending exceeds income, making savings goals unachievable
A reduction in discretionary expenses can improve savings

```
```
🚀 How to Use
Open Power BI Desktop
Load the dataset (cleaned_transactions.csv)
Apply transformations (date, month, day columns)
Create DAX measures
Build visuals and dashboard
Interact using filters and slicers
```
```
🏆 Project Highlights
Real-world financial analytics problem
Strong use of DAX for insights
Interactive and dynamic dashboard
Business-focused recommendations
```
```
📈 Future Enhancements
Integration with real-time expense APIs
Mobile-friendly dashboard
AI-based expense prediction
Personalized budgeting suggestions
```
```
👩‍💻 Author

Meghana B U
Final Year Engineering Student

⭐ Conclusion

SpendLens is not just a visualization project — it is a decision-support system that helps users understand their financial behavior and take actionable steps toward better money management.
