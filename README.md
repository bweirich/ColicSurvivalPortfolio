# ColicSurvivalPortfolio
Colic Survival Portfolio (Python) This repository contains the python code for a colic Survival project. Further details of the project can be read in the notebook.

## Purpose 
Colic in horse is problem with the gastro-intestinal tract that causes abdominal pain. Colic can vary between mild cases to sever cases which can involve surgury. The cost of treatment can also vary greatly with the severity of the case.  

This analysis will predict the survival of a horse based on the features of the medical condition of a horse. The ability to predict a horses survival will allow owners and veterinarians to make better decisions regarding the best interest of the horse and the cost to the owner.

## EDA (Exploratory Data Analysis)

The feature variables distribution was examined and and the handling of null values was determined.  I created functions to assist with the visualization of numerical features and categorical features as well as functions to assist in the filling in of null values.  


The overall null values showed a distribution below:

![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/null_values.PNG)

#### Rectal Temp
![alt_text]()

As the mean of the rectal temp is very close with regards to all the outcomes possible and the distribution is normal we will be able to fill in the null values with the mean rectal temp.

#### Pulse
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/pulse.PNG)

As the distribution is skewed right and there are many outliers the median of each outcome is more accurate value to fill in the null values.

#### Respiratory Rate
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/respiratory_rate.PNG)

As the distribution is skewed right and there are many outliers the median of each outcome is more accurate value to fill in the null values.

#### Nasogastric Reflux PH
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/nasogastric_reflux.PNG)

As over 80% of the nasogastric_reflux_ph is null the better option is to remove the variable rather than fill in missing data.

#### Packed Cell Volumn
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/packed_cell_vol.PNG)

As the distribution is skewed right and there are many outliers the median of each outcome is more accurate value to fill in the null values.

#### Total Protein
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/total_protein.PNG)

As the majority of the values are concentration the mode is the best option to fill in the null values.

#### Abdominal Protein
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/abdomo_protien.PNG)

As the over 60% of the abdomo_protein is null the better option is to remove the variable rather than fill in missing data.

#### Lesions
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/lesions.PNG)

There are 3 different lesion feature variables.  As the values associated with the lesion variables are categorical rather then numerical the columns can be combined into one and the count of lesions can be recorded and used instead. 

#### Surgery
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/surgery.PNG)

#### Age
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/age.PNG)

#### Temperature of Extremities
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/temp_extremities.PNG)

The mode of each outcome is the best option to fill in the null values.

#### Mucous Membrane
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/mucous_membrane.PNG)

The mode of each outcome is the best option to fill in the null values.

#### Capillary Refill Time
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/capillary.PNG)

The mode of each outcome is the best option to fill in the null values.

#### Pain
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/pain.PNG)

The mode of each outcome is the best option to fill in the null values.

#### Peristalsis
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/peristalsis.PNG)

The mode of each outcome is the best option to fill in the null values.

#### Abdominal Distention
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/abdomo_distention.PNG)

The mode of each outcome is the best option to fill in the null values.

#### Nasogastric Tube
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/nasogastric.PNG)

The null values will be replaced with the mode of the dataset as it is by far the most common and is for all outcomes.

#### Nasogastric Reflux
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/nasogastric_reflux.PNG)

The null values will be replaced with the mode of the dataset as it is by far the most common and is for all outcomes.

#### Rectal Exam Feces
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/rectal_exam.PNG)

The mode of each outcome is the best option to fill in the null values.

#### Abdomen
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/abdomon.PNG)

The null values will be replaced with the mode of the dataset as it is by far the most common and is for all outcomes.

#### Abdomen Appearance
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/abdomo_app.PNG)

As over 50% of the values are null this variable will be dropped from the dataset.

#### Surgical Lesion
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/surgical_lesion.PNG)

#### CP Data
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/cp_data.PNG)

## Encoding

Pandas get_dummies was used to encode the categorical features in the dataset.

## Machine Learning Models

We have chosen Logistic Regression, DecisionTree, RandomForest and KNeighborsClassifier to predict the outcomes. I will use the Classification Report to gauge the effectiveness of the different models to select the best option.

#### Logistic Regression
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/lr_class.PNG)

#### DecisionTree
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/decision_class.PNG)

#### RandomForest
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/rf_class.PNG)

#### KNeighbors
![alt_text](https://raw.githubusercontent.com/bweirich/ColicSurvivalPortfolio/master/images/kn_class.PNG)

## Select best model  
Based on the Classification Report measurements of f1-score and accuracy the Logistic Regression is the best model for prediction.  

## Conclusion 
Since the training dataset is fairly small I would recommend that more data is collected for the models to train on before the model is deployed for real world use in predictions.
