📌 Project Overview

This project builds a unified analytics pipeline that transforms raw transactional data into meaningful insights.

Key goals:

Understand revenue drivers and trends
Identify high-value customers and segments
Analyze product and seller performance
Detect operational inefficiencies (e.g., delivery delays)
Provide actionable business recommendations

🏗️ Architecture & Workflow
1. Data Integration
Combined multiple relational tables into a single dataset (master_df)
Used left joins to preserve complete order history

Tables used:

Customers
Orders
Order Items
Products
Payments
Reviews
Sellers
Category Translation

👉 The ER diagram (Page 3 of report) shows relationships between these entities.

2. Data Cleaning
Converted timestamps to datetime
Handled missing values from joins
Removed negative delivery times
Ensured consistency across keys
3. Feature Engineering
🔹 Order-Level Features
Total Order Value = price + freight
Delivery Time = delivery date - purchase date
Items per Order
🔹 Customer-Level Features
Purchase Frequency
Customer Lifetime Value (CLV)
Average Order Value (AOV)

📊 Key Insights

👥 Customer Analysis
~93% customers are new users
Only ~7% are repeat customers
25% customers generate 61% of revenue

👉 Insight: Strong need for customer retention strategy

💰 Revenue Trends
Peak sales: October 2017
Growth in 2017 → decline post mid-2018 (possible data cutoff)
📦 Product Analysis

Top categories:

Bed, Bath & Table
Furniture & Decor
Computers & Accessories
Health & Beauty

👉 Sales follow a long-tail distribution

🧑‍💼 Seller Analysis
No single seller dominates (~1.5% each)
Thousands of low-performing sellers
Healthy but long-tail ecosystem

⭐ Reviews & Satisfaction
56% → 5-star reviews
13% → 1-star reviews (high)

📌 Key finding (Page 8):

Bad deliveries take ~7 days longer
Delivery delay is a major driver of poor ratings

🚀 Business Recommendations
1. Customer Retention
Loyalty programs
Post-purchase engagement
Win-back campaigns
Referral incentives
2. High-Value Customers
VIP tiers
Early access sales
Personalized offers
3. Delivery Optimization
Reduce delivery time gap (~7 days)
Set SLA benchmarks (7–10 days)
Regional fulfillment centers
4. Geographic Expansion
Reduce dependency on top states (SP, RJ, MG)
Expand into underpenetrated regions
5. Product Strategy
Focus on top categories
Bundle products
Promote long-tail inventory

🧭 Strategic Roadmap
Priority	Initiative	Timeline	Impact
P1	Reduce delivery time	0–3 months	↓ 1-star reviews
P1	Retention campaigns	0–3 months	↑ repeat customers
P1	VIP loyalty program	0–3 months	Protect revenue
P2	Geographic expansion	3–6 months	Reduce risk
P3	Product optimization	6–12 months	↑ AOV

🛠️ Tech Stack
Python (Pandas, NumPy)
Data Visualization (Matplotlib / Seaborn)
Data Processing
Business Intelligence & Analytics
📁 Project Structure

📦 Ecommerce_Intelligence_Project
 ┣ 📂 dataset            # Raw and processed data files
 ┣ 📂 notebook           # Jupyter notebooks (EDA, feature engineering, analysis)
 ┣ 📜 README.md          # Project documentation

📈 Conclusion

This project demonstrates how data can uncover critical business insights:

Strong acquisition, weak retention
Delivery delays impact satisfaction
Revenue concentrated in few customers & regions

👉 Key takeaway:

Fix delivery, build loyalty, and protect high-value customers to drive long-term growth.
