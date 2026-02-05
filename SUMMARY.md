 Methodology

This project analyzes the relationship between **Bitcoin market sentiment** and **trader behavior and performance** on the Hyperliquid platform.

Two datasets were used: a daily Bitcoin Fear & Greed Index and detailed trader-level transaction data. After loading and validating both datasets, timestamps were converted to a common datetime format and aligned at a **daily level**. Sentiment labels were standardized to ensure consistency.

Trader transaction records were aggregated per **account per day** to create key behavioral and performance metrics, including:

* Daily profit and loss (PnL)
* Number of trades per day
* Average trade size
* Win rate

The aggregated trader data was then merged with daily market sentiment. Traders were segmented into **high activity** and **low activity** groups based on average daily trade frequency. Analysis was performed to compare performance and behavior across sentiment regimes.

As a bonus, a **lightweight predictive model** was built to classify whether a trader would have a profitable day using sentiment and behavioral features. Logistic Regression was used as a baseline, followed by a Random Forest model to capture non-linear patterns.

Key Insights

1. **Trader profitability is highest during Fear sentiment**
   Fear days showed the highest average daily PnL, driven by increased trade frequency and larger average trade sizes. This suggests that heightened volatility creates more profit opportunities, despite increased risk.

2. **Greed sentiment improves accuracy, not total profit**
   Greed days exhibited slightly higher win rates but lower overall profitability due to reduced trading activity and smaller position sizes. Traders appear more selective during optimistic market conditions.

3. **High-activity traders are more sentiment-sensitive**
   High-activity traders significantly increase participation during Fear and reduce activity during Greed, while low-activity traders maintain relatively stable behavior across sentiment regimes.

4. **Market sentiment influences behavior more than precision**
   Profitability is driven more by changes in trading behavior (frequency and size) than by win rate alone, highlighting the importance of sentiment-aware risk management.

 Strategy Recommendations

1. **Fear Market Strategy**
   Allow increased trade frequency during Fear conditions, but enforce stricter controls on leverage or position size to manage heightened risk.

2. **Greed Market Strategy**
   Prioritize high-confidence, selective trades during Greed periods. Avoid over-trading, as accuracy improves but overall opportunity decreases.

3. **Neutral Market Strategy**
   Use balanced, consistency-focused strategies during Neutral sentiment, as these periods show fewer strong trading signals and lower profitability.

Predictive Modeling Outcome (Bonus)

The Random Forest model achieved approximately **95% accuracy** in predicting daily trader profitability using only sentiment and behavioral features. This validates the strong predictive signal present in trader behavior combined with market sentiment, even without price-based indicators.

 Final Note

The focus of this project is **interpretability and actionable insight**, not complex modeling. Results demonstrate that sentiment-aware behavioral analysis can meaningfully inform trading strategy design.
