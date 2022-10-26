# Neural_Network_Charity_Analysis

## Overview

Using machine learning and neural networks, a model was created to predict whether applicants will be
successful if funded by Alphabet Soup. A file containing thousands of lines of data was used to train 
the model, which can predict success 72.5% of the time.

## Results

### Data Preprocessing

The variable considered the target for the model is the "IS_SUCCESSFUL" column.

The variables that are used as features for the model are:
- STATUS
- ASK_AMT
- APPLICATION_TYPE
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION

The variables that did not add value to the model, and were dropped are:
- EIN
- NAME

### Compiling, Training, and Evaluating the Model

Model_Def

Three hidden layers were chosen for the model.
- Hidden Layer 1 had 80 neurons, and used the "relu" activation function.
- Hidden Layer 2 had 30 neurons, and used the "sigmoid" activation function.
- Hidden Layer 3 had 15 neurons, and used the "sigmoid" activation function.

The number of epochs was also changed to 50.

This combination of layers, neurons and epochs was chosen after numerous trial and error attempts 
to improve the accuracy to above 75%. Unfortunately, this model is only able to achieve 72.5% accuracy.

The attempts to improve the accuracy included changing the number of hidden layers, the number of
neurons, the activation function used, the number of epochs and the number of features included in 
the model.

## Summary

A neural network model consisting of three (3) hidden layers and 125 total neurons was used to predict whether an applicant
would be successful if they received funds from Alphabet Soup. The model used both the "relu" and "sigmoid" activation
functions. It ran through 50 epochs to predict that 72.5% of the applicants who receive funds from Alphabet Soup will be
successful.

I believe a different model, possibly a logistic regression model, could be used to predict the success of an applicant.
The data set does contain information on which applicants were actually successful after receiving funding. This means that
a supervised machine learning model can be used, i.e. logistic regression.
