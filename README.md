# Global Stock Market Analysis 

## Project Overview & Concept
The **Global Stock Market Analysis** project is an end-to-end data analytics solution designed to ingest, clean, model, and visualize daily historical trading data of 10 major global stock indices (representing over 13,000 trading records). 

By tracking liquidity, market sentiment, historical trends, and volatility across different countries, the project provides a unified multi-tool analytics experience utilizing **Microsoft Excel**, **Microsoft Power BI**, and **Tableau**.

---

### Graduation Project | Digital Egypt Pioneers Initiative (DEPI) - Data Analysis Track

**Dataset Source:** [Kaggle - Daily Global Stock Market Indicators](https://www.kaggle.com/datasets/aliiihussain/daily-global-stock-market-indicators)

---

## Project Objectives
The primary strategic and technical objectives of this project are:
* **Centralize Global Market Data:** Consolidate disparate daily trading metrics from 10 major global indices into a single, structured analytical pipeline.
* **Assess Market Volatility:** Track and quantify daily price fluctuations to help investors identify stable versus high-risk trading environments.
* **Analyze Liquidity Distribution:** Evaluate trading volumes across different countries to pinpoint where global financial capital and liquidity are concentrated.
* **Decipher Market Sentiment:** Create automated classifications (Bullish/Bearish) to monitor daily market direction trends over time.
* **Demonstrate Multi-Tool Proficiency:** Showcase comprehensive data analytical capabilities by delivering cohesive, specialized dashboards using Microsoft Excel, Power BI, and Tableau.


---

##  Project Contributors

We are pleased to introduce the team members collaborating on this project:

| Full Name | GitHub Account |
| :---: | :---: |
| **Hazem Shady Nasr** | [@HazemShady](https://github.com/HazemShady) |
| **Merna Elia Abdelmaboud** | [@mernaelia](https://github.com/mernaelia) |
| **Mostafa Mohamed Elbohoty** | [@MostafaElbohoty97](https://github.com/MostafaElbohoty97) |
| **Mohamed Sobhi Ibrahim** | [@mohamedabofoul](https://github.com/mohamedabofoul) |
| **Injy Makarem Abd elmenaem** | [@injymakarem](https://github.com/injymakarem) |
| **Ayatullah Ahmed Sallam** | [@AyatullahSallam](https://github.com/AyatullahSallam) |


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

### Phase 1: Power BI
Focused on data modeling, interactive layouts, and dynamic KPI tracking using DAX calculations.
* **Core KPIs & Measures Tracked:**
  * `Total Markets` (Distinct Count of Stock Indices)
  * `Average Close Price`
  * `Max Close Price`
  * `Min Close Price`
  * `Market Sentiment Ratio` (Bullish vs. Bearish distribution)

#### Power BI Dashboard Showcase:
<p align="center">
  <img width="1198" height="670" alt="1000202908" src="https://github.com/user-attachments/assets/a10419ea-d291-41e2-84de-9b3a7d4a407d" />
  <img width="1151" height="656" alt="1000202907" src="https://github.com/user-attachments/assets/59cb84f7-07b5-4146-b0a3-71d544a32596" />
<img width="1147" height="671" alt="1000202906" src="https://github.com/user-attachments/assets/9b44f478-05ea-4fe4-92cc-d2bb9317a4e9" />


</p>

---

### Phase 2: Excel

### Stock Market and Financial Insights Dashboard

This project features an interactive, dynamic Excel Dashboard designed to analyze global stock market trends, financial performance, and volatility. The dashboard is built on a dynamic architecture where all visualizations update instantly based on user interaction.

#### Dashboard Overview

The dashboard serves as a unified interface that consolidates vital financial and market information into a single screen. It provides stakeholders with an interactive environment to explore data dynamically. 

By interacting with the dashboard, users can:
* Select and filter by a specific Country.
* Select and filter by a specific Stock Index.
* Select and filter by a specific Sector.
* Adjust and change the Timeframe.
* Observe all visual elements and charts updating instantly in real-time.

#### Key Performance Indicators (KPIs) and Visualizations

The dashboard is structured into specific dynamic sheets, each tracking critical performance metrics and financial indicators:

##### 1. Interactive Filters (Slicers)
These components allow the user to isolate and display specific subsets of data instead of viewing the entire dataset at once:
* **Country:** Filters the metrics to display data for a specific country (such as USA, UK, or Germany), enabling a direct performance comparison between countries.
* **Stock Index (Index Name):** Filters the metrics to display data for a specific index (such as NASDAQ, S&P 500, FTSE, or DAX), allowing focused tracking of a single index's performance.

##### 2. Market Performance Metrics

* **Close Price Over Time (Line Chart):**
  * **Horizontal Axis (X-Axis):** Date.
  * **Vertical Axis (Y-Axis):** Close Price.
  * **Purpose:** Identifies the overall trend of the market.
  * **Function:** Determines whether the stock index is in a rising (bullish), falling (bearish), or stable state.

* **Index Performance Ranking (Bar Chart):**
  * **Purpose:** Compares different indices (such as NASDAQ, S&P 500, or FTSE).
  * **Function:** Identifies which stock index achieved the highest value.

* **Volume Over Time (Area Chart):**
  * **Purpose:** Displays the trading volume over a period of time.
  * **Function:** It represents the performance trend similarly to a line chart, but with the area underneath the line shaded to visually emphasize the strength of growth or decline.

* **Countries by Trading Volume (Bar Chart):**
  * **Purpose:** Compares a specific value (such as Average Volume) for each stock index.
  * **Function:** Instantly highlights and identifies the best-performing index.

##### 3. Financial Insights Metrics

This section is dedicated entirely to evaluating the corporate and financial performance of indices and companies:

* **Revenue Comparison:**
  * **Purpose:** Compares total revenues generated among different companies.
  * **Function:** Pinpoints which company achieved the highest revenue.

* **Profit Comparison:**
  * **Purpose:** Displays and compares profitability metrics.
  * **Function:** Identifies the most profitable companies.

* **Index Performance Ranking (Financial Index Performance):**
  * **Purpose:** Sorts and ranks all available indices from the best-performing to the worst-performing.
  * **Function:** Helps to instantly identify the top-performing index.

* **Trend and Volatility Analysis (Max Close vs. Min Close / Average Volatility) (Line Chart):**
  * **Purpose:** Displays the historical change of specific financial metrics over time, such as Profit, Revenue, or Market Value.
  * **Function:** Analyzes financial trends and price fluctuations.

#### Technical Architecture

##### Pivot Tables
The dashboard relies entirely on Pivot Tables to process the backend data:
* **Function:** They summarize thousands of raw data rows into structured, simplified tables.
* **Metrics Aggregated:** Calculates Average, Sum, Count, Maximum (Max Value), and Minimum (Min Value).

##### Pivot Charts
* All visual charts on the dashboard are Pivot Charts directly linked to their respective Pivot Tables.
* Any change made to the filters (Slicers) or the underlying dataset automatically updates the Pivot Tables and refreshes all charts instantly.

#### Excel Dashboard Showcase:
<p align="center">
 <img width="863" height="472" alt="1000202909" src="https://github.com/user-attachments/assets/2ea128ee-4d98-4998-9492-ac3b60257ead" />

 <img width="758" height="452" alt="1000202910" src="https://github.com/user-attachments/assets/99f73c72-7f3e-48ed-b84f-dd808f5e1015" />

</p>

---
### Phase 3: Tableau
Focused on advanced visual analytics, geographical mapping, and market correlation.
* **Core KPIs & Visual Analysis:**
  * `Volume by Country` (Spatial liquidity tracking)
  * `Volatility vs. Volume` (Correlation scatter plots)
  * `Historical Price Trends` (Time-series forecasting)

#### Tableau Dashboard Showcase:
<p align="center">
  <img width="1361" height="846" alt="1000202903" src="https://github.com/user-attachments/assets/acff6945-240f-4caf-8f90-1be449c75387" />
<img width="1367" height="847" alt="1000202904" src="https://github.com/user-attachments/assets/3c378503-5217-4791-a457-d6351401358b" />
<img width="1362" height="846" alt="1000202905" src="https://github.com/user-attachments/assets/844b8d90-d401-4526-842d-6d0e12aa0e43" />

</p>

---
## Key Insights & Findings
1. **Liquidity Distribution:** The US market dominates global liquidity with a massive Total Volume of **100.05B**, followed by Hong Kong and Japan.
2. **Market Sentiment Equilibrium:** Historically, global markets display a highly balanced distribution of trend directions with approximately **50.67% Bearish** sessions vs. **49.33% Bullish** sessions.
3. **Volatility Assessment:** Developed a customized Volatility index showing that the UK market (FTSE) showed relatively stable volatility (average of 5.51) despite market fluctuations.
