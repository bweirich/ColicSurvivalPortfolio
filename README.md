# ColicSurvivalPortfolio
Colic Survival Portfolio (Python) This repository contains the python code for a colic Survival project. Further details of the project can be read in the notebook.

## Purpose 
Colic in horse is problem with the gastro-intestinal tract that causes abdominal pain. Colic can vary between mild cases to sever cases which can involve surgury. The cost of treatment can also vary greatly with the severity of the case.  

This analysis will predict the survival of a horse based on the features of the medical condition of a horse. The ability to predict a horses survival will allow owners and veterinarians to make better decisions regarding the best interest of the horse and the cost to the owner.

## EDA (Exploratory Data Analysis)

The feature variables distribution was examined and and the handling of null values was determined.  I created functions to assist with the visualization of numerical features and categorical features as well as functions to assist in the filling in of null values.  


The overall null values showed a distribution below:

![alt_text]()

#### Rectal Temp
![alt_text]()

As the mean of the rectal temp is very close with regards to all the outcomes possible and the distribution is normal we will be able to fill in the null values with the mean rectal temp.

#### Pulse
![alt_text]()

As the distribution is skewed right and there are many outliers the median of each outcome is more accurate value to fill in the null values.

#### Respiratory Rate
![alt_text]()

As the distribution is skewed right and there are many outliers the median of each outcome is more accurate value to fill in the null values.

#### Nasogastric Reflux PH
![alt_text]()

As over 80% of the nasogastric_reflux_ph is null the better option is to remove the variable rather than fill in missing data.

#### Packed Cell Volumn
![alt_text]()

As the distribution is skewed right and there are many outliers the median of each outcome is more accurate value to fill in the null values.

#### Total Protein
![alt_text]()

As the majority of the values are concentration the mode is the best option to fill in the null values.

#### Abdominal Protein
![alt_text]()

As the over 60% of the abdomo_protein is null the better option is to remove the variable rather than fill in missing data.

#### Lesions
![alt_text]()

There are 3 different lesion feature variables.  As the values associated with the lesion variables are categorical rather then numerical the columns can be combined into one and the count of lesions can be recorded and used instead. 

#### Surgery
![alt_text]()

#### Age
![alt_text]()

#### Temperature of Extremities
![alt_text]()

The mode of each outcome is the best option to fill in the null values.

#### Mucous Membrane
![alt_text]()

The mode of each outcome is the best option to fill in the null values.

#### Capillary Refill Time
![alt_text]()

The mode of each outcome is the best option to fill in the null values.

#### Pain
![alt_text]()

The mode of each outcome is the best option to fill in the null values.

#### Peristalsis
![alt_text]()

The mode of each outcome is the best option to fill in the null values.

#### Abdominal Distention
![alt_text]()

The mode of each outcome is the best option to fill in the null values.

#### Nasogastric Tube
![alt_text]()

The null values will be replaced with the mode of the dataset as it is by far the most common and is for all outcomes.

#### Nasogastric Reflux
![alt_text]()

The null values will be replaced with the mode of the dataset as it is by far the most common and is for all outcomes.

#### Rectal Exam Feces
![alt_text]()

The mode of each outcome is the best option to fill in the null values.

#### Abdomen
![alt_text]()

The null values will be replaced with the mode of the dataset as it is by far the most common and is for all outcomes.

#### Abdomen Appearance
![alt_text]()

As over 50% of the values are null this variable will be dropped from the dataset.

#### Surgical Lesion
![alt_text]()

#### CP Data
![alt_text]()

## Encoding

Pandas get_dummies was used to encode the categorical features in the dataset.

## Machine Learning Models

We have chosen Logistic Regression, DecisionTree, RandomForest and KNeighborsClassifier to predict the outcomes. I will use the Classification Report to gauge the effectiveness of the different models to select the best option.

#### Logistic Regression
![alt_text]()

#### DecisionTree
![alt_text]()

#### RandomForest
![alt_text]()

#### KNeighbors
![alt_text]()

## Select best model  
Based on the Classification Report measurements of f1-score and accuracy the Logistic Regression is the best model for prediction.  The features that have the most importance on the models prediction are:

![alt_text]()

## Conclusion 
Since the training dataset is fairly small I would recommend that more data is collected for the models to train on before the model is deployed for real world use in predictions.
