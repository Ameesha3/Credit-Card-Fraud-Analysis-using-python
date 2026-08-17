# 🕵️ Fraud Transaction Analysis

## 📌 Executive Summary
This project analyzes transactional datasets to uncover fraud patterns across **amount bands, transaction types, and hourly activity**.  
The analysis highlights fraud hotspots, risky transaction ranges, and time-based vulnerabilities.  
It provides actionable insights for financial institutions to strengthen fraud detection systems and reduce financial losses.

---

## 🎯 Business Problems & Objectives
### Business Problems
- Fraudulent transactions are difficult to detect in real-time.  
- Mid-range transactions often go unnoticed but contribute significantly to fraud losses.  
- Fraud activity spikes at specific hours, making monitoring inconsistent.  

### Objectives
- Identify **fraud-prone transaction ranges**.  
- Compare **legitimate vs fraudulent transaction behavior**.  
- Detect **time-based fraud patterns**.  
- Provide **business insights** for fraud prevention strategies.  



## 📂 Data Source & Preparation
- **Datasets Used**:
  - `amount_band_analysis.csv` → Fraud rate by transaction amount bands  
  - `amount_by_transaction_type.csv` → Legitimate vs Fraud transaction distribution  
  - `hourly_transaction_analysis.csv` → Hourly fraud trends  
  - `top_20_fraud_transactions.csv` → Largest fraud transactions  
  - `top_20_transactions.csv` → Largest legitimate transactions  

- **Preparation Steps**:
  - Cleaned CSV files using **Pandas**.  
  - Calculated fraud rates, averages, and totals.  
  - Aggregated data by **amount bands, transaction type, and hourly slots**.  
  - Prepared datasets for visualization in **Python**.  



## 🛠 Tech Stack & Tools
- **Python** → Data cleaning & analysis  
- **Pandas / NumPy** → Data manipulation  
- **Matplotlib / Seaborn** → Visualization   
- **CSV datasets** → Raw input files  


## 🔎 Exploratory Data Analysis (EDA) & Key Insights
- **Fraud by Amount Band** → Mid-range transactions (₹500–₹1000) show the highest fraud rate (~0.40%).  
- **Transaction Type** → Fraud transactions are fewer but have higher average amounts (₹123 vs ₹88).  
- **Hourly Trends** → Fraud peaks between **2 AM – 4 AM**, suggesting night-time vulnerability.  
- **Top Transactions** → Legitimate transactions reach ₹25,691, while fraud maxes at ₹2,125.  



## 📊 Business Impact
- Enables banks to **flag suspicious mid-range transactions**.  
- Supports **time-based monitoring** (late-night hours).  
- Provides datasets ready for **dashboard visualization**.  
- Can be extended into **machine learning models** for fraud prediction.  


## 🚀 How to Run the Program
1. Clone the repository:
   ```bash
   git clone https://github.com/Ameesha3/fraud-analysis.git
