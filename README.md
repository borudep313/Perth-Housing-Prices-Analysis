# Perth Housing Prices Analysis

## Project Overview
This project analyses key drivers of residential house prices in Perth using a dataset of approximately 33,000 property transactions. The goal is to understand how structural, locational, and amenity-related features influence housing prices, and to assess how well these factors explain price variation.

## Dataset
Dataset Source: Downloaded from Kaggle, from: "https://www.kaggle.com/datasets/syuzai/perth-house-prices?resource=download"

The dataset includes property-level information such as:
- Sale price
- Number of bedrooms and bathrooms
- Land area and floor area
- Distance to the CBD
- Proximity and ranking of nearest schools
- Location coordinates and sale dates

## Methods
The analysis consists of:
- Exploratory data analysis (EDA) to understand price distributions and feature relationships
- Feature-level visual analysis (scatter plots, box plots)
- Correlation analysis to identify key associations
- Multivariate linear regression to quantify the combined effect of multiple predictors
- Residual diagnostics and multicollinearity checks (VIF)

## Key Findings
- Perth house prices are positively skewed, with most sales between $300k–$700k.
- Floor area and number of bathrooms are the strongest positive predictors of price.
- Distance to the CBD has a clear negative effect on prices.
- Land area has a relatively weak effect once extreme values are filtered.
- Bedrooms have a negative coefficient in a multivariate setting, reflecting trade-offs in space allocation.

## Model Performance
- Linear regression explains approximately 50% of price variation (R² ≈ 0.50).
- Prediction errors increase substantially for high-priced properties.
- Residual analysis indicates heteroscedasticity and missing nonlinear or location-based effects.

## Limitations
- Important predictors such as suburb, zoning, renovation quality, and views are omitted.
- Linear regression cannot fully capture nonlinear relationships in housing markets.
- Multicollinearity exists among size-related variables (bedrooms, bathrooms, floor area).
- Results are interpretive rather than predictive in nature.

## Future Improvements
- Include categorical variables (e.g. suburb or postcode encoding).
- Apply transformations to reduce skewness.
- Explore nonlinear or tree-based models for improved predictive performance.
