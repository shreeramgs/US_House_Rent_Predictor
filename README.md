# US Rent Price Prediction 

The goal of the project is to analyze the rental postings across the United States and provide actionable insights to the users in form of graphs and intuitive user interface.

## Problem Statement 

Although supply and demand is one of the major factors that can influence rental prices, several factors such as Parking, Location, Housing type and pets allowed etc., can influence fluctuations which in turn changes the rent prices. This project is done in order to help us better understand such anomalies, and how these change over the time with respect to the given demographics. With the aid of this project we get a glimpse of at least some factors that influence the collective change in rent price, and help us understand the need of how to use these findings to make better decisions in future to invest or to rent houses.

## Data 

The dataset for this analysis is available in Kaggle. (https://www.kaggle.com/austinreese/usa-housing-listings) It comprises information collected from various listings on Craigslist. It contains 22 attributes and over 300k listings.

## Screenshots 

Streamlit App

![alt text](https://github.com/Nirmalyan/us_rent_price_prediction/blob/main/screenshots/user-interface.png?raw=True)

Feature Importance

![alt text](https://github.com/Nirmalyan/us_rent_price_prediction/blob/main/screenshots/feature_importance.png?raw=True)

## Inferences: 

* The decision tree regression model performed better than the gradient boosting regression and linear regression models in terms of "Root Mean Squared Error" and "Adjusted R2". This metric is choosen for evaluation as the target variable is continuous and goal of the project is to predict the price range of the house given its property.  

* Certain features like sqfeet, number of beds, baths have significant influence in deciding the rental price of the house. We could also see some the names of the states like California, Masachussets and Hawaii which implies the rental price of houses are greatly affected by these places. 

## Installation

This project requires Python 3.7+. Install the packages from requirements.txt

```sh
pip install -r requirements.txt
```

## Folder and File Structure

 - database folder contains the sqlite database with normalized tables
 - load_data.ipynb contains code to read the csv file, normalize the data to remove redundancy and insert it into a sqlite database. 
 - eda.ipynb contains code for the analysis of rental listings and deriving insights
 - model.ipynb contains code that applies Machine Learning algorithms to the data to predict the rental price of the house 
 - app.py contains code that runs the streamlit web server where the users provide their input to get estimated rental price. 

## Future Objectives 

* Deploy the Streamlit app 
* Build a better model and check into dimensionality reduction 

