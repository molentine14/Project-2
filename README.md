# Project-2
### Core Hypothesis: If there were fed announcements related to COVID-19, intentions of actions by the Fed, or direct actions by the Fed then there will be correlated market movement in the stock market and bond markets

1) To test our hypothesis we scraped press releases straight from the Federal Reserve COVID page using BeautifulSoup python library. From the scrape we used a for loop to pull the text into a dataframe to utilize in the next steps. 

2) We will then use SpaCy to analyze the following sentiment catagories related to each topic:
    - COVID-19: Does the article mention positive or negative shifts in the pandemic
    - Intentions mentioned of Fed action: Does the Fed indicate additional action or continued action is likely or unlikely
    - Direct or planned action by Fed is mentioned: Does the Fed indicate they have acted or plan to act

3) Based on our findings of the article each sentiment category will be paired with a weighted impact on the stock and bonds markets, respectively.

4) Option 1: The next piece of our project is to create a trading algorithm that will incorporate and form trading signals based on sentiment
Option 2: The next piece of our project is to create a trading algorithm that will incorporate and adjust bollinger bands based on news sentiment for the day. Increasing standard deviation for high volatile trading days.

5) Trading algorithm with appropriate weights will then be back tested to the estimated beginning of COVID-19 pandemic coverage.

6) Standard portfolio analysis will be used to measure the trading algorithm's ability to perform in historical data. Metrics included will be:
    - Profit/Loss
    - Sharpe Ratio
    - Standard Deviation, Alpha, Beta
Will include charts and tables to lay out the analysis/metrics

7) Draw Conclusions about the model and configure scraper and trading algorithm for live use

8) Run the algorithm with live market data and have weights adjust for live reads on article sentiment
