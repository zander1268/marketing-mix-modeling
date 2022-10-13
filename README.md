# Marketing Mix Modeling
**Author**: [Alex FitzGerald](https://www.linkedin.com/in/alex-fitzgerald-0734076a/)
![MMM header](Images/mmm_hero_image.png)

## Overview
Media Mix Modeling is an analysis technique to understand and quantify the impact that advertising has on its desired goal, typically sales of the product being promoted. This project focuses on media mix modeling with different linear regression techniques of varying complexities. This works builds off of the work done by [Dr. Robert Kübler](https://github.com/Garve?tab=repositories) adding additional analysis tools marketers to implement in real-world scenarios.

## Business Problem
It has been said that 50% of advertising spend is wasted, the trouble is knowing which half. Advertisers need to understand where to allocate their marketing budgets to maximize ROI (return on advertising spend). In a world with limited budgets and many available channels, wasting 50% of your investment simply isn't good enough. Smart media planning begins with an informed ROI prediction across your advertising channels. Media Mix Modeling uses the historical data from the advertiser to draw connections between spend (X) and sales (y). These connections not only help illuminate the ROI of past investments, they unlock the ability to optimize future media plans.

## Data
In the data set [available here](https://medium.com/r/?url=https%3A%2F%2Fgithub.com%2FGarve%2Fdatasets%2Fblob%2F4576d323bf2b66c906d5130d686245ad205505cf%2Fmmm.csv) we see historical investment in three advertising channels by week over the course of 200 weeks. These will be our features in the linear regression model.
1. TV
2. Radio
3. Online Banners

We also have a column representing our target variable, Product Sales.

## Methods
The projects lays out three linear regression models built with scikit-learn of varying complexities
1. Simple linear regression
2. Simple linear regression with manual adjustment
3. Advanced linear regression with feature engineering

Linear regression Media Mix Models are looking for two things…
1. The coefficients of this model tell us the degree to which adjusting spend on a given channel impacts sales.
2. Isolating the impact that one channel has on sales from a baseline of sales and other marketing allows us to find an ROI for the channel.

Simple linear regressions for MMM opperate on the assumption that the relationship between advertising spend and sales is linear, as ad spend increases, so does sales. More advanced MMMs account for the the practical implications of advertising spend that cause this assumption to break. The feature engineered versions of the models here account for the saturation and carry over effects of advertising. 

## Results
**Simple linear regression**: R2 0.71
