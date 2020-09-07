# Case-Severity-Prediction-in-Emergency-Departments

In this project, I try to predict the urgency level of each patient once they arrive to the Emergency Room. It is trained on the National Hospital Ambulatory Medical Care Survey (NHAMCS). The NHAMCS contains data for patients from the US from 1999 to 2017. It has 949 different features.

## NHAMCS
Firstly, the dataset was cleaned: nans were removed and columns that could cause data leakage werte removed as well. Furthermore, many columns were representing the same information so all of them but one were removed.

## Model

4 Different versions are developed and they use both Logistic Regression and Support Vector Classifiers.
Essentially, the label is the 'IMMEDR' column and it has values between 1 and 5, where 1 is the most urgent and 5 is the least urgent.
I am training the model on the 2017 and the 2016 data only, due to the limited computational power available.

In order to select the features out of the 900 features, SelectKBest was utilized. To optimize all the paramters, a GridSearchCV was used.

## Results

The results of each of these models can be found in the 4 versions developed under the Model directory.

Authors: 
Ramez Moussa
Bassant Monuir
Hoda Amin
