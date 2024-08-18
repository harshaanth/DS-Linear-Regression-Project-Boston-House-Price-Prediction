# Linear Regression Project: Boston House Price Prediction

## Problem Statement

The problem at hand is to predict the housing prices of a town or suburb based on the features of the locality provided to us. In the process, we need to identify the most important features in the dataset. We need to employ techniques of data preprocessing and build a linear regression model that predicts the prices for us.

## Project Overview

This project is focused on predicting the median home value (`MEDV`) in the Boston area using a linear regression model. The dataset used for this analysis contains various attributes that describe different aspects of the localities in Boston, such as crime rates, the proportion of residential land, accessibility to highways, and others. The goal is to build a model that can accurately predict home prices based on these features.

## Data Information

Each record in the database describes a Boston suburb or town. The data was drawn from the Boston Standard Metropolitan Statistical Area (SMSA) in 1970. Below is the detailed attribute information:

- **CRIM**: Per capita crime rate by town.
- **ZN**: Proportion of residential land zoned for lots over 25,000 sq.ft.
- **INDUS**: Proportion of non-retail business acres per town.
- **CHAS**: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise).
- **NOX**: Nitric oxides concentration (parts per 10 million).
- **RM**: Average number of rooms per dwelling.
- **AGE**: Proportion of owner-occupied units built prior to 1940.
- **DIS**: Weighted distances to five Boston employment centres.
- **RAD**: Index of accessibility to radial highways.
- **TAX**: Full-value property-tax rate per $10,000.
- **PTRATIO**: Pupil-teacher ratio by town.
- **LSTAT**: Percentage of lower status of the population.
- **MEDV**: Median value of owner-occupied homes in $1000s (target variable).

### Observations:

- Half of the regions have per-capita crime rates between 0.08204 and 3.677082.
- Most regions do not have residential land zoned for lots over 12,500 sq. ft.
- Fifty percent of regions have between 5.2% and 18.1% of non-retail business acres per town.
- Fifty percent of regions have nitric oxide concentrations between 0.449 and 0.624 PPM.
- Fifty percent of regions have an average of 5.9 to 6.6 rooms per dwelling.
- In fifty percent of regions, between 45% and 94% of owner-occupied units were built prior to 1940.
- Fifty percent of regions are between 2.10 and 5.19 units of weighted distance to five Boston employment centers.
- In fifty percent of regions, the full-value property-tax rate per $10,000 is between $279.00 and $666.00.
- In fifty percent of regions, the pupil-teacher ratio is between 17.4 and 20.2.
- The distribution of the proportion of lower income population is very spread out. A typical region has about 11.3% lower status.
- Median value of owner-occupied homes ranges between $5,000 and $50,000, with half of the values concentrated between $17,000 and $25,000. A typical region has a home value of $21,200.

## Key Feature Interpretations

- **CRIM (-1.2455)**: For each unit increase in the per capita crime rate, the model predicts a 1.2% decrease in the median home value. This suggests that areas with higher crime rates are less desirable, leading to lower property values.

- **RM (5.932275)**: For each unit increase in the average number of rooms per dwelling, the model predicts a 5.9% increase in the median home value. This indicates that homes with more rooms are generally valued higher, reflecting the preference for spacious living environments.

## Conclusions

- **Lower Median Home Value**:
  - Regions with higher crime rates, greater accessibility to highways, higher full-value property tax rates, and a larger percentage of the population characterized as lower status tend to have lower median home values.
  
- **Higher Median Home Value**:
  - Median home values are higher in regions with more homes bordering the Charles River, higher nitrous oxide concentration, more rooms on average, farther distances from Boston employment centers, and a higher pupil-teacher ratio.

## Business Recommendations

- **Property Valuation**: The model can be effectively used to predict median home values based on the features included in this analysis. This can assist real estate investors, urban planners, and developers in assessing property values and making informed investment decisions.

- **Targeted Development**: Areas with higher crime rates or lower socioeconomic status should be targeted for development or revitalization to enhance property values. Improving safety, reducing pollution, and enhancing education infrastructure could positively impact housing prices in these regions.

- **Investment Strategy**: Investors looking for high-value properties might focus on areas with larger homes, proximity to the Charles River, and regions with a higher pupil-teacher ratio. These factors are positively correlated with higher median home values.

## Files in this Repository

- **Boston_house_price.ipynb**: Jupyter Notebook containing the full analysis, including data exploration, model building, and evaluation.
- **README.md**: This file, providing an overview of the project and repository structure.
