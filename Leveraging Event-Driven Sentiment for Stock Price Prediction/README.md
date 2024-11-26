# Leveraging Event-Driven Sentiment for Stock Price Prediction

## Overview
This project explores the relationship between **event-driven sentiment** and **stock price prediction**, focusing on high-impact corporate events like **Apple’s iPhone 16 launch** and **Tesla’s Battery Day 2020**. By integrating **FinBERT**, a sentiment analysis model for financial text, with historical stock data, this approach demonstrates how sentiment can significantly enhance the accuracy of stock price prediction.

## Features
- **Sentiment Analysis :** Uses **FinBERT** to extract daily sentiment scores (positive, neutral, negative) from Twitter data.
- **Stock Price Prediction :** Combines sentiment scores with historical stock features (e.g., Open, Close, Volume) for prediction using a linear regression model.
- **Event Impact Assessment :** Evaluates the influence of market sentiment on stock price movements during specific corporate events.
- **Cross-Validation :** Utilizes time-series cross-validation to ensure robust model performance.

## Use Cases
- **Investor Insights :** Provides actionable insights for traders and investors by correlating public sentiment with stock performance.
- **Event Analysis :** Helps assess the market impact of major corporate events.
- **Financial Forecasting :** Enhances predictive capabilities for automated trading systems and financial analysts.

## Technologies Used
- **Python :** Core programming language.
- **FinBERT :** Financial text-specific sentiment analysis model from Hugging Face.
- **Pandas :** For data manipulation and analysis.
- **Matplotlib** and **Seaborn :** For data visualization.
- **Scikit-learn :** For implementing the linear regression model and evaluating performance.

