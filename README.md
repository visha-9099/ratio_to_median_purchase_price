📊 Ratio to Median Purchase Price – A Smart Metric for Outlier Detection & Price Analysis
The ratio_to_median_purchase_price project focuses on building a powerful, interpretable, and scalable machine learning pipeline that leverages the ratio of an item’s price to its median purchase price as a central feature. 
This feature engineering technique plays a crucial role in anomaly detection, price optimization, fraud prevention, and customer behavior analysis—particularly in e-commerce, retail, or procurement analytics.

🎯 Objective
The core goal of this project is to explore and model purchasing behavior by calculating and analyzing the ratio between an item’s purchase price and the typical (median) price it’s been bought for historically. 
This can help answer questions such as:

Is a product being sold or purchased significantly above or below its average price?

Are there pricing anomalies that may indicate fraud, promotions, or errors?

Can we build predictive models to forecast demand, price, or anomalies?

📦 Dataset Overview
The dataset typically includes:

Item ID or Product Code

Purchase Price

Transaction Date

Buyer ID or Supplier ID (optional)

Quantity, Category, Region, etc

🔍 Use Cases
Price Anomaly Detection: Flag purchases that deviate significantly from historical norms.

Procurement Intelligence: Identify vendors offering better-than-average deals.

Customer Behavior Analysis: Spot patterns in buying habits and spending efficiency.

Dynamic Pricing Models: Adjust prices based on product volatility or customer thresholds.

🔧 Workflow Overview
Data Cleaning & Preparation

Handle missing values

Normalize product identifiers

Convert transaction dates to datetime objects

Feature Engineering

Compute item-level median purchase prices

Calculate ratio_to_median_purchase_price

Add time-lagged features or grouped statistics (e.g., rolling median)

Exploratory Data Analysis

Distribution of ratios across products and time

Visuals of anomalies (extreme high or low ratios)

Correlations with other transaction variables

Modeling & Analysis

Unsupervised techniques: Isolation Forest, DBSCAN, PCA

Supervised models (if labeled anomalies available): Random Forest, XGBoost

Use of SHAP/LIME to interpret the influence of the ratio feature

Deployment (Optional)

Interactive dashboard (Streamlit or PowerBI)

API for real-time ratio computation

Alerts/threshold system for procurement monitoring

🛠️ Tools & Libraries
Python 3.8+

Pandas, NumPy

Scikit-learn

Matplotlib, Seaborn, Plotly

XGBoost, LightGBM

Streamlit (for dashboard)

SQL (for real-time integrations)

📈 Example Visualization
Visualize how purchase price deviates from the median using time-series or boxplots. Identify spikes in the ratio for real-time anomaly alerts.

🚀 Future Improvements
Integrate with ERP systems or procurement APIs for live monitoring

Apply deep learning for sequence analysis

Improve dynamic thresholding with statistical control limits

Add explainability layer to communicate why a price was flagged

