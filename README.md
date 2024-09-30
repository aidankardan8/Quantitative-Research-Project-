# Quantitative Research Project: S&P 500 Stock Prediction

## Project Overview

This project focuses on building predictive models for stock prices within the S&P 500. Using Python and R, it involves data extraction, transformation, statistical analysis, and advanced modeling techniques. The goal is to predict stock prices and classify future price movements, leveraging historical OHLCV data.

## Project Plan

### 1. **Data Extraction**
- **Objective**: Dynamically extract S&P 500 stock tickers and retrieve OHLCV data for a specified time range.
- **Tools**: Python, yfinance.
- **Details**:
  - Extracted tickers from two online sources.
  - Validated tickers and downloaded historical data (Open, High, Low, Close, Volume).
  - Focused on stocks with sufficient historical data for meaningful analysis.

### 2. **Data Transformation and Preparation**
- **Objective**: Clean and preprocess data for statistical analysis.
- **Tools**: Python, R.
- **Details**:
  - Conducted correlation analysis to remove weak predictors.
  - Applied log and Box-Cox transformations to appropriate variables.
  - Reduced the initial dataset from 93 predictors to around 50 based on correlation strength and transformation suitability.

### 3. **Model Building**
- **Objective**: Build baseline models for regression and classification.
- **Tools**: R (preferred for complex modeling).
- **Details**:
  - Created baseline models with most variables log-transformed.
  - Performed initial regression and classification models to predict stock price changes.
  - Focused on the impact of key predictors on the stock price and market behavior.

### 4. **Statistical Testing and Feature Selection**
- **Objective**: Conduct multicollinearity tests and refine the model.
- **Tools**: R (VIF, partial F-tests).
- **Details**:
  - Performed Variance Inflation Factor (VIF) analysis to detect multicollinearity.
  - Employed statistical significance testing to select the best predictors.
  - Tested residuals for model accuracy and explored advanced feature selection methods like Lasso and Ridge regression.

### 5. **Advanced Statistical Techniques**
- **Objective**: Apply advanced statistical methods for deeper insights.
- **Tools**: R (ARIMA, bootstrapping, robust regression).
- **Details**:
  - Developed ARIMA models for time series analysis.
  - Used robust regression techniques to handle outliers and non-normality.
  - Applied bootstrapping to enhance model accuracy and uncertainty estimation.

### 6. **Time Series Analysis**
- **Objective**: Analyze time series behavior and trends in stock prices.
- **Tools**: R, Python.
- **Details**:
  - Created lagged variables to capture temporal relationships.
  - Investigated trends, seasonality, and volatility in the data.
  - Applied ARIMA models to predict future stock prices based on historical patterns.

### 7. **Ongoing and Planned Work**
- **Objective**: Continuously refine and expand the project.
- **Details**:
  - Exploring deeper machine learning integration, such as random forests and gradient boosting.
  - Fine-tuning predictive models using additional data and advanced statistical tests.
  - **Planned**: Implement Markov Chain Monte Carlo (MCMC) methods for further refinement of model predictions.
  - Expanding the analysis to different market conditions and economic factors.

## Results and Findings
- Most predictors required transformation (log or Box-Cox) to achieve linearity.
- Strong correlations between certain volatility indicators and price movement.
- ARIMA models provided a promising direction for time series forecasting.

## Tools and Technologies
- **Languages**: Python, R.
- **Libraries**: `yfinance`, `tidyverse`, `data.table`, `nlme`, `ta` (technical analysis), `car` (for VIF analysis).

## Next Steps
- Complete ARIMA modeling with lagged variables.
- Conduct multicollinearity testing on all features.
- Further refine models using robust regression.
- **Planned**: Begin structuring MCMC analysis for uncertainty estimation.
