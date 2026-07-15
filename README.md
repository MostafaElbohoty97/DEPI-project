# Global Stock Market Analysis Dashboard
### Graduation Project | Digital Egypt Pioneers Initiative (DEPI) - Data Analysis Track

**Dataset Source:** [Kaggle - Daily Global Stock Market Indicators](https://www.kaggle.com/datasets/aliiihussain/daily-global-stock-market-indicators)

---

## Project Overview & Concept
The **Global Stock Market Analysis** project is an end-to-end data analytics solution designed to ingest, clean, model, and visualize daily historical trading data of 10 major global stock indices (representing over 13,000 trading records). 

The primary objective of this project is to transform raw market indicators into actionable financial insights. By tracking liquidity (volume), market sentiment (Bullish vs. Bearish), historical trends, and market volatility across different countries, the project provides a unified multi-tool analytics experience utilizing **Microsoft Excel**, **Microsoft Power BI**, and **Tableau**.

---

## Data Dictionary & Schema
The dataset consists of **13,050+ rows** of historical daily stock market records. Below is the technical schema of the attributes analyzed:

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `Date` | Date | The specific trading day (YYYY-MM-DD format). |
| `Index_Name` / `Stock Index` | Text | Name of the global stock index (e.g., S&P 500, FTSE 100, Nikkei 225). |
| `Country` | Text | The country where the stock index exchange is located. |
| `Open` | Decimal | The opening price of the index on that trading day. |
| `High` | Decimal | The highest price recorded during the trading session. |
| `Low` | Decimal | The lowest price recorded during the trading session. |
| `Close` | Decimal | The closing price of the index (used as the primary benchmark). |
| `Volume` | Integer | The total number of shares/units traded (representing market liquidity). |
| `Daily Return` | Decimal | Calculated percentage of gain/loss compared to the previous session. |
| `Volatility` | Decimal | Calculated index price fluctuation metric. |
| `Market Sentiment` | Text | Classification of the day's trend (`Bullish` if Close > Open, `Bearish` if Close < Open). |

---

## Project Implementation & Tooling

The project is structured into three distinct analytical phases:

### Phase 1: Microsoft Excel (Data Engineering & Initial EDA)
* **Data Cleaning & ETL:** Used **Power Query** to handle blank/null values, format column types, and standardize country names.
* **Feature Engineering:** Created calculated columns for `Year`, `Month`, `Volatility`, and `Daily Return` using Excel formulas.
* **Pivot Tables & Exploratory Data Analysis (EDA):** Built initial pivot tables to summarize trading volumes, identify outliers, and establish baseline averages for global markets.

#### Excel Dashboard Showcase:
*(Insert your Excel Dashboard screenshots below)*
