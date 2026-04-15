#  Trader Performance vs Market Sentiment Analysis

##  Objective
This project analyzes how market sentiment (Fear/Greed index) impacts trader behavior and performance on Hyperliquid. The goal is to identify actionable patterns that can improve trading strategies.

---

##  Methodology

### Data Preparation
- Loaded Bitcoin Fear/Greed dataset and Hyperliquid trader dataset
- Cleaned missing values and removed duplicates
- Converted timestamps into datetime format
- Aligned both datasets at a daily level
- Merged datasets using the `date` column

### Feature Engineering
Created key metrics:
- Daily Profit & Loss (PnL)
- Win rate (profitable trades %)
- Trade size (USD)
- Trade frequency
- Buy/Sell distribution

### Segmentation
- Winners vs Losers
- Frequent vs Infrequent traders
- Large vs Small trade sizes

---

## Key Insights

### 1. Profitability peaks during Extreme Greed
Average PnL is highest during Extreme Greed periods, indicating strong bullish sentiment creates profitable opportunities.

### 2. Fear periods outperform normal Greed
Fear conditions show higher PnL than normal Greed, suggesting traders benefit from volatility and market corrections.

### 3. Market extremes are more profitable
Both Extreme Fear and Extreme Greed outperform Neutral conditions, showing that high volatility leads to better trading outcomes.

### 4. Trader behavior changes with sentiment
- Trade sizes increase during Greed periods (higher risk-taking)
- Trading activity varies across sentiment regimes
- Buy/Sell patterns shift depending on sentiment

### 5. Experienced traders perform better
Frequent and consistently profitable traders outperform others across all sentiment conditions.

---

## Strategy Recommendations

- Increase exposure during Extreme Greed to capitalize on bullish trends
- Use Fear periods for selective opportunities like dip-buying
- Avoid aggressive trading during Neutral markets due to low profitability
- Focus on consistency and disciplined trading behavior

---

##  How to Run

1. Clone the repository:
```bash
git clone https://github.com/your-username/trader-sentiment-analysis.git
