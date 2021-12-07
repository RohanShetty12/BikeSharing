# Demand dynamics of Bike Sharing system
> This is a Linear regression Model Development project on the BikeSharing data.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Outcome of Model Development](#Outcome-of-model-development)
* [Recommendations](#Recommendations)


<!-- You can include any other section that is pertinent to your problem -->

## General Information
### Introduction
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free.
A US bike-sharing provider **BoomBikes** has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. Owing to such a harrowing situation, the company has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

### Problem Statement
BoomBikes wants to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:
- Which variables are significant in predicting the demand for shared bikes
- How well those variables describe the bike demands
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 

### Business Goal
We need to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 

### About the Dataset
The company has provided the booking data of their bikes on a daily basis for the year 2018 and 2019. The data is provided in the form of a CSV file (**day.csv**). The company has also provided the data dictionary for the variables which are part of the historical data (**Readme.txt**) 


## Technologies Used
- numpy - 1.16.2
- pandas - 0.24.2
- matplotlib - 3.0.3
- seaborn - 0.11.2
- statsmodels - 0.9.0
- scikit-learn - 0.20.3

## Outcome of Model Development
### Final Equation
The equation of the best fitted line is:
cnt = 0.192401 + 0.259882*yr + 0.437302*atemp - 0.170985*spring - 0.227425*Light

### Interpretation
- We see that for every 1 unit raise in year, cnt increases by 0.26 units while keeping the rest of the parameters constant.
- Similarly, for every 1 unit raise in atemp, cnt increases by 0.44 units while keeping the rest of the parameters constant.
- During the presence of spring, cnt decreases by 0.17 units while keeping the rest of the parameters constant.
- When the weather is slighlty rainy or snowy, cnt decreases by 0.17 units while keeping the rest of the parameters constant.


## Recommendations
After interpriting our linear regression equation, we see that there are 4 major factors that affect the rental count:
- **Temperature as felt by the customers**
- **Every passing year**
- **Season**
- **Weather situation**

Below are some of the recommendations after analyzing the linear regression model and the EDA:
- ***Temperature felt by the customers*** has a ***positive correlation*** with the sales of bike. Hence it would be beneficial to release some offers while the temperatures are low so that the customers are motivated to rent a bike.
- We see that with every ***passing year, the rental number increases***. Hence the sales are increasing on a yearly basis.
- We see that ***season*** has an impact on the bike sales. Specially, after analyzing the linear regression model and the EDA, we discovered that spring and winter season result in lower cusotmers renting bikes. The company needs to focus on this aspect.
- ***Weather situation*** also has a serious impact on the rentals. We see that while the weather is clear and sunny, cusotmers tend to rent more compared to on a gloomy, rainy or snowy day. Hence the company needs to attarct customers to use the bikes during such weather situations by either modifying the bikes to make the bikes more ridable during such unpleasent conditions.


## Contact
Created by [@RohanShetty12] - feel free to contact me!
