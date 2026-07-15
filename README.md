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
# Stock Market Performance and Financial Insights Dashboard

An interactive, dynamic Excel Dashboard designed to track, analyze, and visualize global stock market indices and financial performance. This project leverages advanced Excel capabilities, Pivot Tables, and dynamic charts to transform raw financial datasets into actionable business intelligence.

---

## Project Overview

[cite_start]The primary goal of this project is to analyze global stock market trends and corporate financial metrics using Excel[cite: 2].

### Key Objectives:
* [cite_start]**Index Tracking:** Monitor and evaluate the performance of various global stock indices over time[cite: 4].
* [cite_start]**Price Comparison:** Compare stock prices and trading volumes across different markets[cite: 5].
* [cite_start]**Financial Analysis:** Analyze corporate revenue, profits, and overall market value[cite: 6].
* [cite_start]**Performance Ranking:** Easily identify top-performing and underperforming indices and countries[cite: 7].
* [cite_start]**Data-Driven Decisions:** Facilitate fast, strategic decision-making through dynamic charts and interactive filters[cite: 8].

---

## Interactive Filters (Slicers)

[cite_start]Slicers allow users to filter the entire dashboard dynamically, isolating specific data points instead of looking at the entire dataset at once[cite: 10].

### 1. Market Filters
* [cite_start]**Country Slicer:** Filters data to display metrics for a specific country (such as China, France, Germany, Hong Kong, Japan, Pakistan, UK, or USA)[cite: 25, 26, 27, 28, 29, 30, 31, 32, 33].
  * [cite_start]**Benefit:** Enables direct performance comparison between countries[cite: 39].
* [cite_start]**Stock Index Slicer:** Filters the dashboard to show data for a specific stock index (such as CAC 40, DAX, Dow Jones, FTSE 100, Hang Seng, KSE 100, NASDAQ Composite, Nikkei 225, S&P 500, or SSE Composite)[cite: 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24].
  * [cite_start]**Benefit:** Allows focused tracking of a single index's performance[cite: 47].

---

## Market Performance Page Visualizations

### 1. Line Chart: "Close Price Over Time"
* [cite_start]**X-Axis (Horizontal):** Date/Time (Months)[cite: 51, 52].
* [cite_start]**Y-Axis (Vertical):** Close Price[cite: 53, 54].
* [cite_start]**Purpose:** Identifies the overall market trend[cite: 55, 56].
* [cite_start]**Business Value:** Helps investors instantly see if an index is in a Bullish (rising), Bearish (falling), or Stable phase[cite: 57, 58, 59].

### 2. Bar Chart: "Index Performance Ranking"
* [cite_start]**Description:** Compares the performance percentage or index values of major indices (such as NASDAQ, S&P 500, FTSE, or DAX)[cite: 88, 89, 90, 91, 92, 93].
* [cite_start]**Business Value:** Easily identifies which stock index has achieved the highest return or value[cite: 95].

### 3. Area Chart: "Volume Over Time"
* [cite_start]**Description:** Similar to a Line Chart, but the area beneath the trend line is shaded[cite: 98, 100].
* [cite_start]**Business Value:** Clearly visualizes market liquidity and highlights the strength of trading volume growth or decline over a specific timeframe[cite: 99, 101, 102].

### 4. Horizontal Bar Chart: "Countries by Trading Volume"
* [cite_start]**Description:** Compares specific trading volume metrics across different countries[cite: 128, 129, 130].
* [cite_start]**Business Value:** Instantly highlights the most active and liquid geographic markets[cite: 134].

---

## Financial Insights Page Visualizations

[cite_start]This page focuses entirely on the financial performance, returns, and volatility of the underlying assets[cite: 150, 151].

### 1. Revenue Comparison
* [cite_start]**Description:** Compares total revenue generated across different entities or companies[cite: 152, 153].
* [cite_start]**Purpose:** Easily identifies the highest revenue-generating assets[cite: 154, 155].

### 2. Profit Comparison: "Average Daily Return by Country"
* [cite_start]**Description:** Displays the daily returns and profitability metrics grouped by country[cite: 174, 175, 176].
* [cite_start]**Purpose:** Pinpoints which countries/markets yield the highest average profitability[cite: 177, 178].

### 3. Index Performance Ranking Chart
* [cite_start]**Description:** Sorts and ranks global indices from best to worst performing[cite: 191, 193, 194].
* [cite_start]**Purpose:** Helps portfolio managers quickly determine which index is leading the market[cite: 200].

### 4. Trend and Volatility Analysis (Max Close vs. Min Close / Average Volatility)
* **Description:** Uses combo charts (line and column) to track key financial metrics such as:
  * [cite_start]Average Volatility by Country [cite: 234]
  * [cite_start]Total Profit and Revenue [cite: 235, 236]
  * [cite_start]Overall Market Value [cite: 237]
* [cite_start]**Purpose:** Analyzes price fluctuations, risk factors (volatility), and historical trends[cite: 238, 239].

---

## Technical Architecture

### Pivot Tables
[cite_start]The backbone of this dashboard consists of multiple dynamic Pivot Tables[cite: 241, 246]. 
* [cite_start]**Function:** They summarize thousands of rows of raw, unstructured market data into clean, aggregated summaries[cite: 247, 248].
* [cite_start]**Metrics Tracked:** Average, Sum, Count, Maximum, and Minimum values[cite: 249, 250, 251, 252, 253].

### Pivot Charts
[cite_start]All visualizations are built as Pivot Charts, meaning they are directly linked to their corresponding Pivot Tables[cite: 240, 241]. 
* [cite_start]**Dynamic Interactivity:** Any filter applied through the Slicers instantly updates the Pivot Tables, which in turn automatically updates all charts in real-time[cite: 242, 243, 244, 245].

---

## Dashboard Interface and User Experience

[cite_start]The final Dashboard consolidates all vital market information into a single, cohesive, and visually appealing interface[cite: 254, 255].

**Interactive capabilities provided to the user:**
1. [cite_start]Filter by Country[cite: 256, 257].
2. [cite_start]Filter by Stock Index[cite: 256, 258].
3. [cite_start]Filter by Sector[cite: 256, 259].
4. [cite_start]Adjust the Timeframe[cite: 256, 260].
5. [cite_start]Watch all charts and performance rankings update instantly for dynamic, real-time reporting[cite: 256, 261].

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
