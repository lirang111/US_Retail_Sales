# US_Retail_Sales
🛍️ U.S. Retail Sales Forecasting
This project analyzes and forecasts monthly U.S. retail sales data from 1992 to 2021 using time series modeling. Through visualization, trend analysis, and predictive modeling (SARIMA), the project offers insights into seasonal retail trends and future sales predictions.

📈 Project Overview
Data Source: U.S. Monthly Retail Sales (1992–2021)

Objective:

Understand long-term and seasonal retail sales patterns

Forecast monthly retail sales using SARIMA

Tools Used: Python, pandas, matplotlib, statsmodels, scikit-learn

🔧 Data Preparation
Raw sales data reshaped using pd.melt() to format each year and month into a long format.

Combined YEAR and MONTH into a YEAR_MONTH datetime column.

Aggregated data by both year and month to explore trends.

📊 Visualizations
Total Retail Sales by Year: Shows steady growth, resilience during 2020–2021.

Retail Sales by Month: Highlights seasonal shopping peaks (May–June, Nov–Dec).

Average Monthly Sales: Used to identify consistent month-over-month trends.

🧠 Time Series Forecasting
Model Used: SARIMA (Seasonal AutoRegressive Integrated Moving Average)

Parameters: (1,1,1)x(1,1,1,12)

Train/Test Split:

Train: Jan 1992 – Jun 2020

Test: Jul 2020 – Jun 2021

Evaluation:

RMSE on test set: ~59,307

Forecast closely tracked actual sales with minor deviations during holiday months.

📌 Key Findings
Strong seasonal effects with predictable spikes in Q2 and Q4.

Retail sales remained surprisingly strong during 2020–2021.

SARIMA provided reasonably accurate forecasts, especially in non-holiday months.

