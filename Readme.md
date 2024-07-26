Welcome

The question had to find and explain how different factors have affected the housing prices in the US over the last 20 years,

The following steps were taken to achieve the desired answer:

1. Data was collected of the following metrics 
    a) Population growth (population.csv)
    b) Construction costs (producerPriceIndex.csv)
    c) Interest rate/federal funds (FEDFUND.csv)
    d) Inflation (consumerPrice.csv)
    e) Unemployment rate (UNRATE.csv)
    f) Gross domestic Product (GDP.csv)
    g) Housing supply (HOUST.csv)
    h) Median household income (medianIncome.csv)

2. The data was preprocessed to remove any empty or missing values as well as making sure that all the different sets of data share the same start and end date.

3. The datasets were merged into one single dataset for the runtime of the code and a correlation matrix was calculated. The heatmap represents values between +1 Perfect positive correlation (when one goes up, the other also goes up) and -1 Perfect negative correlation (when one goes up, the other goes down). This helps us see which economic factors are closely related to home prices and to each other.

4. Regression analysis was done to understand the relationship between one dependent variable (home prices) and multiple independent variables (economic factors). This was followed by an OLS model to find the best fitting line through the data. The regression gives us coefficients for each factor, showing how much the home price is expected to change when that factor changes by one unit. Positive coefficient indicates that the factor increases home prices and vice versa.

5. Scatterplots were plotted to show individual data points and help us visualize the relationship between each economic factor and home prices. Trend Line (Red Line) shows the general trend or direction of the relationship where the upward slope indicates a positive relationship (as the factor increases, home prices increase) while a downward slope indicates a negative relationship (as the factor increases, home prices decrease).

6. A feature importance graph was visualized to help us understand which economic factors have the most significant impact on home prices. The bars represent the coefficients from the regression model where a Positive Bar indicates that as the factor increases, home prices increase and a Negative Bar indicates that as the factor increases, home prices decrease. This plot helps us quickly see which factors are most important in predicting home prices.

7. A linear regression model was also trained on the data to test and predict the housing prices.

Putting together all the results and the information, the conclusion stands as follows:

From the data collected, it has been seen that only the unemployment rate has an inverse relation to the housing prices, while all other factors have a positive relationship with the housing prices. Lets try to explain these results:


1. Unemployment Rate
Inverse Relationship: The unemployment rate has a negative impact on housing prices.
Reason:
Reduced Income: Higher unemployment means more people are out of work, leading to lower household incomes.
Decreased Demand: With less income, fewer people can afford to buy homes, leading to reduced demand for housing.
Foreclosures: Higher unemployment can lead to more foreclosures, increasing the supply of houses on the market and further depressing prices.
2. GDP (Gross Domestic Product)
Positive Relationship: GDP has a positive impact on housing prices.
Reason:
Economic Growth: Higher GDP indicates a growing economy with more jobs and higher incomes, increasing the ability of people to buy homes.
Consumer Confidence: Strong economic performance boosts consumer confidence, encouraging more people to invest in real estate.
3. CPI (Consumer Price Index)
Positive Relationship: CPI has a positive impact on housing prices.
Reason:
Inflation: Higher CPI indicates higher inflation, which often leads to higher costs for construction materials and labor, increasing home prices.
Asset Protection: In times of high inflation, people may invest in real estate as a hedge against inflation, increasing demand and driving up prices.
4. Federal Funds Rate
Positive Relationship: The Federal Funds Rate has a positive impact on housing prices in the observed period.
Reason:
Economic Context: Although traditionally higher interest rates can reduce borrowing and lower housing demand, the context of the observed period may reflect times when the economy was strong enough to sustain housing demand despite higher rates.
Lag Effect: Changes in the Federal Funds Rate might take time to impact the housing market, and during periods of economic expansion, the positive impact on incomes and employment might outweigh the negative impact of higher borrowing costs.
5. Housing Starts
Positive Relationship: Housing Starts have a positive impact on housing prices.
Reason:
Economic Activity: More housing starts indicate a growing economy with increased construction activity, signaling strong demand for housing.
Supply and Demand Dynamics: While more housing starts increase supply, they also reflect confidence in the market and future demand, which can support higher prices.