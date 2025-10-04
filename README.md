# AI Financial Data Analysis and Stock Impact Forecasting

## Overview
This project analyzes synthetic daily financial data for AI companies (OpenAI, Google, Meta) from 2015 onwards. The goal is to explore trends in R&D spending, AI revenue, and events, then forecast stock impact percentage using time-series models like ARIMA.

Key features:
- Data cleaning and exploration (EDA) with visualizations.
- Time-series forecasting for stock impact.
- Insights into how AI investments affect financial performance.

The data is synthetic (from "ai_financial_market_daily_realistic_synthetic.csv") and covers metrics like R&D spending, AI revenue growth, events, and stock impact.

## Dataset Description
- **Date**: Calendar day of the record.
- **Company**: OpenAI, Google, or Meta.
- **R&D_Spending_USD_Mn**: R&D investment in millions USD.
- **AI_Revenue_USD_Mn**: AI-specific revenue in millions USD.
- **AI_Revenue_Growth_%**: Daily percentage growth in AI revenue.
- **Event**: Significant company events (e.g., "AI partnership deal"; mostly "No Event").
- **Stock_Impact_%**: Daily percentage change in stock price.

Data spans ~10,959 rows (2015-2024, daily per company).

## Installation
1. Clone the repo:
3. Key sections:
- Data loading and cleaning.
- EDA (stats, plots).
- ARIMA forecasting (focused on OpenAI; extendable to others).

Example output: ARIMA forecast plot for OpenAI's stock impact (MSE ~0.34).

## Results
- Strong correlations between AI revenue growth and stock impact.
- ARIMA model provides baseline forecasts; potential for improvement with LSTM or Prophet.
- Visualizations show upward trends in R&D and revenue over time.

See the notebook for full details and plots.

## Limitations
- Synthetic data—results may not reflect real markets.
- Basic ARIMA; no external factors (e.g., market indices).
- Events are sparse and not deeply analyzed.

## Future Work
- Integrate real data (e.g., via yfinance API).
- Add machine learning models (e.g., XGBoost for regression).
- Event sentiment analysis using NLP.

## License
MIT License. Feel free to use and contribute!

Author: [AGORO TIMILEHIN]  
LinkedIn: [www.linkedin.com/in/agoro-oluwatimilehin-aba2851aa]  
Date: October 2025