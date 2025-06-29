
🧠 Trader Behavior vs. Market Sentiment Analysis

 Problem Statement

The objective of this project is to explore the relationship between **Bitcoin market sentiment** (Fear/Greed) and **trader performance** using two datasets:

- A Bitcoin Market Sentiment dataset containing daily sentiment classification.
- Historical Trader Data capturing trade-level performance and strategy data.

By merging these datasets and performing exploratory analysis, we aim to uncover behavioral patterns and generate actionable insights that can inform smarter trading strategies in the crypto market.

---

 Datasets

1. Bitcoin Market Sentiment Dataset**
- Columns:Date`, `Classification`
- Description: Daily classification of the Bitcoin market as either `Fear` or `Greed`.

2. Historical Trader Data 
- Columns: `account`, `symbol`, `execution price`, `size`, `side`, `time`, `start position`, `event`, `closedPnL`, `leverage`, etc.
- Description:Individual-level trader transactions with detailed metrics.

---

## 🧪 Methodology

1. Data Cleaning & Preprocessing
   - Converted time fields to datetime format.
   - Normalized classification labels and merged datasets on date.
   - Removed or handled missing/invalid values.

2. Data Merging
   - Merged sentiment data with trader data using the `date` field to associate each trade with the prevailing sentiment.

3. Exploratory Data Analysis
   - Conducted statistical and visual analysis of trader behavior under different sentiment conditions using Python libraries (`pandas`, `seaborn`, `matplotlib`, `scipy`).

---

 Key Insights

1. Profitability Trends  
Traders tend to perform significantly better during **Greed** sentiment days, with both **higher average profits** and **higher win rates**. However, volatility in outcomes also increases, suggesting greater risk-taking.

2. Leverage Usage  
Leverage is **more aggressively used** during Greed periods, while traders **scale back** during Fear. Top-performing traders use **lower leverage** on Fear days, suggesting more disciplined risk management.

3. Trading Volume  
Traders show higher activity (measured by volume and position size) during Greed, reflecting increased market confidence.

4. Symbol-Specific Behavior  
Mainstream cryptocurrencies like BTC and ETH perform better on Greed days, while some smaller coins remain active during Fear days due to speculative behavior.

5. Top Traders vs. Others  
Top traders (ranked by cumulative profit) demonstrate more conservative behavior, especially during fearful sentiment days. They manage risk better and achieve more consistent outcomes.

---

 Conclusion

> **Sentiment is a strong behavioral signal.** Understanding how trader behavior aligns or diverges under Fear and Greed can help develop **risk-aware strategies**, allocate **capital more intelligently**, and **identify market inefficiencies**.  
>
> This analysis demonstrates that integrating sentiment data into trading systems can significantly enhance decision-making and performance tracking in volatile crypto markets.

---

Tech Stack

- **Languages:** Python (Pandas, NumPy)
- **Visualization:** Matplotlib, Seaborn
- **Statistical Testing:** Scipy
- **Optional Dashboard:** Tableau / Streamlit

---

