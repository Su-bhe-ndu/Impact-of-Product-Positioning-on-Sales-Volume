# Impact-of-Product-Positioning-on-Sales-Volume

## Table of Content
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning/Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)

### Project Overview
In today's competitive retail environment, understanding the factors influencing sales volume is crucial for maximizing revenue and ensuring business success. One such factor is product positioning within a store. This project aims to explore and quantify the effect of product positioning on sales volume. Using a dataset with variables such as product price, competitor's price, promotional activities, foot traffic, consumer demographics, product category, and seasonality, the project seeks to:

- Analyze patterns and relationships between product positioning and sales volume.
- Determine statistical significance of product positioning using ANOVA.
- Build a predictive model to forecast sales volume based on multiple factors.

### Data Sources
The dataset used for this project includes the following fields:

- Product ID: Unique identifier for products.
- Product Position: Location within the store (e.g., aisle, end-cap).
- Price: Selling price of the product.
- Competitor's Price: Price offered by competitors.
- Promotion: Indicator of promotional activities (e.g., discounts, buy-one-get-one).
- Foot Traffic: Customer count within the vicinity of the product.
- Consumer Demographics: Demographic details of customers (e.g., age, income level).
- Product Category: Type/category of the product.
- Seasonal: Seasonal indicators (e.g., holiday, off-season).
- Sales Volume: Number of units sold.

### Tools
- Programming Language: Python
- Libraries: pandas, NumPy, Matplotlib, Seaborn, scikit-learn, statsmodels
- Other Tools: Jupyter Notebook, VS Code

### Data Cleaning And Preparation
- Handling Missing Values: Missing data was imputed or removed to maintain data integrity.
- Formatting Issues: Ensured consistent data types for all columns (e.g., numerical and categorical fields).
- Outlier Detection: Used box plots and Z-scores to identify and handle outliers, particularly in sales volume and price-related columns.
- Feature Encoding: Encoded categorical variables (e.g., Product Category, Seasonal) using one-hot encoding for modeling.
- Data Splitting: Divided the data into training and testing sets for model evaluation.

### Exploratory Data Analysis
- Univariate Analysis: Examined the distribution of variables like price, sales volume, and foot traffic using histograms and box plots.
- Bivariate Analysis: Analyzed relationships between sales volume and key factors such as product position, price, and promotion using scatter plots and heatmaps.
- Seasonality Trends: Assessed the impact of seasonality on sales volume using time-series plots.
- Correlation Matrix: Identified correlations among variables to understand potential multicollinearity.

### Data Analysis
#### 1. Hypothesis Testing
- Conducted ANOVA (Analysis of Variance) to test if there are statistically significant differences in sales volume based on product positions (e.g., aisle vs. end-cap).
- Results showed no significant difference in sales volumes across positions (p-value > 0.05).
#### 2. Predictive Modeling
- Built a linear regression model to predict sales volume based on all input variables.
- Observed poor model performance (R²: -47.91), indicating that linear relationships were insufficient to explain the variance in sales volume.
- Identified the need for advanced modeling techniques, such as Random Forest or Gradient Boosting, and additional feature engineering.

### Results
#### 1. Insights from EDA:
- No significant patterns emerged between product positioning and sales volume.
- Factors like price, promotions, and seasonality showed weak correlations with sales volume.
#### 2. ANOVA Test Findings:
- Product positioning did not significantly impact sales volume, suggesting that other factors may play a more prominent role.
#### 3. Predictive Modeling Performance:
- Linear regression underperformed, with an R² score of -47.91, highlighting the need for further exploration of non-linear relationships and additional variables.

### Recommendations:
1. Explore Advanced Models: Use machine learning models like Random Forest or Gradient Boosting to capture non-linear relationships.
2. Feature Engineering: Consider creating interaction terms or aggregating data for better representation of trends.
3. Additional Data Collection: Gather more granular data on customer behavior, in-store movement, and promotional strategies.
4. Pilot Studies: Conduct real-world experiments with varying product positions to validate findings.

### Limitations:
1. Data Constraints: Limited granularity in the dataset may have restricted the analysis.
2. Model Performance: Poor predictive power of the initial model indicates the need for more robust algorithms.
3. Unaccounted Variables: Other factors, such as store layout or external market trends, may influence sales volume but were not captured.

### References
1. Scikit-learn Documentation
2. Pandas Documentation
3. Kaggle
