# BART
This is a project assigned to me during [theDevMasters](https://www.thedevmasters.com) bootcamp.<br> 
For more information, click [here](https://www.kaggle.com/saulfuh/bart-ridership).

## Introduction
[Bay Area Rapid Transit](https://www.bart.gov/)(BART) is a rapid transit public transportation system located in the San Francisco Bay Area. With so many people using BART trains to travel, the organization needs to properly account for the number of passengers travelling between two stations at any given time. Releasing such data to the public allows customers to plan accordingly.

## Objective
The objective of this project is broken down into two parts.
The first is to answer some critical questions:
1. Which BART station is the busiest?
2. What is the least popular BART route?
3. When is the best time to go to SF from Berkeley if you want to find a seat?
4. Which day of the week is the busiest?
5. How many people take the BART late at night?

The final objective of the project is to predict the number of people commuting to work by Bart between any 2 stations.

## Metric
The Root Mean Square Error (RMSE) was used as the evaluation metric for this project. The metric score indicates how different the predicted 
values are from the actual values. The lower the error the better the model is in predicting the target feature.

## Approach
The following steps were taken to complete the project:
1. Import libraries and datasets
2. Merge the 2016 and 2017 dataset
3. Create address, latitude, and longitude columns
4. Correct inconsistent values between the merged dataframe and the station dataframe
5. Merge the two dataframes
6. Check for null values
7. Wrangle the data to answer questions
8. Calculate the distance between each unique combination of two train stations
9. Normalize quantitative features
10. Create dummy variables for the categorical columns
11. Select best model

## Model Selection
The model was chosen based on the lowest RMSE score.<br>
The gradient boosting model was selected as the optimal model for this project.

<img width="502" alt="Screen Shot 2020-11-29 at 4 51 06 PM" src="https://user-images.githubusercontent.com/51253177/100558466-7326b600-3263-11eb-93c7-ae1bf00b1613.png">

## Technologies
Application: Jupyter Notebook<br>
Programming Language: Python 3.7.4<br>
Libraries: Numpy, Pandas, Scipy, Pyspark, Geopy, Re<br>

## Project Files
* [README](https://github.com/Ericjung008/BART/blob/main/README.md)
* [Project](https://github.com/Ericjung008/BART/blob/main/BART.ipynb)
* [2016 Dataset](https://www.kaggle.com/saulfuh/bart-ridership)
* [2017 Dataset](https://www.kaggle.com/saulfuh/bart-ridership)
* [Station Dataset](https://www.kaggle.com/saulfuh/bart-ridership)

## Acknowledgments
Data used to complete this project were recorded by the BART organization.
