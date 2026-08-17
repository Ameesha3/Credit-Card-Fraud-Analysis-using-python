# 💳 Credit Card Transaction & Fraud Analytics

## 📌 Project Overview

This project performs an exploratory analysis of credit card transactions using Python to identify transaction patterns, fraudulent activity, high-value transactions, and potential fraud-risk indicators.

The project demonstrates how data analysts can use transaction data to generate meaningful business insights and support financial fraud-monitoring decisions.

## 🎯 Business Objective

Credit card fraud can result in significant financial losses for banks and customers. Analyzing transaction behavior can help financial institutions identify unusual patterns and improve fraud-monitoring strategies.

This project aims to answer:

* What is the total transaction volume and value?
* What is the average transaction amount?
* What percentage of transactions are fraudulent?
* How does fraud transaction value compare with legitimate transactions?
* Which hours have the highest transaction activity?
* Which hours show higher fraud rates?
* Which transaction amount ranges have higher fraud rates?
* What are the highest-value transactions?
* Which anonymized features show stronger relationships with fraud?



## 📊 Dataset

The dataset contains **284,807 credit card transactions**.

### Dataset Features

| Column     | Description                          |
| ---------- | ------------------------------------ |
| `Time`     | Seconds elapsed between transactions |
| `V1`–`V28` | Anonymized transaction features      |
| `Amount`   | Transaction amount                   |
| `Class`    | Transaction classification           |

### Target Variable

* `0` → Legitimate transaction
* `1` → Fraudulent transaction

### ⚠️ Dataset Limitation

The dataset does **not** contain:

* Customer ID
* Age
* Gender
* State/Region
* Income group
* Merchant
* Merchant category
* Card type
* Minimum due
* Total due
* Late fees

Therefore, these fields have **not been artificially created or assumed** in the analysis.



## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook / VS Code**



## 🔍 Project Workflow

### 1. Data Loading

Loaded the credit card transaction dataset using Pandas.

### 2. Data Cleaning

Performed:

* Missing-value checks
* Duplicate-value checks
* Data-type inspection
* Duplicate removal

### 3. Feature Engineering

Created additional features including:

* Transaction hour
* Transaction time in hours
* Log-transformed transaction amount
* Transaction type
* Transaction amount bands

### 4. KPI Analysis

Calculated important business KPIs:

* Total Transactions
* Total Transaction Value
* Average Transaction Amount
* Fraud Transactions
* Fraud Rate
* Fraud Transaction Value
* Fraud Amount Share

### 5. Fraud Analysis

Compared legitimate and fraudulent transactions based on:

* Transaction count
* Total transaction value
* Average transaction amount
* Median transaction amount
* Maximum transaction amount

### 6. Time Analysis

Analyzed transaction behavior by hour to identify:

* Peak transaction hours
* Transaction value by hour
* Fraud count by hour
* Fraud rate by hour

### 7. Amount Analysis

Transactions were divided into different amount ranges:

* 0–10
* 10–50
* 50–100
* 100–250
* 250–500
* 500–1000
* 1000+

Fraud rates were then compared across these transaction ranges.

### 8. High-Value Transaction Analysis

Identified:

* Top 20 highest-value transactions
* Top 20 highest-value fraudulent transactions

### 9. Correlation Analysis

Analyzed relationships between anonymized transaction features and the fraud classification using a correlation matrix.


## 📈 Key Visualizations

The project generates several visualizations:

### Transaction Value by Hour

Shows how transaction value changes throughout the day.

### Fraud Rate by Hour

Highlights hours with comparatively higher fraudulent transaction rates.

### Transaction Amount Distribution

Compares the transaction amount distribution between legitimate and fraudulent transactions.

### Fraud Rate by Amount Band

Shows which transaction-value ranges have higher observed fraud rates.

### Correlation Matrix

Displays relationships between anonymized transaction features, transaction amount, and fraud classification.



## 💡 Business Insights

The analysis can help financial institutions:

* Identify high-risk transaction periods.
* Monitor unusual transaction amounts.
* Compare fraudulent and legitimate transaction behavior.
* Prioritize suspicious transactions for investigation.
* Improve fraud-monitoring rules.
* Identify variables that may be useful for future fraud-detection models.



## 📂 Project Structure

```text
credit-card-transaction-fraud-analysis/
│
├── README.md
├── credit_card_analytics.py
├── creditcard.csv
├── requirements.txt
│
├── outputs/
│   ├── amount_by_transaction_type.csv
│   ├── hourly_transaction_analysis.csv
│   ├── amount_band_analysis.csv
│   ├── top_20_transactions.csv
│   └── top_20_fraud_transactions.csv

## 🚀 How to Run the Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/Ameesha3/credit-card-transaction-fraud-analysis.git
```

### Step 2: Open the Project

```bash
cd credit-card-transaction-fraud-analysis
```

### Step 3: Install Required Libraries

```bash
pip install -r requirements.txt
```

### Step 4: Run the Python Script

```bash
python credit_card_analytics.py
```



## 📊 Sample KPIs

The project calculates:

```text
Total Transactions
Total Transaction Value
Average Transaction Amount
Fraud Transactions
Fraud Rate
Fraud Transaction Value
Fraud Amount Share
```

These KPIs provide a high-level view of transaction activity and fraud exposure.



## 🔮 Future Improvements

The project can be further enhanced by adding:

* SQL-based transaction analysis
* Power BI fraud-monitoring dashboard
* Customer-level analysis when customer information is available
* Machine Learning fraud classification
* Anomaly detection
* Precision, Recall and F1-score evaluation
* Real-time fraud-monitoring concepts
* Advanced statistical analysis



## 👩‍💻 Skills Demonstrated

### Data Analysis

* Exploratory Data Analysis
* Data Cleaning
* Feature Engineering
* KPI Development
* Fraud Analysis
* Time-Based Analysis
* Correlation Analysis

### Python

* Pandas
* NumPy
* Matplotlib
* Seaborn

### Business Analytics

* Business Question Formulation
* Pattern Identification
* Risk Analysis
* Insight Generation
* Data Storytelling



## ⭐ Resume Description

**Credit Card Transaction & Fraud Analytics | Python**

* Analyzed **284K+ credit card transactions** using Pandas and NumPy to evaluate transaction value, fraud rate, and transaction-risk patterns.
* Engineered time and transaction-value features to identify **hourly and amount-band patterns associated with fraudulent activity**.
* Developed **Matplotlib and Seaborn visualizations** to compare legitimate and fraudulent transaction behavior.
* Performed correlation analysis on **28 anonymized transaction features** to identify variables associated with fraud.



## 📄 Disclaimer

This project is created for educational and portfolio purposes.

The dataset contains anonymized transaction features. The `V1`–`V28` variables should not be interpreted as customer demographics, merchant information, or other real-world attributes.

No customer, merchant, card-type, or demographic information has been fabricated for this analysis.
