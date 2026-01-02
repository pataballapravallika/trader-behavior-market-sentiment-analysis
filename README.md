# Trader Behavior vs Market Sentiment Analysis

## 📌 Project Overview
This project analyzes the relationship between **Bitcoin market sentiment (Fear vs Greed)** and **trader behavior/performance** using historical trading data.  
The goal is to uncover patterns in profitability, risk-taking, and trading activity under different market sentiment conditions.

---

## 🎯 Objective
- Understand how market sentiment influences trader performance
- Compare trading behavior during **Fear** and **Greed** phases
- Extract actionable insights that can inform smarter trading strategies

---

## 📂 Datasets Used
1. **Historical Trader Data (Hyperliquid)**
   - Contains individual trade-level information such as execution price, trade size, side (buy/sell), timestamps, and closed PnL.

2. **Bitcoin Fear & Greed Index**
   - Daily market sentiment classification indicating whether the market is in a Fear or Greed state.

> ⚠️ Note:  
> The datasets were provided as part of the hiring assignment and are **not included in this repository** due to size and usage considerations.

---

## 🛠️ Tools & Technologies
- Python  
- Pandas & NumPy (data manipulation)  
- Matplotlib & Seaborn (visualization)  
- Jupyter Notebook  

---

## 🔍 Methodology

### Step 1: Data Loading & Understanding
- Loaded both datasets and inspected structure, data types, and missing values.
- Identified appropriate timestamp columns for alignment.

### Step 2: Data Cleaning & Preparation
- Converted trade timestamps to date format.
- Standardized date fields across both datasets.
- Removed rows with missing sentiment classification.

### Step 3: Data Integration
- Merged trade-level data with daily market sentiment using the date column.
- Ensured correct alignment between trades and corresponding sentiment.

### Step 4: Feature Engineering
- Created a profitability indicator (`is_profit`) based on closed PnL.
- Used trade size (USD) as a proxy for risk exposure.

### Step 5: Exploratory Data Analysis
- Compared average PnL across Fear and Greed periods.
- Analyzed win rates (percentage of profitable trades).
- Examined trade size behavior under different sentiment conditions.
- Visualized distributions using box plots and bar charts.

---

## 📊 Key Insights
- Traders tend to take **larger positions during Greed periods**, indicating higher risk appetite.
- **Win rates and average profitability are generally higher during Greed**, but outcome variability is also greater.
- **Fear periods show more conservative trading behavior**, with smaller trade sizes and reduced profitability.
- Market sentiment plays a significant role in influencing trader decision-making and risk exposure.

---

## 📁 Repository Structure
1. path
   ```bash
   trader-behavior-market-sentiment-analysis/
   ├── analysis.ipynb # Main analysis notebook
   ├── README.md # Project documentation
   ├── requirements.txt # Python dependencies
   └── .gitignore # Ignored files (datasets, caches)
  
---

## 🚀 How to Run the Project
1. Clone the repository
   ```bash
   git clone <repository-url>


---

2. Install dependencies
   ```bash
   pip install -r requirements.txt


---

3. Open and run the notebook
   ```bash
   jupyter notebook analysis.ipynb


---

## Conclusion
This analysis demonstrates how combining market sentiment indicators with trade-level data can reveal meaningful patterns in trader behavior.
Such insights can be leveraged to design sentiment-aware trading strategies and improve risk management decisions.

## Author
Pataballa Pravallika
