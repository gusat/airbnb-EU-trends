# Airbnb-EU-Trends

## Project Overview
This project aims to analyze Airbnb rental data for various European cities to gain insights into the rental market, understand the impact of Airbnb on local rental prices, and explore the relationship between prices, guest satisfaction, and other factors.

## Installation
To run the Jupyter Notebook and interact with this project, you need to have Python installed together with the necessary libs.
Associated blog => https://medium.com/@mgusat/is-airbnb-really-pushing-us-out-3e18f59dc778

## File Descriptions
- `airbnb-EU-trends-v1x.ipynb`: Jupyter Notebook containing the analysis code.
- `data/`: Directory containing Airbnb rental data for European cities in CSV format.
- `Airbnb EU Blog.PDF`: Full (detailed) blog related to the associated Medium blog post.

## How to Interact with the Project
1. Clone or download the project repository.
2. Install Python and the required libraries.
3. Open the Jupyter Notebook `airbnb-EU-trends.ipynb`.
4. Run the cells in the Notebook sequentially.
5. The Notebook contains detailed explanations and comments; for details see the PDF blog.

## Licensing, Authors, and Acknowledgements
Mitch Gusat for Udacity P1 in T3; 
Under MIT License & Apache License 2.0


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
