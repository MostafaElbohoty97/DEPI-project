# Global Stock Market Analysis 



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
| :--- | :--- |
| **Mostafa Mohamed Elbohoty** | [@MostafaElbohoty97](https://github.com/MostafaElbohoty97) |
| **Hazem Shady Nasr** | [@HazemShady](https://github.com/HazemShady) |
| **Merna Elia Abdelmaboud** | [@mernaelia](https://github.com/mernaelia) |
| **Mohamed Sobhi Ibrahim** | [@mohamedabofoul](https://github.com/mohamedabofoul) |
| **Injy Makarem Abd elmenaem** | [@injymakarem](https://github.com/injymakarem) |
| **Ayatullah Ahmed Sallam** | [@AyatullahSallam](https://github.com/AyatullahSallam) |

---




---

## Project Overview & Concept
The **Global Stock Market Analysis** project is an end-to-end data analytics solution designed to ingest, clean, model, and visualize daily historical trading data of 10 major global stock indices (representing over 13,000 trading records). 

By tracking liquidity, market sentiment, historical trends, and volatility across different countries, the project provides a unified multi-tool analytics experience utilizing **Microsoft Excel**, **Microsoft Power BI**, and **Tableau**.

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

### Phase 1: Excel
Focused on data engineering, cleaning, and calculating core market metrics using Power Query and Excel formulas.
* **Core KPIs & Metrics Tracked:**
  * `Daily Return` (Day-over-day price change percentage)
  * `Volatility` (Daily price fluctuation range)
  * `Total Volume` (Overall market liquidity)

#### Excel Dashboard Showcase:
<p align="center">
 <img width="863" height="472" alt="1000202909" src="https://github.com/user-attachments/assets/2ea128ee-4d98-4998-9492-ac3b60257ead" />

 <img width="758" height="452" alt="1000202910" src="https://github.com/user-attachments/assets/99f73c72-7f3e-48ed-b84f-dd808f5e1015" />

</p>

---

### Phase 2: Power BI
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

---
