# US-Home-Price-Prediction

Welcome to the "US Home Price Prediction & Trends Analysis" project repository! In this project, we embark on a data-driven journey to understand the key factors influencing home prices in the United States of America over the past twenty years. Our goal is to build a comprehensive model that sheds light on the intricate relationships between various factors and home prices by leveraging publicly available data and advanced data science techniques. 

## Libraries and Tools used:

1. Programming Languages: Python
2. Data Analysis Libraries: NumPy, pandas, matplotlib, seaborn
3. Machine Learning Libraries: scikit-learn
4. Data Visualization: Matplotlib, Seaborn
5. Version Control: Git, GitHub
6. Colab Notebooks for data exploration and analysis

## Data Collection Sources:

1. Target (S&P/Case-Shiller U.S. National Home Price Index.) https://fred.stlouisfed.org/series/CSUSHPINSA
2. Population (Population includes resident population plus armed forces overseas.  The monthly estimate is the average of estimates for the first of the month and the first of the following month.) https://fred.stlouisfed.org/series/POPTHM
3. Personal Income (It is the income that persons receive in return for their provision of labor, land, and capital used in current production and the net current transfer payments that they receive from business and from government.) https://fred.stlouisfed.org/series/PI
4. Gross Domestic Product (Featured measure of U.S. output, is the market value of the goods and services produced by labor and property located in the United States.) https://fred.stlouisfed.org/series/GDP
5. Unemployment Rate (The unemployment rate represents the number of unemployed as a percentage of the labor force. (16 years age or above)) https://fred.stlouisfed.org/series/UNRATE
6. Mortgage Rate (A mortgage rate is the interest rate charged for a home loan.(Percentage)) https://fred.stlouisfed.org/series/MORTGAGE30US
7. Employment-Population Ratio: (It is a macroeconomic statistic that measures the civilian labor force currently employed against the totalworking-age populationof a region, municipality, or country. (emratio)) https://fred.stlouisfed.org/series/EMRATIO https://www.investopedia.com/terms/e/employment_to_population_ratio.asp
8. Building Construction issued permit in US (Total Units) https://fred.stlouisfed.org/series/PERMIT
9. Labor Force Participation Rate (The participation rate is the percentage of the population that is either working or actively looking for work.) https://fred.stlouisfed.org/series/CIVPART https://www.investopedia.com/terms/p/participationrate.asp
10. Monthly Supply of New Houses in the United States (The monthly supply is the ratio of new houses for sale to new houses sold.) https://fred.stlouisfed.org/series/MSACSR
11. Housing starts (New Housing Project) (This is a measure of the number of units of new housing projects started in a given period.) https://fred.stlouisfed.org/series/HOUST
12. Median Sales Price. (Median Sales Price of Houses Sold for the United States.(US Dollers)) https://fred.stlouisfed.org/series/MSPUS
13. Producer Price Index -Cement Manufacturing https://fred.stlouisfed.org/series/PCU327310327310
14. Producer Price Index by Industry: Concrete Block and Brick Manufacturing https://fred.stlouisfed.org/series/PCU32733132733106
15. All Employees, Residential Building Construction (Thousands of Peoples) (Construction employees in the construction sector include: Working supervisors, qualified craft workers, mechanics, apprentices, helpers, laborers, and so forth, engaged in new work, alterations, demolition, repair, maintenance etc.) https://fred.stlouisfed.org/series/CES2023610001
16. All Employees, Construction (Thousands of persons) (Construction employees in the construction sector include: Working supervisors, qualified craft workers, mechanics, apprentices, helpers, laborers, and so forth, engaged in new work, alterations, demolition, repair, maintenance.) https://fred.stlouisfed.org/series/USCONS
17. Industrial Production: Cement (The industrial production (IP) index measures the real output of all relevant establishments located in the United States) https://fred.stlouisfed.org/series/IPN32731S https://www.investopedia.com/terms/i/ipi.asp
18. Homeownership Rate (Percentage) (The homeownership rate is the proportion of households that is owner-occupied.)
https://fred.stlouisfed.org/series/RSAHORUSQ156S
19. Personal Saving Rate (Percent) (Personal saving as a percentage of disposable personal income (DPI), frequently referred to as "the personal saving rate," is calculated as the ratio of personal saving to DPI. Personal income that is used either to provide funds to capital markets or to invest in real assets such as residences.)
https://fred.stlouisfed.org/series/PSAVERT
20. New Privately-Owned Housing Units Completed: (Total units in thousands) https://fred.stlouisfed.org/series/COMPUTSA
21. New Privately-Owned Housing Units Under Construction: (Total Units in thousands) 
https://fred.stlouisfed.org/series/UNDCONTSA
