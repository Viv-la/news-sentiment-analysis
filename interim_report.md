# Interim Report — Financial News Sentiment Analysis

## Week 1 Challenge — Nova Financial Solutions

This interim report summarizes the progress made toward analyzing the relationship between financial news sentiment and stock market behavior. The project focuses on combining financial news headlines with historical stock price data to identify patterns, trends, and potential predictive relationships between market sentiment and stock price movements.

The analysis conducted so far includes exploratory data analysis on the financial news dataset, initial technical analysis on stock price data, and preliminary sentiment analysis using natural language processing techniques.

# Project Objective

The objective of this project is to investigate how financial news sentiment may influence stock market performance. Specifically, the project aims to:

- Analyze financial news headlines and publisher behavior
- Identify trends and patterns in financial news publications
- Apply sentiment analysis techniques to quantify headline sentiment
- Compute technical indicators from historical stock price data
- Explore relationships between sentiment and stock market movements

# Environment and Git Setup

A professional project structure was established using Git and GitHub for version control and collaboration. A dedicated branch (`task-1`) was created for development activities, and changes were committed regularly using descriptive commit messages following conventional commit practices.

A Python virtual environment was configured to ensure reproducibility, and all required dependencies were stored in the `requirements.txt` file. The project structure includes organized folders for notebooks, raw data, scripts, tests, and source files.

Tools and libraries used include:
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- NLTK
- VADER Sentiment

# Data Loading and Cleaning

Two primary datasets were used during this phase:

1. Financial news dataset containing headlines, publishers, publication dates, and stock symbols
2. Historical stock price datasets for multiple companies including AAPL, AMZN, GOOG, META, and NVDA

During preprocessing:
- malformed rows in the news dataset were skipped
- unnecessary columns were removed
- date columns were converted into datetime format
- multiple stock CSV files were merged into a unified dataframe
- datasets were sorted chronologically for time-series analysis

# Exploratory Data Analysis Findings

Initial exploratory analysis revealed several notable patterns:

- Financial news publication volume increased significantly over time, with major spikes observed around periods of increased market activity.
- Certain publishers contributed a disproportionately high number of articles.
- Frequently occurring keywords were strongly associated with earnings reports, stock ratings, market performance, and analyst recommendations.
- Most headlines exhibited relatively neutral sentiment, although positive and negative variations were identified across different stocks.
- Some stocks consistently appeared more frequently in financial reporting than others.

# Initial Technical Analysis

Several technical indicators were implemented to analyze stock market behavior:

- Simple Moving Average (SMA)
- Exponential Moving Average (EMA)
- Relative Strength Index (RSI)
- Moving Average Convergence Divergence (MACD)

The indicators revealed:
- strong long-term upward trends in several stocks
- periods of increased volatility
- momentum shifts identified through MACD crossover behavior
- potential overbought and oversold conditions identified using RSI

# Sentiment Analysis Preview

A preliminary sentiment analysis pipeline was implemented using the VADER sentiment analyzer. Sentiment scores were generated from financial news headlines and classified into positive, neutral, and negative categories.

Initial findings suggest that:
- the majority of headlines are neutral in tone
- sentiment varies across stocks and reporting periods
- sentiment signals may provide additional context for interpreting stock market behavior

# Challenges Encountered

Several challenges were encountered during this phase of the project:

- The financial news dataset contained malformed rows that required special handling during loading.
- Date formatting inconsistencies initially affected time-series analysis.
- Managing multiple stock CSV files required dataset consolidation and restructuring.
- Large dataset sizes increased processing time for certain NLP operations.

# Next Steps

The remaining phase of the project will focus on:

- completing full sentiment correlation analysis
- aligning news publication dates with stock trading dates
- calculating Pearson correlation coefficients
- generating scatter plots for sentiment vs stock returns
- improving visualization quality and notebook storytelling
- refining investment insights and recommendations

# Conclusion

Significant progress has been made toward understanding the relationship between financial news sentiment and stock market behavior. The project now includes structured exploratory analysis, technical indicator implementation, and preliminary sentiment analysis workflows.

The next phase will focus on integrating sentiment and stock performance data to evaluate whether financial news sentiment can serve as a meaningful predictive signal for stock market movement.