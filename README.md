# deep-learning-challenge
UCB Data Analysis Bootcamp Module 21 Deep Learning Challenge

## Installation

Google Colab is used to complete this challenge.


## Overview

This is the Module 21 challenge for the UC Berkeley Data Analyticd Boot Camp. In this challenge, the non-profit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. We are building a machine learning model that will use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

The Alphabet Soup's business team provided a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organizations, including:
  * EIN and NAME -- identification columns
  * APPLICATION_TYPE -- Alphabet Soup application type
  * AFFILIATION -- Affiliated sector of inductry
  * CLASSIFICATION -- Government organization classification
  * USE_CASE -- Use case for funding
  * ORGANIZATION -- Organization type
  * STATUS -- Active Status
  * INCOME_AMT -- Income classification
  * SPECIAL_CONSIDERATIONS -- Special considerations for application
  * ASK_AMT -- Funding amont requested
  * IS_SUCCESSFUL -- Was the money used effectively

## Results
### Data Processing
* The target variable is the IS_SUCCESSFUL column.
* Feature variables are the APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATION and ASK_AMT.
* Variables removed are the identification columns, that are EIN and NAME.

### Compiling, Training and Evaluating the Model
* Trained the model originally with 2 hidden layers, first layer with 80 neurons and second layer with 30 neurons, both layers have ReLU as the activation function. However, the model was unable to achieve the desired performance, so more neurons and/or hidden layers are added.
* The desired performance is an accuracy rate of 75% and higher, but unfortunately this model only reached 72.79% as its highest performance.
* Different methods are used in attempt to increase model performance:
  1. Increase the number of neurons
  2. Increase the number of hidden layers
  3. Use a different activation function
  4. All of item 1 to 3
  5. All of item 1 to 3, plus reducing the number of epoch
