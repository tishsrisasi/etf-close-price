**Email To: Tish S.**

**Email From: Sarah F.**

**Dated: 19th January 2026**

***RE: ETF Prices Project - Data Analytics Business Requirements Document (Pending)***

Hi Tish,

*Hoping you're having a good 2026 so far!*

Apologies for not getting back to you sooner, but it's been quite hectic here over the last few months! The good news is my stakeholders have read your proposal to use data analytics to help us with our new business venture (just to remind you what we discussed I've put all the notes [here](https://github.com/tishsrisasi/Individual_Formative_Assignment/blob/main/README.md)) and they have decided to proceed with your recommendations.

Therefore, I would like to get things started and I'm very keen for you to realise your 'Next Steps' (in order of importance):

-         **Sourcing of Real-Time data**

-         **Application of Machine Learning**

-         **Dashboards**

To be honest, I've not had time to put the below feedback from various departmental heads and 'SMEs' {Subject-Matter-Experts} into a formal Business Requirements Document, but it should provide you with enough details to get you started. I promise I'll continue to work with the relevant teams here and provide you with more details and any updates (where needed) as soon as they become available.

Just to mix things up a bit, since I saw you over coffee last year, we've recently received several new investor clients with a strong interest in US-Based ETFs. Between you and me, I think this is due to the current US Government Administration's foreign policy activities, as many people are hoping this will drive up stocks and consequently raise ETF prices. Looks like *Imperialism* is back on the menu! {Satire}

So, for the time being, please shift your focus from Global ETFs to analysing just US ETFs (for now, I don't mind if the ETF incorporates Global indexes if they are US-based). We can pick up on Global ETFs as a requirement again once the recent appetite for US ETFs diminishes somewhat.

**Sourcing of Real-Time data**

As you mentioned in your finding, we need to improve on the data source, and I think we won't be able to use *Kaggle* like we did before. However, you might want to use it earlier on in your analysis just to get a 'feel' for real ETF market data: There's one [dataset](https://www.kaggle.com/datasets/borismarjanovic/price-volume-data-for-all-us-stocks-etfs) which is worth look at for context.

We'll leave the sourcing of data to your good self. However, there's a few essential requirements to note:

-         We will need the following datasets:

1.   Daily **US Macroeconomic Indicator Data** (which **MUST** include Gross Domestic Product -- GDP figures. The rest of the indicators, I'll leave it up to you to choose.)

2.   Daily **ETF Market Data** (which **MUST** include the *Trade Volumes* and *Closing Price*)

-         The above datasets must be **relatable by date**, so a "Time Series" for both is a must.

-         The above datasets must be of **high quality** without any missing values -- we expect something closer to 'idealistic' data as we don't have the resources to clean the data in-house yet.

-         **The datasets must preferably be available for free** (or sourced from the public domain) as I've not yet received approval for the premium market data subscription. Again, I'm hoping this will be done sooner than later but for now, please 'grab' whatever's out there!

-         The datasets must provide the following **date range: 1st Jan 2020 to 31st December 2025** (and capture the period where Covid hits the US -- a *Jimmy* from my Economic Data BA team is keen to see its impact on ETF pricing as well as on macroeconomic indicators).

-         ETF datasets must include the following 'Tickers' (at least to start with, we can get more added later).

| **Sample Ticker Name:** |
| --- |
| 'SKY', 'VOO', 'IVV', 'VTI', 'ITOT' |
| 'QQQ', 'QQQE' |
| 'IWM', 'IWF', 'IWD', 'MDY' |
| 'XLK', 'XLF', 'XLE', 'XLV' |
| 'TLT', 'BND', 'HYG' |
| 'VEU', 'EFA' |

**Application of Machine Learning**

Again, I'll leave the choice of ML predictors to you as you've probably come across a few on your course so far -- please for now choose just the best one or two models to predict the following:

1.       Daily ETF **Closing Price**. Only consider model(s) that have a *R-Squared* score of over 90%)

2.       Daily ETF **Price Direction** (i.e. if the ETF Closing Price was higher or lower than the day before) -- I need to know if it's up or down however, you should also record any that stayed the same. Only consider models that have over 57% Accuracy. See if you can hit around the mid-70%.

From the feedback I've received, it would also be good to determine how much US **GDP** influences the above predictions or put it another way, how *sensitive* is ETF closing price and price movements to fluctuations in US GDP figures.

**Dashboards**

I'll need two versions of the Dashboards -- one for my **ETF investors and ETF trading desk** jockeys, the other for my **Economic Data & Financial Business Analyst** eggheads.

Sadly, they are familiar with two different Dashboard applications. On the ETF trader's side -- they are using **Microsoft Power BI**. However, my Business Analysts are more familiar with **Tableau**.

**In Power BI**

Just as a side-quest, our Trading Desk's Team-Lead is *Duncan*. He's a real 80's fan. Think the film: *Wall-Street* meets the series: *Miami Vice*! He's specifically requested a unique design for his Power BI -- based Dashboard. Please use LOTs of Neon-Esque colours for his dashboard but also make it versatile enough to show up to 6 ETF Ticker data at one time and he'll also need the whole range of dates mentioned above loaded into the application before we can move it to the testing phase.

**In Tableau**

You'll have more creative space here. However, the Dashboard for my Economists and Finance BAs must contain the following functionalities:

-         Linking both datasets -- please select by dates, choosing only to pull back matching rows.

-         Linking ETF Market data Graphs to Macroeconomic Indicator data Graphs -- my Tableau guru *Lisa* says there is a function in Tableau to help you with this. Essentially, you'll need to convert the graphs in both datasets to show percentage movements relative to a specific date (say starting range date of 1^st^ January 2020) this will ensure what you see on ETF data-driven graph is relatable to what you'd see on a Macroeconomic data-driven graph. I'll try to send you the way to do this, but I'll need to go back to her first to clarify.

-         You'll have to create an **"Overall"** dashboard, pitting 6 ETF Close Price averages against the overall  top 10 Macroeconomic influencers. This will be determined by the results of your ML ETF close price predictor model. For the sake of user customisation, please ensure that the graphs on this are 'hot-swappable' meaning someone on my team would be able to swap one macroeconomic graph for another in this dashboard.

-         My BAs also asks you to provide a **"Heatmap Wall"** Dashboard -- again this should be hot-swappable. But for the time being and for demo purposes I just need you to add 2 relevant {ETF heatmaps} and 4 \[Macroeconomic heatmaps\]. *Please use square and curly brackets to distinguish the datasets, as I've shown you above.*

-         Final request for dashboards (I promise) -- We have individual BAs who need to regularly check on the movements of two or three ETFs throughout the evening shift. Therefore, for these "ETF Night Watch" (or Watchers) we need individualised **"ETF Health Check"** Dashboards. These will have Average Close Price vs. Average Trade Volumes (focus these onto one graph if possible) -- pitted against the top 6 Macroeconomic factors that specific ETF Close Price is sensitive to the most. Maybe provide demos for 3 ETFs to begin with.

That's it from me. Well nearly. I've got one more challenge for you, as I know you love them!

**Additional Business Requirement (Optional): Running Multiple Predictive Models in Parallel**

For extra points, we'd be interested to know if it's possible to code something to accurately predict the *R-Squared* value for say up to 20 ETFs at the same time. From these, relating to the information above, we'll also need a set of top 10 Macroeconomic indicators that influence the specific ETF the most.

That's it from me for today, as I have a meeting with all the stakeholders in 5 minutes.

There's a lot of work ahead and I'll make sure we compensate you for your time and effort this time!

Hope to see you again soon, but if there's any questions on the above, please don't hesitate to contact me via voicemail or email and I'll get back to you ASAP.

Good luck with the above and with the rest of your course at **Code Institute** and thank you again for helping an old friend with this enormous undertaking!

Best regards,

Sarah Frugal