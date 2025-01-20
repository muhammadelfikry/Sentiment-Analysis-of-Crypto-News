# Crypto Market Sentiment Analysis and Price Movement Correlation

## Backgorund
This project aims to analyze the sentiment of cryptocurrency-related news articles, especially bitcoin, and correlate it with market price movements. Utilizing natural language processing (NLP) techniques and financial data analysis, the project seeks to determine how market sentiment affects cryptocurrency prices.

## Objectives
- Perform sentiment analysis using machine learning.
- Collect bitcoin prices from CoinGecko.
- Correlate sentiment with cryptocurrency price movements.

## Exploratory Data Analysis
1. what happened?
   
   ![image](https://github.com/user-attachments/assets/7ad4997e-22b2-4918-a623-ce100f772645)

   Based on the data collected from the news and the model training results, the majority of the public shows a positive sentiment towards Bitcoin.

2. What words are frequently used in public sentiment towards bitcoin?

   ![image](https://github.com/user-attachments/assets/9df82eee-4691-4dd5-b02d-f026cee3108d)
   ![image](https://github.com/user-attachments/assets/b6a3f131-cf68-43bd-915f-244c509591f0)
   ![image](https://github.com/user-attachments/assets/d764e69b-dcdc-408e-950b-ef3931cd84e9)
   ![image](https://github.com/user-attachments/assets/0d008d3b-3fbe-4b90-89f2-1186b33897e7)

   Most of the many news stories use words like btc, bitcoin, etf, investor, increase, price, market, report.

3. how sentiment correlates with bitcoin price?

   ![image](https://github.com/user-attachments/assets/be3368f5-28cc-432b-837c-36a83ad4a5a1)
   ![image](https://github.com/user-attachments/assets/7f8249d4-f685-4d6e-92cd-df0e97694a6c)

   Based on the news dataset used for model training and its correlation with bitcoin price movements, no correlation was found from market sentiment to bitcoin price movements. This is also influenced by the limited dataset used for model training in conducting sentiment analysis.

## Methodology
1. Data Collection:
   - Using the news dataset obtained from Kaggle. [Dataset](https://www.kaggle.com/datasets/imadallal/sentiment-analysis-of-bitcoin-news)
   - Collect historical price data for the same period using the CoinGecko API.
2. Preprocessing
   - Clean and tokenize news text.
   - Remove stop words, perform lemmatization, and extract key features using TF-IDF.
3. Sentiment Analysis
   - Perform text labeling using TextBlob.
   - Determining sentiment for news articles using Naive Bayes, Logistic Regression, Random Forest, and Multilayer Perceptron algorithms.
4. Correlation Analysis:
   - Aggregate sentiment data with daily price trends.
   - Perform correlation calculation and visualization. 

## Conclusion
Random Forest is the best machine learning model to predict sentiment with 99.4% accuracy on training data and 77.5% on test data.
