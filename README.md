Forward
=======

For my capstone project, I wanted to do something a bit **different**:

-         I wanted to move away from the limitations of *Kaggle* and try to make my own dynamic dataset using *APIs*.

-         I wanted to continue with the *storytelling* from my [Individual Formulative Assignment](https://github.com/tishsrisasi/Individual_Formative_Assignment) (link provided).

-         I wanted to mimic predictive Machine Learning models like those currently used in real-world situations.        

**Teerachai ('Tish') Srisasi**
**(19th January 2026)**

ETF Prediction ML Models: A Brief Background
============================================

Research shows most financial institutions will spend a hefty share of their financial budget and resources building ML models to *anticipate* and *predict* ETF price direction accuracy (whether the price will go up or down on a given timeframe, say hourly or daily). They do this to generate ETF buy/sell signals, by feeding their ML models with premium (read costly) real-time financial market data. Although the overall process is proving a relatively expensive endeavour for the financial sector, at the time I'm writing this, they are only getting accuracy rates of around 50-57% (this is little better than flipping a coin). Research also shows that ML models to predict ETF price still are sadly not considered as normal practice (again at the time of writing).

Business Opportunity/Challenge & Context
========================================

What if there was a way to accurately predict **BOTH** *ETF price direction* **AND** *ETF closing price* using just generic, easily accessible & freely available macroeconomic indicator (time series) data (e.g. US Gross Domestic Product (GDP) figures generated daily)?

**For context - business use case scenario example:** the proposed ML ETF **close price** prediction model from this project could provide reliable insight to investors in real-time (by using a live ETF data feed) that through valuation, if the ETF(s) in his/her portfolio is *under or over-priced*. If say an ETF is expected to be *under-priced*, this could possibly trigger a 'buy order' in the anticipation that the closing price of the ETF would more than likely go up as the ETF market corrects itself. The reverse would be true for *over-priced* ETFs -- a 'sell order' could be anticipated in advance. In both cases the investor could make a decent profit if he acted accordingly, using  the model predictive prowess to guide him/her.

**Similarly**, accurately predicting ETF **price direction** could EVENTUALLY provide an investor with market movement anticipation (say if the ETF market is 'bullish' or 'bearish'), optimise his/her trading strategies and help with effective market/investment risk management.

This model, SHOULD creates business value and without a live feed could still be used for back-testing ETF trade data.

Business Requirement, Scope & Hypotheses
========================================

Requirement One-Line Summary:
-----------------------------

*"Can Machine Learning models utilise generic, publicly available macroeconomic indicator data to accurately predict ETF (daily) closing price & (daily) price direction?"*

Additional Business Requirement
-------------------------------

*Find a way to accurately predict closing price for up to 20 ETFs at the same time (running multiple predictive models).*

Business Variable Scope
-----------------------

| **ETF:** | US-Based ETFs only |
| --- |  --- |
| **Macro-Economic Data:** | US-Based Indicators Only |
| **Time Series Date Range:** | 01/01/2020 to 31/12/2025 |
| **Time Series Data Interval:** | 1 day (1d) |

### Business Subject: ETF Scope (Total of 20):

| **Grouping Description** | **Ticker Name** |
| --- |  --- |
| Core S&P/Total Market | 'SKY', 'VOO', 'IVV', 'VTI', 'ITOT' |
| Nasdaq/Growth | 'QQQ', 'QQQE' |
| Small/Mid/Growth/Value | 'IWM', 'IWF', 'IWD', 'MDY' |
| Tech/Finance/Energy | 'XLK', 'XLF', 'XLE', 'XLV' |
| Bonds | 'TLT', 'BND', 'HYG' |
| International (US-listed) | 'VEU', 'EFA' |

Hypotheses (what I intend to prove):
------------------------------------

-         **H0:** Machine Learning ETF (**H2** and **H3**) predictions accuracy relies heavily on macroeconomic data.

-         **H1:** Most ETF close prices and price direction are heavily influenced by GDP data figures

-         **H2:** Most ETF close prices are accurately predicted using *just* macroeconomic data

-         **H3:** Most ETF price directions are accurately predicted, again using just macroeconomic data

 Hypotheses Validation Methods (what I will use to prove the above):
--------------------------------------------------------------------

-         **V0:** Parallel testing datasets with and without macroeconomic data using Classical Machine Learning

-         **V1:** Classical Machine Learning -- Feature Selection

-         **V2:** Classical Machine Learning -- Linear Regression

-         **V3:** Feature Engineering - Machine Learning -- Classification by Random Forrest

Dataset Source(s): Considered
=============================

Static Dataset Source (used initially for research, but dropped in favour of more dynamic APIs below)

| **Name of Dataset** | Huge Stock Market Dataset |
| --- |  --- |
| **Data Description** | Historical daily prices and volumes of all U.S. stocks and ETF                 |
| **Data Source Origins** | [Kaggle](https://www.kaggle.com/) |
| **Web URL** | <https://www.kaggle.com/datasets/borismarjanovic/price-volume-data-for-all-us-stocks-etfs> |
| **Dataset Original Filenames** | Archive.zip (containing various stock and ETF data files) |
| **Dataset version and file size** | 516MB |
| **Useability Rating** | 7.50/10.00 |
| **Dataset Dated** | 16/01/2026 (Download Date) |

Dataset Source(s): Used
=======================

Dynamic API Dataset Source (two data sources were used **FRED** for macroeconomic indicators and **Yahoo Finance** for ETF)

| FRED (or Federal Reserve Economic Data) -- Federal Reserve Bank of St. Louis | <https://fred.stlouisfed.org/> |
| --- |  --- |
| Yahoo Finance | <https://finance.yahoo.com/markets/etfs/most-active/> |

Audit Trail: Project Board & Documents Provided
-----------------------------------------------

| **Documentation/Link** | **Document Format, Date & Version Control** |
| --- |  --- |
| Business Requirement Document (mock email format) | Markdown, 18/01/2026, Version 1.0 |
| Functional Specification Document | Markdown, 18/01/2026, Version 1.0 |
| Testing Checklist & Results Summary | Markdown, 18/01/2026, Version 1.0 |
| Project Board | https://trello.com/b/bhCNa53F/capstone-project-tish-srisasi-etf-close-price |

Git-Hub Directory Structure
---------------------------



	



Project Delivery Challenges & Bug Fixes
---------------------------------------

### Data Sourcing

### Machine Learning Models

### Dashboards

Dashboards: Deployment
----------------------
## Power BI - Board 1 (Dashboard)
![Power BI](reports/powerBI2_board1_db.jpg)
## Power BI - Board 2 (Dashboard)
![alt text](reports/powerBI1_board2_db.jpg)
## Tableau - Heatmap Wall (Dashboard)
![alt text](reports/tableau2_heatmap_wall_db.jpg)
## Tableau - Health Check - ETF Watcher's Screen (Dashboard)
![alt text](reports/tableau3_etf_health_check_db.jpg)
## Tableau = Overall Dashboard
![alt text](reports/tableau1_overall_db.jpg)

| **Application** | **Link** |
| --- |  --- |
| Tableau: |  |
| \-          Overall | [https://public.tableau.com/app/profile/teerachai.srisasi/viz/Tableau\_ETF\_Final/OVerall](https://public.tableau.com/app/profile/teerachai.srisasi/viz/Tableau_ETF_Final/OVerall) |
| \-          Heatmap Wall | [https://public.tableau.com/app/profile/teerachai.srisasi/viz/Tableau\_ETF\_Final/Heatmaps](https://public.tableau.com/app/profile/teerachai.srisasi/viz/Tableau_ETF_Final/Heatmaps) |
| \-          ETF Health Check: |  |
| \-          QQQ | [https://public.tableau.com/app/profile/teerachai.srisasi/viz/Tableau\_ETF\_Final/QQQ](https://public.tableau.com/app/profile/teerachai.srisasi/viz/Tableau_ETF_Final/QQQ) |
| \-          QQQE | [https://public.tableau.com/app/profile/teerachai.srisasi/viz/Tableau\_ETF\_Final/QQQE](https://public.tableau.com/app/profile/teerachai.srisasi/viz/Tableau_ETF_Final/QQQE) |
| \-          VOO | [https://public.tableau.com/app/profile/teerachai.srisasi/viz/Tableau\_ETF\_Final/VOO](https://public.tableau.com/app/profile/teerachai.srisasi/viz/Tableau_ETF_Final/VOO) |
| Power BI:(No Cloud Service -- Local File Only) |  ![alt text](reports/power_bI_file.jpg)|



Main Data Analysis Tools and Libraries
--------------------------------------

Project Results Summary
-----------------------

Business Applications
---------------------

### Next Steps

-          Feed the Yahoo Finance: ETF and FRED: macroeconomic indicator data directly into Power BI and Tableau

-          Use the predictive models to create an app in Streamlit -- then deploy

-          Add new ETF and Macroeconomic Features for 'premium users' (list provided)

-          Test other types of ML models and see which one gives better predictive accuracy

-          Finally build a live direct API feed into the ML model and test to see if this can be used to accurately predict ETF direction and current price.

-          Expand to Global ETF & Macroeconomic datasets using available and relevant APIs.

-          Further use of ML Cross-Validation models for transparency.

Ethical Considerations/GDPR
---------------------------

-          **Disclaimer:** As per the **section** below -- I must emphasise that this project is educational only and utilises only public and freely available FRED economic data. The model has limitations and should NOT be used commercially.

-          **Ethical Consideration** - Model's limitations: Please note that past performance of economic indicators does not predict FUTURE ETF close prices due to the uncertainty of market volatility, BLACK SWAN events and potential overfitting risks.

-          **BIAS and fairness concerns** -- as mentioned, the FRED economic data's limited scope covers just US-based ETFs. Therefore, it should NOT be used on a global scale (country bias), e.g. predicting Global ETF close prices.

-          **Legal note** -- FRED data is public domain from the St. Louis Fed -- and is free for non-commercial use only -- there is no direct/indirect endorsement here from me and you are free to select other sources as a basis for running your models on.

-          **Regulatory compliance** -- any *performance claims* within this project are speculative and should not be considered as financial advice.

-          **GDPR notes** -- FRED and Yahoo Finance data contains no personal data, so GDPR is not applicable -- this capstone is compliant be default.

Disclaimer (UK)
---------------

*This repository and the machine learning model it contains are provided **for educational and research purposes only** and **do not constitute investment or financial advice or a personal recommendation** under UK law. Users should not rely on any content or outputs as a basis for making investment decisions and should seek advice from an independent, authorised financial adviser.*

*The author is **not authorised or regulated by the Financial Conduct Authority (FCA)**, and nothing herein is a financial promotion. Use of the code, models and information is entirely at your own risk, and the author accepts **no liability** for any loss or damage arising from their use or reliance.*

Credits
-------

Acknowledgements
----------------