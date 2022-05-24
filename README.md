# Forecasting_Net_Prophet

 In this analysis, I analyze website search traffic, daily revenue, and stock prices of Mercado Libre, to create a time series model with Prophet. I utilized basic pandas calculations to aid in my analysis, and hvplot was used for data visualization.

 ## Summary
 Based on the analysis, I was able to answer the following questions:

 1. Read the search data into a DataFrame, and then slice the data to just the month of May 2020. (During this month, MercadoLibre released its quarterly financial results.) Use hvPlot to visualize the results. Do any unusual patterns exist?
    - Yes, there appears to be a seasonal pattern.

2. Did the Google search traffic increase during the month that MercadoLibre released its financial results?
    - Yes. Compared to the overall monthly median valule, traffic appears to have increased by about 8.5% during the month that MercadoLibre released its financial results.

3. Does any day-of-week effect that you observe concentrate in just a few hours of that day?
    - Yes, it appears that traffic is heaviest between hours 20-23, and 0-2. This pattern is consistent over each day of the week.

4. Does the search traffic tend to increase during the winter holiday period (weeks 40 through 52)?
    - Yes. Based on the plot, the search traffic between weeks 40 through 52 declines initially, but sharply increases during the holiday period.

5. Market events emerged during the year of 2020 that many companies found difficult. But, after the initial shock to global financial markets, new customers and revenue increased for e-commerce platforms. Do both time series indicate a common trend that’s consistent with this narrative?
    - No. Although there are points in the "search trends" plot that correspond with the trends in the stock price plot, the search trends show a more seasonal pattern, not consistent with the overall movement of the stock trends.

6. Does a predictable relationship exist between the lagged search traffic and the stock volatility or between the lagged search traffic and the stock price returns?

    - There is very small negative correlation between Stock Volatility and Lagged Search Trends. There is also a very small correlation between Hourly Stock Return and Lagged Search Traffic. Based on these results, there does not appear to be a predictable relationship between lagged search traffic and stock price returns. However, we would have to analyze deeper in order to be sure that a relationship does or does not exist.