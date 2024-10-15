

## Overview of the Analysis


*The goal of this analysis is to build a binary classifier that predicts whether an applicant will be successful if funded by Alphabet Soup. The dataset provided by Alphabet Soup contains metadata about more than 34,000 organizations, with features related to their industry affiliation, classification, use case for funding, organization type, and more. By leveraging these features, we aim to build a deep learning model to assist Alphabet Soup in selecting the most promising applicants for funding.


RESULTS

To start the data processing, we eliminated irrelevant details. 
We removed the EIN and NAME columns to focus on the columns that would serve as features for the model. 
However, NAME was reintroduced during a second test to assist with binning. 
We subsequently divided the dataset into training and testing sets. 
The target variable, named "IS_SUCCESSFUL," was used in the model to indicate a successful outcome, represented as 1 for yes and 0 for no. 
We reviewed the APPLICATION data, and utilized the "CLASSIFICATION" column for binning purposes. 
Several data points were designated as thresholds to group infrequent values under a new category, "Other," for each unique value. 
Once binning was verified to be effective, categorical variables were transformed using the get_dummies() function to encode them.


Compiling, Training, and Evaluating the Model:
There were three layers in total for each model after applying Neural Networks. 
The number of hidden nodes were dictated by the number of features.

