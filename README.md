# Google-Stock-Price-Analysis
A stock price analysis system for Google (GOOGL) using historical data from 2020 to 2022, retrieved via the yfinance library. The project downloads and preprocesses stock data (Adjusted Close, Open, Close, High, Low) and sets the foundation for predictive modeling using machine learning techniques like LSTM.
# Google Stock Price Analysis
## Overview
This project analyzes Google's (GOOGL) historical stock prices from January 1, 2020, to December 29, 2022, using the yfinance library to retrieve data. The dataset includes 755 daily records with features like Adjusted Close, Open, Close, High, and Low prices, rounded to three decimal places. The project preprocesses the data using MinMaxScaler and sets the foundation for time-series forecasting with machine learning models like LSTM. It leverages Python libraries including yfinance, TensorFlow, Pandas, NumPy, Matplotlib, and Scikit-learn for data manipulation, visualization, and predictive modeling.

## Features
- Data Retrieval: Downloads Google's historical stock data (2020–2022) using yfinance.
- Data Preprocessing: Extracts key features (Adjusted Close, Open, Close, High, Low) and normalizes data using MinMaxScaler.
- Data Inspection: Displays the dataset with 755 rows and 5 columns for initial analysis.
- Visualization: Supports plotting stock price trends using Matplotlib (extendable for further insights).
- Extensibility: Designed to support time-series forecasting with LSTM or other machine learning models.

## Dataset
The dataset is sourced from Yahoo Finance via the yfinance library:
- Ticker: GOOGL (Google/Alphabet Inc.).
- Time Period: January 1, 2020, to December 29, 2022.
- Total Records: 755 daily entries.
- Features: Adjusted Close, Open, Close, High, Low (all rounded to 3 decimal places).
- Sample Data:
  - First record (2020-01-02): Adj Close: 68.356, Open: 67.421, Close: 68.434, High: 68.434, Low: 67.325.
  - Last record (2022-12-29): Adj Close: 88.349, Open: 86.620, Close: 88.450, High: 88.850, Low: 86.610.

## Requirements
- Python 3.10
- Libraries: `yfinance`, `tensorflow`, `pandas`, `numpy`, `matplotlib`, `scikit-learn`

## Usage
- Download Google's stock data using yfinance for the specified period (2020–2022).
- Preprocess the data by selecting relevant features and applying normalization with MinMaxScaler.
- Inspect the dataset to verify structure and contents (755 rows, 5 columns).
- Visualize stock price trends using Matplotlib for exploratory analysis.
- (Optional) Extend the project by implementing LSTM models for stock price prediction and evaluating performance with metrics like RMSE.

## Example
The project retrieves and preprocesses Google's stock data:
- Dataset Size: 755 daily records.
- Features: Adjusted Close, Open, Close, High, Low.
- Sample Visualization: Plot Adjusted Close prices over time to identify trends.
- Future Steps: Train an LSTM model on normalized data to predict future stock prices.

## Methodology
- Data Retrieval: Uses yfinance to download historical stock data for GOOGL.
- Preprocessing: Selects five key features and applies MinMaxScaler for normalization, suitable for machine learning.
- Inspection: Outputs the dataset as a Pandas DataFrame for initial analysis.
- Visualization: Employs Matplotlib to plot stock price trends (e.g., Adjusted Close over time).
- Future Modeling: The project is structured to support LSTM-based time-series forecasting, with potential evaluation using RMSE or MAE.

## Future Improvements
- Implement LSTM models for stock price prediction using TensorFlow.
- Add technical indicators (e.g., Moving Averages, RSI) to enhance feature engineering.
- Evaluate model performance with metrics like RMSE, MAE, and R².
- Incorporate data augmentation or sliding window techniques for time-series analysis.
- Enhance visualizations with interactive plots using Plotly or additional metrics like volatility.
