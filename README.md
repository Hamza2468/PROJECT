# PROJECT

## Overview
This project comprises a comprehensive pipeline for analyzing financial news and predicting stock prices. The implementation is divided into five tasks, each addressing a specific aspect of data analysis, modeling, and prediction.

---

### Task 1: Exploratory Data Analysis (EDA)
- **Objective**: Analyze the provided dataset for insights into article volume trends, word frequency, and other descriptive statistics.
- **Key Features**:
  - Load and preprocess the dataset (handle missing values).
  - Generate time-series analysis for article trends.
  - Create word clouds for headlines and descriptions.
- **Output**: Visualizations of article volume trends and word clouds.

---

### Task 2: Stock Ticker Extraction
- **Objective**: Extract stock tickers from financial news articles.
- **Key Features**:
  - Use regex to identify stock tickers in article headlines.
  - Apply fuzzy matching for ambiguous company names.
  - Save extracted tickers to a CSV file.
- **Output**: A CSV file containing articles and their associated stock tickers.

---

### Task 3: Financial Data Retrieval
- **Objective**: Retrieve stock price data and financial metrics for extracted tickers.
- **Key Features**:
  - Fetch historical stock prices using the Yahoo Finance API.
  - Extract financial metrics such as market cap, P/E ratio, and dividend yield.
  - Handle API errors and missing data gracefully.
- **Output**: Individual CSV files for historical stock prices and a consolidated CSV for financial metrics.

---

### Task 4: Stock Price Forecasting
- **Objective**: Predict future stock prices using machine learning models.
- **Key Features**:
  - Build and train an LSTM model on historical stock price data.
  - Predict stock prices for the next 7, 15, and 30 days.
  - Evaluate model performance using metrics such as Mean Squared Error (MSE) and Mean Absolute Error (MAE).
  - Visualize historical data alongside future predictions.
- **Output**: Predictions for 7, 15, and 30 days, along with evaluation metrics and visualizations.

---

### Task 5: Sentiment Analysis and Impact on Stock Prices
- **Objective**: Analyze the sentiment of financial news and its impact on stock price changes.
- **Key Features**:
  - Perform sentiment analysis on news headlines and descriptions using TextBlob.
  - Merge sentiment scores with historical stock prices to study correlations.
  - Build a linear regression model to predict stock price changes based on sentiment scores.
  - Evaluate the model using MSE and MAE metrics.
  - Visualize sentiment scores, stock prices, and predictions.
- **Output**: Insights into the relationship between sentiment and stock prices, with visualizations and model evaluation metrics.

---

## How to Use
1. **Prerequisites**:
   - Python 3.8+
   - Required libraries: `pandas`, `numpy`, `matplotlib`, `wordcloud`, `textblob`, `yfinance`, `tensorflow`, `scikit-learn`

2. **Run Each Task**:
   - Task 1: Analyze the dataset and generate visualizations.
   - Task 2: Extract stock tickers from news articles and save to a CSV file.
   - Task 3: Fetch stock prices and financial metrics for tickers.
   - Task 4: Train an LSTM model and predict future stock prices.
   - Task 5: Perform sentiment analysis and evaluate its impact on stock prices.

3. **Data Sources**:
   - Financial news dataset: `/content/reuters_headlines.csv`
   - Historical stock price data: Retrieved dynamically using Yahoo Finance API.

4. **Outputs**:
   - CSV files for processed data and predictions.
   - Visualizations for trends, forecasts, and sentiment analysis.

---

## Project Structure
- **`Task 1: EDA`**: Descriptive analysis and visualizations.
- **`Task 2: Ticker Extraction`**: Identifies stock tickers from news articles.
- **`Task 3: Data Retrieval`**: Fetches stock prices and financial metrics.
- **`Task 4: Forecasting`**: LSTM-based future stock price predictions.
- **`Task 5: Sentiment Analysis`**: Studies the relationship between news sentiment and stock prices.

---

## Disclaimer
- The tools and code provided in this project are for research and educational purposes only.
- No warranty is provided regarding the accuracy or reliability of the predictions.

---

## Citation
```bibtex
@misc{financialnews2025,
  title={Financial News and Stock Price Prediction},
  author={Your Name},
  year={2025}
}
