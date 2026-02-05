Trader Performance vs Market Sentiment

 Overview
This project analyzes how Bitcoin market sentiment (Fear, Greed, Neutral)
influences trader behavior and profitability on the Hyperliquid platform.

The analysis combines:
- Market sentiment data
- Trader behavioral metrics
- Machine learning models for prediction

The goal is to derive **actionable, sentiment-aware trading insights**.

 Dataset
- **Bitcoin Fear & Greed Index**
- **Hyperliquid Trader Historical Data**

Project Workflow

1. Data loading & cleaning
2. Timestamp alignment and daily aggregation
3. Feature engineering (PnL, win rate, activity)
4. Trader segmentation
5. Sentiment-based analysis
6. Predictive modeling (bonus)

 Models Used

- Logistic Regression (baseline)
- **Random Forest Classifier (final model)**

The Random Forest model captures non-linear interactions between sentiment
and trader behavior.

 Model Performance

**Random Forest Accuracy: ~95%**

- Balanced precision and recall
- Strong performance for both profitable and non-profitable days
- No price indicators used — only sentiment and behavior

 Key Insights

- Traders earn higher profits during Fear due to increased activity
- Greed days show higher accuracy but lower overall profit
- High-activity traders are more sentiment-sensitive
- Market sentiment impacts behavior more than prediction accuracy

 Setup Instructions


