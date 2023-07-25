# airbnb-EU-trends

# Airbnb Analysis on EU Cities

This Jupyter Notebook analyzes Airbnb rental data for various European cities. The notebook explores the relationship between Airbnb prices, guest satisfaction, and other factors using linear regression and basic statistical techniques using pandas and numpy.


## Data Ingestion

The code reads the Airbnb rental data for 10x2 (WEs + weekdays) EU cities from CSV files in the 'data/' directory. It then concatenates and preprocesses the data to create the working 'df' DataFrame.

## EU Cities Airbnb Ranking: Travellers' Statistics

Calculate average and median rental prices per city and ranks the cities based on guest satisfaction scores. The results are displayed in tables and scatter plots.

## Data Quality: Basic Checks

Perform basic data quality checks, detecting NaNs, and potentially wrong/false values. It also calculates variance and skewness for each city and identifies outliers.

## Market Study: Satisfaction vs. Price, Distance, Cleanliness, and Attractivity

We explore correlations between guest satisfaction and price, distance, cleanliness, and attractiveness for different market segments.

## Airbnb Impact Analysis on EU Cities

Compare the Airbnb short-term rental prices with long-term rental prices for EU cities, showing the potentially massive impact of Airbnb on the resp. local rental markets.

## Linear Models' Fittings: From Global to Per-City

The code trains a variety of linear regression, including Ridge and Lasso models for the entire dataset and per city. It ranks cities based on price predictability (R-squared and RMSE).

## Feature Engineering: Log and Standard Scaling for Linear Regression

The code applies logarithmic transformations on distance-related features and standard scaling on numerical features attempting (in vain) to improve the models' performance.

## Feature Engineering: Clipping for Outlier Control

We visually analyze the impact of clipping outliers on model performance and then we optimally refit the linear regression model with optimal clipping to improve both R2 and RMSE.

## Conclusion

The notebook provides insights into the Airbnb rental market in EU cities, the impact on local rental prices, and the relationship between prices, guest satisfaction and various gentrification factors. We thus provide a preliminary baseline guidance for travellers, investors/developers, urban planners, EU & local tax authorities.

Note: Some parts of the code have been excluded from this summary for brevity.
