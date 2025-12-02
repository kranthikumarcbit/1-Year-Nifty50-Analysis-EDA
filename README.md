# 1-Year-Nifty50-Analysis-EDA
observation of Market Trends, Volatility, Traders Behaviour, Seasonality Insights over 1 year of Nifty50 data


🧭 Project Objective

To analyze one year of Nifty 50 stock market data using Python and discover meaningful insights on price movement, volatility, trend behavior, and investor sentiment — all through data visualization and statistical analysis.


---

⚙ Dataset Overview

Contains daily records for ~1 year.

Columns: Date, Open, High, Low, Close, Volume, Daily Return, etc.

The analysis focuses on price trends, volatility, returns, and correlations.

<img width="629" height="345" alt="Overall_trends" src="https://github.com/user-attachments/assets/7842ef9d-badf-4f36-95b4-5008fa951f06" />


---

📈 Major Components of the Analysis

1️⃣ Market Trend Analysis

Close price trend showed clear uptrends and downtrends across the year.

Downturns: March & May → driven by fiscal year-end selling, “Sell in May” sentiment.

Recovery: From June–October → stable earnings & festive optimism.

Rolling means (20-day & 50-day) captured trend reversals via Golden Cross (bullish) and Death Cross (bearish) points.


<img width="629" height="332" alt="Short_term vs Mid term " src="https://github.com/user-attachments/assets/a4daed49-d1cb-4fce-b1c4-5e46118c59d9" />

---

2️⃣ Average Monthly Returns

Bar chart of monthly average returns revealed alternating bullish and bearish phases.

Positive months: January, July, October, November — investor optimism and festive demand.

Negative months: March & May — fiscal rebalancing, global risk-off behavior.

Months were unordered (alphabetically), but the pattern shows clear cyclical sentiment.


<img width="532" height="386" alt="Monthly_trends" src="https://github.com/user-attachments/assets/39b2cd52-13cf-48f9-8cb0-14267b8a3a32" />

---

3️⃣ Weekday Effect

Mondays → often negative (weekend news & cautious starts).

Wednesdays & Fridays → relatively positive (institutional trades, short covering).

Thursdays → highly volatile due to weekly F&O expiry.

Confirms behavioral finance pattern — traders’ psychology shapes intraday rhythm.
<img width="438" height="318" alt="weekly_trends" src="https://github.com/user-attachments/assets/5ea5e8c5-affc-4ccb-987d-2bf178ca8ce9" />



---

4️⃣ Volatility Pattern

Daily volatility spiked in March, May, and September due to rebalancing and global triggers.

Lower volatility phases in July–October suggested investor confidence.

High volatility = uncertainty; low volatility = stable trends.

<img width="629" height="291" alt="daily_volitility" src="https://github.com/user-attachments/assets/6037e402-1f5f-4ad4-a3d1-7f4b0c4ed437" />


---

5️⃣ Distribution of Daily Returns

Near-normal but slightly negatively skewed distribution.

Most returns cluster around zero (small day-to-day moves).

Fat tails (kurtosis > 3) — extreme events occur more often than random models predict.

Implies market reacts faster to fear than to optimism.
<img width="392" height="288" alt="Daily return distrubutions" src="https://github.com/user-attachments/assets/1dda1ae7-121f-40ef-88b9-5d52e4ce24bb" />



---

6️⃣ Correlation Heatmap

Open, High, Low, Close are almost perfectly correlated (>0.95).

Volume has weak correlation (~0.2–0.4) with price — high trading doesn’t guarantee high returns.

Suggests market movement is trend-driven, not volume-driven.
<img width="407" height="341" alt="correlation" src="https://github.com/user-attachments/assets/544f9358-913b-4880-850e-a24571aec458" />



---

7️⃣ Scatter Plot (Volume vs Daily Return)

Random scatter — no linear relationship between trading volume and daily return.

High volume = volatility, not necessarily profit.

Price direction depends on sentiment, not just trade count.



---

8️⃣ Biggest Gain & Drop Days

Identified using idxmax() and idxmin() on daily returns.

Example:

Biggest Gain: May 12, 2025

Biggest Drop: Likely due to macro or earnings shock


Helps identify event-driven volatility days for deeper cause analysis.

<img width="350" height="298" alt="overall_trends candle data" src="https://github.com/user-attachments/assets/1f51f99e-5bf9-4cf8-9878-52a65b9016de" />


---

🧩 Overall Storyline

> The Nifty 50 over this one-year period displayed classic cyclical behavior — early optimism, mid-year corrections, and festive recovery.
Trends were strong and identifiable via moving averages, but short-term returns were highly volatile.
Volume didn’t explain returns — confirming that sentiment and macroeconomic timing are the true market drivers.
The market’s bias toward sharper declines than rises reflects the Indian market’s reaction to global uncertainty and domestic fiscal cycles.
