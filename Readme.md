
![launching-moon-bitcoin-rocket-start_886350-528](https://github.com/user-attachments/assets/eaf10ab6-2a69-481c-858a-a6d5fbe6ea72)

# Bitcoin Price Prediction

## Author: Jessie Freelander

### Problem Statement
The goal of this project is to predict Bitcoin price movements based on sentiment analysis, volume of tweets, and previous bitcoin price action movements. By understanding the correlation between social media sentiment and Bitcoin price fluctuations, we aim to develop a predictive model that can predict the accuracy of a 24 hour price increase or decrease.

## Data Overview
- **Source**: Twitter (X) posts and CoinGecko API for Bitcoin price data.
- **Timeframe**: December 2023 to March 2024.
- **Features**:
  - **Sentiment Analysis**: VADER sentiment scores with custom weights, resulting in an aggregate score as the **Predicted SID**.
  - **Target Variable**: Bitcoin price movement.
- **Limitations**:
  - 60,000 crypto related tweets were collected
  - Limited timeframe of data collection.
  - Focused exclusively on Bitcoin instead of a broader range of cryptocurrencies.


## Methods
### Sentiment Analysis
- **VADER Sentiment Analysis**: Applied with custom weights to calculate an aggregate sentiment score.

- **Preprocessing**: Cleaning of raw text data to extract meaningful sentiment.

### Sentiment and Price Analysis Graph 
![Screenshot 2024-11-15 at 9 52 51 AM](https://github.com/user-attachments/assets/837202e1-9007-4409-8ece-69def16dfc71)

- **Graph**: 
This graph illustrates the relationship between Bitcoin's price and average sentiment (red line) over time from December 2023 to February 2024. Bitcoin's price shows an overall upward trend with significant fluctuations, while sentiment varies sharply, possibly reflecting market reactions to news or events. Although not perfectly correlated, there are instances where a rise in sentiment is followed by an increase in Bitcoin's price, hinting that sentiment could have an influence on price movements.

### Machine Learning Models
- Built and evaluated multiple models to predict price action.
![Screenshot 2024-11-15 at 9 56 57 AM](https://github.com/user-attachments/assets/27290fbe-7af1-4b7c-b43f-b555cd25c6c7)

- Performance Metrics:
  - **Accuracy**: 0.65
  - **Precision**: 0.64
  - **F1-Score**: 0.75


## Key Findings
1. Sentiment analysis shows potential in explaining Bitcoin price movements, but results are inconsistent.
2. Model performance suggests room for improvement by:
   - Refining the dataset (e.g., focusing on smaller, more volatile cryptocurrencies).
   - Incorporating additional features like trading volume and on-chain metrics.
3. Features related to sentiment had moderate importance, indicating other external factors may have significant influence.

## Recommendations
- Collect more consistent and diverse data for Tweets, Bitcoin, and altcoins.
- Focus on smaller, more volatile cryptocurrencies to test sentiment's predictive power.
- Explore additional features such as news coverage, on-chain analytics, and trading patterns.


## Directory
Data: [Combined Data Frame]([https://pypi.org/project/pybaseball/2.0.0/](https://github.com/Anicca18/Phase-4-Project/tree/main/Data))
Presentation: [Presentation.pdf]([https://github.com/user-attachments/files/17546271/Presentation.pdf](https://github.com/Anicca18/Phase-4-Project/blob/main/Presentation.pdf))
