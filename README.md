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

This project features an interactive Power BI dashboard designed to analyze global stock market trends by studying financial index data across multiple countries[cite: 3]. It assists investors and data analysts in tracking market movements, comparing performance across countries, and analyzing trading volumes, returns, and price trends over time[cite: 3].

The dashboard is built with fully interactive elements, allowing users to seamlessly filter data by country, year, month, or index name to extract key insights and drive data-backed investment decisions[cite: 3].

---

#### Key Performance Indicators (KPIs) & DAX Measures

The dashboard utilizes specialized DAX measures to calculate critical financial metrics dynamically:

##### 1. Total Markets
* **Formula:** `Total Markets = DISTINCTCOUNT(Sheet1[Index_Name])`[cite: 3]
* **Description:** Calculates the total number of unique stock markets or indices present in the dataset[cite: 3].
* **Value:** Helps track the scale of the dataset and the number of active markets under analysis[cite: 3].

##### 2. Average Close Price
* **Formula:** `Average Close = AVERAGE(Sheet1[Close])`[cite: 3]
* **Description:** Calculates the average closing price across selected records[cite: 3].
* **Value:** Measures the overall average baseline performance of indices during the selected period[cite: 3].

##### 3. Max Close
* **Formula:** `Max Close = MAX(Sheet1[Close])`[cite: 3]
* **Description:** Calculates the highest closing price recorded[cite: 3].
* **Value:** Pinpoints the peak value achieved by the stock index within the filtered timeframe[cite: 3].

##### 4. Min Close
* **Formula:** `Min Close = MIN(Sheet1[Close])`[cite: 3]
* **Description:** Calculates the lowest closing price recorded[cite: 3].
* **Value:** Identifies the minimum baseline value recorded for the index[cite: 3].

##### 5. Average Return
* **Formula:** `Average Return = AVERAGE(Sheet1[Daily_Return])`[cite: 3]
* **Description:** Calculates the average daily return[cite: 3].
* **Value:** Evaluates the overall average profitability or loss rate of the selected indices[cite: 3].

##### 6. Total Volume
* **Formula:** *Standard Sum aggregation on the Volume column*[cite: 3]
* **Description:** Calculates the total cumulative trading volume[cite: 3].
* **Value:** Measures overall market activity, transaction density, and trading liquidity[cite: 3].

---

#### Dashboard Interactive Filters (Slicers)

* **Slicer (Index Name):** Filters all visuals to focus on a specific stock index's performance[cite: 3].
* **Slicer (Month):** Enables month-by-month historical analysis[cite: 3].
* **Slicer (Year):** Filters the dataset to display annual performance[cite: 3].
* **Slicer (Country):** Filters the dashboard to display metrics for a specific country[cite: 3].

---

#### Visualizations & Analytical Insights

##### 1. Market Trend Analysis
* **Close Price Over Time (Area Chart):**
  * **Description:** Visualizes the fluctuations of the average closing price across years[cite: 3].
  * **Value:** Tracks long-term market trends to quickly determine if the market is overall growing, declining, or consolidating[cite: 3].

##### 2. Country & Index Comparisons
* **Top Countries by Average Close (Clustered Column Chart):**
  * **Description:** Compares the average closing prices across different countries[cite: 3].
  * **Value:** Instantly identifies the leading global markets by closing price and simplifies international index comparison[cite: 3].

##### 3. Market Sentiment Distribution
* **Bullish vs. Bearish (Donut Chart):**
  * **Description:** Displays the percentage distribution of the market status (rising vs. falling)[cite: 3].
  * **Value:** Provides a high-level snapshot of global market sentiment, showing the exact ratio of bullish versus bearish days[cite: 3].

##### 4. Geographic Analysis
* **Average Close by Country (Azure Map):**
  * **Description:** Plots countries on a global map, where bubble sizes correspond to their average closing price[cite: 3].
  * **Value:** Offers a geographical overview of market performances, visually emphasizing stronger economic zones[cite: 3].

##### 5. Liquidity & Trading Strength
* **Total Volume by Country (Treemap):**
  * **Description:** Represents the total trading volume for each country using sized tiles[cite: 3].
  * **Value:** Easily distinguishes which countries hold the largest shares of market liquidity and trading activity[cite: 3].

##### 6. Return Evaluation
* **Average Daily Return (%) by Country (Clustered Column Chart):**
  * **Description:** Compares the average daily return percentages across countries[cite: 3].
  * **Value:** Rates the performance of each country based on returns, highlighting the most profitable and the weakest markets[cite: 3].

##### 7. Granular Data Reference
* **Performance Summary (Table):**
  * **Description:** Displays a comprehensive tabular view of each country alongside its key metrics: *Total Volume*, *Average Return*, *Average Close*, and *Average Volatility*[cite: 3].
  * **Value:** Serves as a reference table that supports visual insights with precise, numeric details[cite: 3].

---

#### Power BI Dashboard Showcase:
<p align="center">
  <img width="1198" height="670" alt="1000202908" src="https://github.com/user-attachments/assets/a10419ea-d291-41e2-84de-9b3a7d4a407d" />
  <img width="1151" height="656" alt="1000202907" src="https://github.com/user-attachments/assets/59cb84f7-07b5-4146-b0a3-71d544a32596" />
<img width="1147" height="671" alt="1000202906" src="https://github.com/user-attachments/assets/9b44f478-05ea-4fe4-92cc-d2bb9317a4e9" />


</p>

---

### Phase 2: Excel

<p align="center">
 <img width="863" height="472" alt="1000202909" src="https://github.com/user-attachments/assets/2ea128ee-4d98-4998-9492-ac3b60257ead" />


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

<p align="center">
 <img width="758" height="452" alt="1000202910" src="https://github.com/user-attachments/assets/99f73c72-7f3e-48ed-b84f-dd808f5e1015" />


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
