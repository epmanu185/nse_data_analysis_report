
# NIFTY 50 and NIFTY Bank Historical Data Analysis Report
---

## Introduction:

In the ever-changing landscape of financial markets, an in-depth analysis of historical stock performance is fundamental for strategic decision-making and market understanding. This report looks into the historical data of both NIFTY 50 and NIFTY Bank, two prominent indices representing key sectors of the National Stock Exchange of India (NSE). This analysis aims to unveil crucial insights into the past year's performance (DEC 2022 - DEC 2023), covering closing prices, identifying dates of highest and lowest prices, and projecting potential percentage increases based on observed trends.

## Objective:

The primary objective of this comprehensive analysis is to provide stakeholders with valuable insights into the historical performance of NIFTY 50 and NIFTY Bank. By examining key metrics such as closing prices, high and low prices, and projecting potential future trends.

## Methodology:

To conduct this analysis, historical data for both NIFTY 50 and NIFTY Bank was obtained, encompassing columns such as Date, Open, High, Low, Close, Adjusted Close, and Volume. The study period spans the last year (DEC 2022 - DEC 2023), allowing us to capture the market dynamics over this timeframe.

## Key Findings:
---

- NIFTY 50 closing price, One year ago Vs Today; *18014.59961 Rs* (26-12-2022) & *21349.40039 Rs* (22-12-2023)
   
   ```SQL
   SELECT * FROM nse_data.nifty_50 ORDER BY Date ASC LIMIT 1
   ```
   ```SQL
   SELECT * FROM nse_data.nifty_50 ORDER BY Date DESC LIMIT 1
   ```

- NIFTY BANK closing price, One year ago Vs Today; *42859.5 Rs* (27-12-2022) & *47491.85156 Rs* (22-12-2023)
   
   ```SQL
   SELECT * FROM nse_data.nifty_bank ORDER BY Date ASC LIMIT 1
   ```
   ```SQL
   SELECT * FROM nse_data.nifty_bank ORDER BY Date DESC LIMIT 1
   ```
- Highest and Lowest Prices:

   This analysis identifies the date and corresponding prices at which both indices reached their highest and lowest points over the past year. Understanding these       extremes is crucial for assessing market volatility and potential areas of opportunity or risk.

   1. Highest price of nifty_50 is observed on DECEMBER 20, 2023 (21593 Rs)
      
   ```SQL
   SELECT * FROM nse_data.nifty_50 ORDER BY High DESC LIMIT 1
   ```
   2. Lowest price of nifty_50 is observed on MARCH 20, 2023 (16828.34961 Rs)
      
   ```SQL
   SELECT * FROM nse_data.nifty_50 ORDER BY Low DESC LIMIT 1
   ```
   3. Highest price of nifty_BANK is observed on DECEMBER 15, 2023 (48219.94922 Rs)
      
   ```SQL
   SELECT * FROM nse_data.nifty_bank ORDER BY High DESC LIMIT 1
   ```
   4. Lowest price of nifty_BANK is observed on MARCH 16, 2023 (38613.14844 Rs)
      
   ```SQL
   SELECT * FROM nse_data.nifty_bank ORDER BY Low ASC LIMIT 1
   ```

- Percentage Increase Projection:
  
   By examining the percentage increase in closing prices over the observed period, we aim to provide insights into potential future trends for both NIFTY 50 and         NIFTY Bank. This projection is based on historical data and market trends.

   To calculate the percentage increase in the stock price over the past year, we can use the following formula:

    ```
    Percentage Increase = [( Today’s Closing Price − Closing Price a year ago) / Closing Price a year ago ) × 100]
    ```
   Therefore, the percentage increase in the NIFTY BANK closing price over the past year is approximately 10.79 % and the percentage increase in the NIFTY 50 closing     price over the past year is approximately 18.5 %.




*Data Source : https://finance.yahoo.com/*

