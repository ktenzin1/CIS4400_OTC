# CIS4400_OTC
Technical Analysis of the OTC Market and Applying Knowledge and Skills learnt from Professor Jefferson in CIS 4400 to do a real-world project

1)	Business Problem
   
I. Brief Description of the OTC Markets Group: 
The Over-the-counter (OTC) market is a market to connect investors with companies to trade securities that are not listed on major exchange venues like the New York Stock Exchange or the NASDAQ. About 12000 U.S and global securities are traded on the OTC market. The OTC website states, "We enable investors to easily trade through the broker of their choice and empower companies to improve the quality of information available for their investors". 

According to the OTC website, securities from the following industries are traded on the OTC market "financial services, metals & mining, oil & gas, pharmaceuticals & biotechnology, healthcare, telecommunications, technology, retail, media, utilities, and many more".

The total annual dollar volume was $507 billion as of December 31, 2022.

II. Give the requirements and any missing requirements you have found
1. Breakdown per year, quarter, month, 
2. Breakdown by sector, by security type
3. You are required to do Technical Analysis (Use the following library https://github.com/bukosabino/ta)
4. On the dashboard, for each security, I need to see technical indicators.

1.  Breakdown per Year, Quarter, Month:  
- This involves examining market data over different periods to identify trends and patterns. A  yearly analysis might show long-term market trends, while a quarterly and monthly analysis can reveal shorter-term fluctuations and seasonal effects. 

2.  Breakdown by Country, Sector:  
-  Sector analysis: Different sectors respond differently to economic cycles. For example, technology stocks might behave differently than energy stocks. 

3.  Breakdown by Security Type:  
- OTC markets can trade a variety of financial instruments, such as equities (stocks)  that are not listed on a central exchange,  bonds  (debt securities), and derivatives  (which derive their value from an underlying asset). 

4.  Technical Analysis Indicators:

-  Ichimoku Cloud: This provides information on future price movements and potential support/resistance levels. It's a comprehensive indicator that defines support/resistance, identifies trend direction, gauges momentum, and provides trading signals.

-  Rate of Change: This is a pure momentum oscillator that measures the percent change in price from one period to the next. In general, prices are rising as long as the ROC remains positive. Conversely, prices are falling when the ROC is negative.

-  Supertrend: The SuperTrend indicator is a popular technical analysis tool used by traders and investors to identify the direction of a trend and potential entry and exit points in the financial markets.

-  Simple Moving Average: The Simple Moving Average (SMA) is a widely used technical analysis tool that helps traders and investors smooth out price data to identify trends over a specified period of time. 

-  Momentum Indicators: These are tools used to identify the speed of price movement or the velocity of price changes, like the Moving Average Convergence Divergence (MACD). 

-  Money Flow Index (MFI): This is a momentum indicator that uses both price and volume to measure buying and selling pressure. It’s also known as the volume-weighted RSI. 

-  Relative Strength Index (RSI): This measures the speed and change of price movements. RSI oscillates between zero and 100. Traditionally, an RSI above 70 is considered overbought, and an RSI below 30 is considered oversold.

-  Stochastic Oscillator: This momentum indicator compares a particular closing price of a security to a range of its prices over a certain period of time. The sensitivity of the oscillator to market movements is reducible by adjusting that time period or by taking a moving average of the result. 
 
2)	Business Impact

Risks:
 
- Market Risk: The potential for losses due to adverse movements in market prices, including factors such as volatility, economic events, and changes in investor sentiment.

- Credit Risk: The risk of financial loss arising from the failure of a counterparty to fulfill its contractual obligations, such as defaulting on a loan or failing to make a payment in a derivative transaction.

- Liquidity Risk: The risk of being unable to execute trades or liquidate positions in a timely manner without causing significant price movements, particularly in markets with low trading volumes or limited market depth.

- Operational Risk: The risk of losses resulting from inadequate or failed internal processes, systems, or human error, including issues related to data management, technology failures, or regulatory compliance.

- Counterparty Risk: The risk that the other party in a financial transaction will not fulfill its obligations, such as delivering securities or making payments, leading to financial losses or disruptions in trading activities

 Benefits:

 - Market Understanding: Analyzing OTC data can provide a deeper understanding of market dynamics, including trading volume, price movements, and liquidity. This understanding can help the persona or company make more informed trading decisions.

 - Risk Management: By analyzing OTC data, the persona or company can identify potential risks, such as volatility or counterparty risk, and take appropriate measures to mitigate them. This could include diversifying portfolios, setting stop-loss levels, or hedging strategies.

 - Identifying Opportunities: OTC data analysis can uncover trading opportunities that may not be apparent from traditional market data sources. This could include identifying undervalued assets, detecting patterns or trends, or spotting arbitrage opportunities.

 - Customized Trading Strategies: Analyzing OTC data allows for the development of customized trading strategies tailored to the persona's or company's specific needs and risk tolerance. This could involve algorithmic trading, quantitative analysis, or other advanced trading techniques.

 
3)	Business Persona 
 
- Technical Analysts​

- Stakeholders ​

- Investors​

- Companies involved in OTC trading ​

- Financial Analysts 

4)	Data
The data sources that you are going to use and the metadata associated with them. 
- OTC Data and data dictionary provided by Professor Jefferson
- The data set is about 1.5 GB. 

Strengths: Historic, Granularity and Diverse ​

Weakness: Data availability, large dataset

5)	Methods
In this section, we will highlight some of the key tools and elements of our tech stack that we will be using for this project. As we learn and build upon our skills during this program, we hope to add additional tools to this section and improve upon some of our initial assumptions.

- Utilized Google Collab as a code editor​

- GitHub to store and organize all our deliverables (Version Control)​

- Visual Studio Code as a code editor and to support GitHub ​

- Python Script to ingest data into Azure Blob​

- DbSchema for Dimensional Modeling for schema

- Python Script for ETL

6)	Data Tools 
Data Storage: Microsoft Azure Blob for cloud storage (containers)

 
Data Processing: 
- First we set up the adaptor in Google Colab. Next, we created a container named otcgroup6 in Azure Blob. Then we copied the connection string from the access keys in Azure to the Google Colab workstation. Those three are needed for the data ingestion.
- We then uploaded the downloaded zip data file to Google Drive to make ingestion into Azure easier.
Using the python script, the zip file from Google Drive was successfully uploaded into Azure Blob.  
 
Data Orchestration: 
- Using python script, extracted the uploaded data in Azure Blob and made a copy of the data frame (extraction)​

- Performed data cleaning and transformation (transformation)​ using hand coded python script

- Loaded the cleaned data into BigQuery using the python script

- Created a csv file of the cleaned dataset
 
7)	Interface
Tableau Public was used for data visualization to study the following technical indicators: Ichimoku Cloud, Rate of Change, Supertrend, Simple Moving Average, Momentum Indicators, Money Flow Index (MFI), Relative Strength Index (RSI), and Stochastic Oscillator. 

Link for Tableau Public dashboards:
https://public.tableau.com/app/profile/karma.yangchen.tenzin/viz/IchihimokuCloud/Dashboard1
https://public.tableau.com/views/roc_17152893719480/Dashboard1?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link
https://public.tableau.com/app/profile/fatima.tariq6857/viz/OTCIndicators/Dashboard1



