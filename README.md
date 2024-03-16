Instructions: STAT Assignment

Address any one of two problem statements or both!
Add the code on GITHUB as public & share the URL.


Options (insurance against movement in either direction) of these indices expire every week on a particular day. I.e. FINNIFTY options expire every Tuesday and NIFTY every Thursday, if expiry day is a holiday then a day prior to it.  
Check here ( https://live.markethound.in/history/decay ) historical straddle theta decay data of NSE and BSE indices i.e. NIFTY, SENSEX, FINNIFTY and BANKEX. 
Straddle price is a sum of CALL (upside movement insurance) and PUT (downside movement insurance) options. 
hi
List of expiries for index can be accessed via below API https://live.markethound.in/api/history/expiries?index=FINNIFTY 
Detailed movement data of each index and staddle price data on minute level granularity can be accessed via API https://live.markethound.in/api/history/decay?name=FINNIFTY&expiry=2024-03-05T00:00:00.000Z&dte=0
accessed Where dte is days to expiry and the list can be accessed here via below API, we are interested in all the data that is from 4dte to 0dte. Days to expiry is calculated as active trading days before expiry. Holidays are excluded. 
https://live.markethound.in/api/history/dtelist?index=FINNIFTY&expiry=2024-03-05T00:00:00.000Z



Given historical data, your assignment is to build a predictive model to predict Straddle Open, High, Low, Close data for the next day. I.e. Today is Modnay (11-03-2024) and NIFTY expiry is on Thursday(14-03-2024). Tuesday(12-03-2024) being 2dte, we want to predict Open, High, Low, Close of Straddle prices (Not the index).
Given index pairs SENSEX, NIFTY(NIFTY50) or FINNIFTY, BANKEX have similar constituents to some extent and hence movement is highly correlated, often during sudden movements insurance premiums (straddle prices) tend to spike to different extend, creating opportunities to take advantage as they stabilize. I.e. Check the image below. Your assignment is to 
Find correlation between pairs 
Create a model or method to quantify spike differentials 

