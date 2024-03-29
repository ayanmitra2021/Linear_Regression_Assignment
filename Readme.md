# Project Name
> Outline a brief description of your project.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- This project was about building linear regression models for a bike sharing company. There were ~14 independent variables given in a dataset for 2 years, where the objective is to determine the impact it has on the number of riders (the target variable). The idea is that the model(s) will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model(s) will be a good way for management to understand the demand dynamics of a new market. 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
We have performed the analysis using 18 different training models, of which we selected 3 best models.

- Model #8 - it uses the 'atemp','yr','workingday', and 'clear' feature variables to determine the target. This was arrived using the forward-pass technique where we kept adding a new feature variable on every iteration to get to an optimal model. We observed the Adjusted R-Squared on the training set is 72% and on test data it is 70%.
- Model #13 - it uses the 'yr', 'workingday', 'feb', 'mar', 'apr', 'may', 'jun', 'jul', 'aug', 'sep', 'oct', 'nov', 'misty', and 'snowy' feature variables to determine the target. This was arrived using the backward-pass technique where we started with all the feature variables and then on every iteration removed one feature variable at a time, to get to an optimal model. We observed the Adjusted R-Squared on the training set is 75% and on test data is 76%.
- Model #18 - it uses 'yr', 'windspeed', 'spring', 'fall', 'aug', 'sep', 'clear', and 'snowy' feature variables to determine the target. This was arrived using the RFE technique to get to an optimal model. We can see the Adjusted R-Squared on the training set is 75% and on test data is 71%.

Between all the above three modesl we can affirmatively say the Model #13 is the most suitable model. This is because we see a dip of ~2% with Model #8 and ~4% with Model #18 if compared between the output of train and test data. Hence we to summarize we can say ~76% of the bikers count depends on:
- whether the year is 2017 or 2018
- whether it is a working day or not
- whether the month is anything between 'feb', 'mar', 'apr', 'may', 'jun', 'jul', 'aug', 'sep', 'oct', 'nov'
- whether the climate is misty or snowy

## Technologies Used
- pandas
- numpy
- matplotlib.pyplot
- seaborn
- statsmodels
- sklearn

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- https://wikipedia.org
- https://stats.stackexchange.com/
- https://math.stackexchange.com/

## Contact
Created by [@ayanmitra2021] - feel free to contact me!