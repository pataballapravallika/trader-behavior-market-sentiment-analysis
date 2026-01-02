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
## 📸 Key Outputs & Visualizations
This section highlights the primary outputs generated from the analysis to support the observed insights.

## 1️⃣ Market Sentiment Integration

Verified successful integration of trader data with daily Bitcoin market sentiment.
Each trade was correctly tagged with the corresponding Fear or Greed classification.

Output:
<img width="463" height="228" alt="image" src="https://github.com/user-attachments/assets/6624ed77-ba6d-4835-817e-ef0f973478e2" />

Frequency count of trades by sentiment category.

## 2️⃣ Average Profitability by Sentiment

Compared mean closed PnL across Fear and Greed periods.
Demonstrates how overall trader profitability varies with market sentiment.

Output:
<img width="612" height="207" alt="image" src="https://github.com/user-attachments/assets/18bedb52-71f2-435c-b901-9809ad858b62" />

Aggregated average PnL values by sentiment.

## 3️⃣ Win Rate Analysis

Calculated the proportion of profitable trades under each sentiment category.

Provides an intuitive performance metric beyond raw PnL.

Output:
<img width="600" height="216" alt="image" src="https://github.com/user-attachments/assets/3b364837-9010-471e-8906-ddfd74481a95" />


Win rate (percentage of profitable trades) for Fear vs Greed.

4️⃣ PnL Distribution Visualization

Visualized the distribution of closed PnL values across sentiment regimes.

Highlights variance and risk associated with different market conditions.

Output:
<img width="981" height="724" alt="image" src="https://github.com/user-attachments/assets/905eeaec-64f1-4c45-add7-9ed6596e792b" />


Box plot showing PnL distribution by sentiment.

5️⃣ Risk Exposure via Trade Size

Analyzed average trade size (USD) as a proxy for risk appetite.

Identifies increased risk-taking behavior during Greed periods.

Output:
<img width="1048" height="713" alt="image" src="https://github.com/user-attachments/assets/464d0fea-4743-47f9-b9c8-6bc461cac8d6" />


Bar chart comparing average trade size by sentiment.

📌 Note

Screenshots of the above outputs are available in the analysis notebook and can be shared upon request.
The GitHub repository focuses on reproducible analysis rather than static images.
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
