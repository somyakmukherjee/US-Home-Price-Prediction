# US-Home-Price-Prediction

![home-prices-are-rising-in-literally-every-major-housing-market-1200-x-630](https://github.com/somyakmukherjee/US-Home-Price-Prediction/assets/110627955/9096e2bc-ff8d-4ac0-90d6-2a5690510de7)


Welcome to the "US Home Price Prediction & Trends Analysis" project repository! In this project, we embark on a data-driven journey to understand the key factors influencing home prices in the United States of America over the past twenty years. Our goal is to build a comprehensive model that sheds light on the intricate relationships between various factors and home prices by leveraging publicly available data and advanced data science techniques. 

## **Project Scope:**
This project aims to build a data science model to predict U.S. home prices based on key economic factors over the last 20 years.

### **Steps**
1.Data Collection and Preparation:

*   Gather historical data for the specified features.
*   Clean and preprocess the data for analysis.

2. Exploratory Data Analysis (EDA):

*   Visualize relationships between features and CSUSHPISA.
*   Identify correlations and patterns.

3. Model Development:

*  Build predictive models using regression or machine learning algorithms.
*  Train and validate the models.

4. Model Evaluation:


*   Evaluate model performance using appropriate metrics.
*   Fine-tune models for better accuracy.

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
6. Employment-Population Ratio: (It is a macroeconomic statistic that measures the civilian labor force currently employed against the totalworking-age populationof a region, municipality, or country. (emratio)) https://fred.stlouisfed.org/series/EMRATIO https://www.investopedia.com/terms/e/employment_to_population_ratio.asp
7. Building Construction issued permit in US (Total Units) https://fred.stlouisfed.org/series/PERMIT
8. Labor Force Participation Rate (The participation rate is the percentage of the population that is either working or actively looking for work.) https://fred.stlouisfed.org/series/CIVPART https://www.investopedia.com/terms/p/participationrate.asp
9. Monthly Supply of New Houses in the United States (The monthly supply is the ratio of new houses for sale to new houses sold.) https://fred.stlouisfed.org/series/MSACSR
10. Housing starts (New Housing Project) (This is a measure of the number of units of new housing projects started in a given period.) https://fred.stlouisfed.org/series/HOUST
11. Median Sales Price. (Median Sales Price of Houses Sold for the United States.(US Dollers)) https://fred.stlouisfed.org/series/MSPUS
12. Producer Price Index -Cement Manufacturing https://fred.stlouisfed.org/series/PCU327310327310
13. Producer Price Index by Industry: Concrete Block and Brick Manufacturing https://fred.stlouisfed.org/series/PCU32733132733106
14. All Employees, Residential Building Construction (Thousands of Peoples) (Construction employees in the construction sector include: Working supervisors, qualified craft workers, mechanics, apprentices, helpers, laborers, and so forth, engaged in new work, alterations, demolition, repair, maintenance etc.) https://fred.stlouisfed.org/series/CES2023610001
15. All Employees, Construction (Thousands of persons) (Construction employees in the construction sector include: Working supervisors, qualified craft workers, mechanics, apprentices, helpers, laborers, and so forth, engaged in new work, alterations, demolition, repair, maintenance.) https://fred.stlouisfed.org/series/USCONS
16. Industrial Production: Cement (The industrial production (IP) index measures the real output of all relevant establishments located in the United States) https://fred.stlouisfed.org/series/IPN32731S https://www.investopedia.com/terms/i/ipi.asp
17. Homeownership Rate (Percentage) (The homeownership rate is the proportion of households that is owner-occupied.)
https://fred.stlouisfed.org/series/RSAHORUSQ156S
18. Personal Saving Rate (Percent) (Personal saving as a percentage of disposable personal income (DPI), frequently referred to as "the personal saving rate," is calculated as the ratio of personal saving to DPI. Personal income that is used either to provide funds to capital markets or to invest in real assets such as residences.)
https://fred.stlouisfed.org/series/PSAVERT
19. New Privately-Owned Housing Units Completed: (Total units in thousands) https://fred.stlouisfed.org/series/COMPUTSA
20. New Privately-Owned Housing Units Under Construction: (Total Units in thousands) 
https://fred.stlouisfed.org/series/UNDCONTSA

## Feature Selection

In our analysis, we identified several key features and their correlations with the target variable, represented by the S&P Case-Shiller Home Price Index.

| Feature                | Correlation with Home Price Index |
|------------------------|----------------------------- -----|
| MSPUS                  | 0.976881                          |
| PPI_Cement             | 0.955342                          |
| GDP                    | 0.952614                          |
| income                 | 0.946638                          |
| PPI_Concrete           | 0.929656                          |
| population             | 0.895138                          |
| total_emp_cons         | 0.779245                          |
| new_private_hw_under   | 0.662241                          |
| all_Const_Emp          | 0.569529                          |
| home_ow_rate           | 0.112943                          |
| monthly_supply         | 0.213615                          |
| permit                 | 0.162787                          |
| house_st               | 0.038691                          |
| new_private_house      | -0.019483                         |
| unemployed_rate        | -0.230195                         |
| IPI_Cement             | -0.242221                         |  
| p_saving_rate          | -0.237831                         |
| emp_pop_ratio          | -0.546168                         |
| mortgage_rate          | -0.730709                         |
| labor_percent          | -0.798830                         |

The positive correlation values indicate a direct relationship with home prices, while negative values suggest an inverse relationship. Features with higher absolute correlation values have a larger impact on home prices.

## **Model Training**

LASSO regression, also known as L1 regularization, is a popular technique used in statistical modeling and machine learning to estimate the relationships between variables and make predictions. LASSO stands for Least Absolute Shrinkage and Selection Operator.

The primary goal of LASSO regression is to find a balance between model simplicity and accuracy. It uses L1 regularization technique,  it is used when we have more features(like our problem) because it automatically performs feature selection.

LASSO regression model uses shrinkage. Shrinkage is where data values are shrunk towards a central point as the mean. The lasso procedure encourages simple, sparse models (i.e. we have a large set of variables, but only a small number of them are truly important). This particular type of regression is well-suited for models showing high levels of multicollinearity or when you want to automate certain parts of model selection, like variable selection/parameter elimination.

The main advantage of a LASSO regression model is that it has the ability to set the coefficients for features it does not consider interesting to zero. This means that the model does some automatic feature selection to decide which features should and should not be included on its own. This is why we choose LASSO regression for our model training.

## **Data splitting and Scaling**

In this project, we employed the **Lasso regression** model due to indications of significant collinearity in the dataset. The Lasso regression model is known for its ability to handle collinearity by applying L1 regularization, which encourages sparsity in feature coefficients.

Optimal Alpha: 0.0100
Mean Squared Error (MSE): 21.25
RMSE: 4.609395
R-squared (R2): 0.99

Cross-Validation R-squared Scores: 
 [0.99540962 0.9930768  0.99603814 0.99374723 0.99470933 0.99493974
 0.99630378 0.99449389]

Mean R-squared: 0.9948
Standard Deviation of R-squared: 0.0010

## **Most Prominent features and least prominent features**

Lasso Regression is unique in that it not only regularizes the model but can also be used for feature selection. As it adds an L1 penalty term, it tends to drive the coefficients of some features to zero. This means that some features are effectively ignored in the final model, which simplifies it and reduces the risk of overfitting.

These coefficients represent the impact of each feature on the prediction of home prices. Positive coefficients indicate a direct relationship with home prices, while negative coefficients suggest an inverse relationship & zero coefficients indicates that they do not significantly impact the prediction of home prices. Here we can see PPI_cement have zero coefficient.

## **Conclusion:**

1. The points cluster closely around the diagonal reference line (the red dashed line), it suggests that the model's predictions closely match the observed values. This alignment indicates good performance.
2. The scatter plot shows a clear, linear relationship along the diagonal line, it indicates that the model captures the underlying patterns in the data well.
3. In data processing phase, deviations, outliers, or systematic patterns was carefully examined to understand areas for improvement in the model.
3. Mean R-squared is 0.9948 & Standard Deviation of R-squared is 0.0010.


