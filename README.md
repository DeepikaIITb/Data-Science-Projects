https://www.kaggle.com/code/deepika125/data-profiler-for-business-strategy

UPI Transaction Insights (Advanced EDA + Feature Engineering)
This project performs a deep exploratory data analysis (EDA) and feature engineering workflow on a synthetic dataset simulating UPI transactions in India.
The primary goal is to extract meaningful business and behavioral insights, not to build prediction models.

Dataset Overview:
The dataset consists of ~250,000 transactions generated to reflect real-world UPI transaction behavior.
It includes various dimensions like:
Transaction Types (P2P, P2M, Bill Payment, Recharge)
Merchant Categories (Grocery, Food, Shopping, etc.)
Transaction Amounts (₹10 to ₹40,000+)
Demographics (Sender/Receiver Age Group, State)
Device Type, Network Type
Banks involved in transactions
Fraud Flag (0.2% fraud base rate)
Temporal Features (timestamp, day of week, hour of day, is_weekend)

Data Preprocessing and Feature Engineering:
Datetime Features: Extracted month, week_of_year, is_peak_hour, and is_night from timestamps for behavioral analysis.

Categorical Encoding:
transaction_status encoded as {SUCCESS: 1, FAILED: 0}.
day_of_week mapped as {Monday: 0, ..., Sunday: 6}.
transaction_type, merchant_category, device_type, network_type, sender_state, sender_bank, and receiver_bank encoded using either label encoding or one-hot encoding.
Age Group Encoding: sender_age_group and receiver_age_group mapped numerically from 0 to 4 based on predefined age bins
Amount Transformation: log_amount feature created using log1p transformation to handle right-skewed distribution.
Fraud Flag: Kept as binary label for insight extraction (not modeling).

Key Business Insights:
95% transactions are successful; 5% failed.
Fraud is extremely rare (0.2%), but most frequent in P2P and Grocery transactions.
Fraud peaks between 6–9 PM; minimal activity overnight.
36–45 age group transacts highest amounts; young (18–25) and seniors (56+) transact less.
Android dominates device usage (~75%); 4G and 5G dominate networks.
SBI leads banking share (25%), followed by HDFC and ICICI.
No major seasonal patterns; steady transaction volume year-round.

Key Learnings:
Advanced EDA helps uncover rich behavioral patterns even without model building.
Categorical encoding and feature extraction are essential before any modeling.
Right-skewed financial data often benefits from log transformations.
Time-of-day and merchant category provide strong insights for operational and fraud risk teams.
The dataset is well-suited for reporting, fraud analysis, and customer segmentation studies.

Tools & Libraries:
Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)

EDA, feature engineering, and visualization performed without predictive modeling.

📌 Maintained by:
Deepika Yadav (deepikayadaviit@gmail.com)
