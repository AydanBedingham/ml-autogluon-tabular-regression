# AutoGluon Regression

## Overview
Uses Autogluon to build, train, and test a variety of machine learning models to predict the number of casual users from a bike rental usage dataset.

# Dataset

- Dataset File: bike_sharing_daily.csv
- Dataset Source: Hadi Fanaee-T, Laboratory of Artificial Intelligence and Decision Support (LIAAD), University of Porto INESC Porto, Campus da FEUP Rua Dr. Roberto Frias, 378 4200 - 465 Porto, Portugal

## Inputs
- instant: record index
- dteday: date
- season: season (1: springer, 2: summer, 3: fall, 4: winter)
- yr: year (0: 2011, 1: 2012)
- mnth: month ( 1 to 12)
- hr: hour (0 to 23)
- holiday: whether day is holiday or not - weekday : day of the week
- Working day: if day is neither weekend nor holiday is 1, otherwise is 0.
- weathersit:
  - 1: Clear Few clouds, Partly cloudy
  - 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
  - 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
  - 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
- temp : Normalized temperature in Celsius. The values are divided to 41 (max)
- windspeed: Normalized wind speed. The values are divided to 67 (max)

## Outputs
- casual: count of casual users


# Notebook
- Load the dataset and perform basic exploratory data analysis
- Split the data into training and testing sets
- Use AutoGluon to train linear regression models
- Evaluate performance of trained models