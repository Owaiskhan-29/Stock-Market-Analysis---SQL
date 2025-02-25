# Stock Market Analysis using SQL

## Project Overview
This project focuses on analyzing stock market data from the National Stock Exchange (NSE) using SQL. It leverages Moving Average (MA) techniques to generate Buy, Sell, and Hold signals based on historical stock prices. The dataset consists of stock prices from January 2015 to July 2018 for six companies: Eicher Motors, Hero, Bajaj Auto, TVS Motors, Infosys, and TCS.

## Problem Statement
Stock market trading relies on technical and fundamental analysis. One widely used technique is the Moving Average Method, which helps smooth price trends and determine potential buy and sell opportunities. This project utilizes 20-day and 50-day moving averages to identify trend shifts:
- **Golden Cross**: A buy signal occurs when the short-term MA (20-day) crosses above the long-term MA (50-day).
- **Death Cross**: A sell signal occurs when the short-term MA crosses below the long-term MA.

## Data Set
The dataset is extracted from NSE and contains daily stock prices. Missing values for moving averages are ignored instead of being filled with averages, as that would distort the analysis.

## Implementation Steps
1. **Data Import**: Create a MySQL schema named `Assignment` and import CSV files as tables corresponding to each stock.
2. **Calculate Moving Averages**: Compute 20-day and 50-day MAs for each stock and store them in a new table.
3. **Master Table Creation**: Merge stock data into a single table with columns for date and stock prices.
4. **Buy/Sell/Hold Signals**: Generate trading signals based on moving average crossovers and store them in separate tables.
5. **User-Defined Function**: Implement a function to retrieve the trading signal for a given date.
6. **Analysis & Inferences**: Summarize key insights based on trends identified in the dataset.

## Technologies Used
- **SQL** (MySQL) for data storage and querying
- **Pandas & Python** (optional for additional data preprocessing and visualization)
- **Excel/CSV** for data import and export

## Results & Insights
- Moving average crossovers effectively signal trading opportunities.
- Stocks exhibit varying trends based on market conditions, requiring further analysis for optimal decision-making.
- The approach can be extended to include additional technical indicators for better predictions.
