# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis is to use the features in the Alphabet Set Charity dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing
- What variable(s) are considered the target(s) for your model?
The "IS_SUCCESSFUL" variable is considered the target variable.

- What variable(s) are considered to be the features for your model?
The "STATUS", "ASK_AMT", "APPLICATION_TYPE", "INCOME_AMT", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION" and "SPECIAL_CONSIDERATIONS" are the feature variables.

- What variable(s) are neither targets nor features, and should be removed from the input data?
The "EIN" and "NAME" variables are neither targets nor features and were therefore removed from the input data.

### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
Since the number of inputs was 43, I used the rule of thumb to have two to three times the amount of neurons in the hidden layer, and therefore chose 80. For the hidden layers, I decreased the number to 50 neurons then another half for my third hidden layer.
I used the relu activation function for the input and hidden layers to identify nonlinear characteristics from the input values.
For the output layer, I used the sigmoid activation function to help us predict the probability that applicants will be successful if funded.

- Were you able to achieve the target model performance?
I was not able to achieve the target model performance over 75%.

- What steps did you take to try and increase model performance?
I increased the number of neurons in my second hidden layer, added another hidden layer with half the neurons as the second hidden layer, and decreased my epochs from 100 to 50. 

## Summary
Even with different iterations of adjusting the neural network model, the model accuracy was still below the target model performance. I would try to use the RandomForest classifier since it is quicker to implement and is a great alternative for classification solving. 
