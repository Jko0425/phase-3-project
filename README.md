![H1N1 vaccine](https://github.com/Jko0425/phase-3-project/blob/main/Images/h1n1%20vaccine.webp)
# Predicting Flu Vaccination Rate

## Overview
In recent events, vaccines have been a controversial topic. From governmental conspiracies to distrust in the health system, the efficiency of vaccines are not enough to get people to medical clinics. It is safe to say that regardless of the research behind vaccines, other variables like doubt and education may impact the patient's decision in receiving the vaccine. We will create several models that will take in all of these variables and predict the most accurate vaccination rate of each patient.

## Business Problem
Many pharmaceutical companies like Pfizer are responsible for producing much of our vaccines, including their very successful [COVID-19 vaccine](https://www.fiercepharma.com/pharma/pfizer-to-exceed-100b-revenue-2022-thanks-to-covid-19-drug-and-vaccine-analyst). Despite the success, [a good percentage of US citizens refused to take the vaccine](https://usafacts.org/visualizations/covid-vaccine-tracker-states). Pharma companies can use these predictive models to calculate the percentage of population willing to take the vaccine. They may also observe the differences in vaccination rate of each feature and make further investigations on why differences in a specific feature exists.

## Data
The data is provided by [Drivendata](https://www.drivendata.org/competitions/66/flu-shot-learning/page/210/). They provide three datasets: training labels, training features, and the test set which is used to make our predictions. The labels contain two target variables: `h1n1_vaccine` and `seasonal_vaccine`, where both labels contain binary values where 0 = No and 1 = Yes. [We will be working with 36 features](https://www.drivendata.org/competitions/66/flu-shot-learning/page/211/#sub_values).

## Results/Analysis
Out of the three models (logistic, nearest neighbor, decision tree) it seems like the model with the greatest accuracy and lowest cost is the logistic model. We then calculate the performance of this model by observing the confusion matrix. 
![Confusion matrix h1n1](https://github.com/Jko0425/phase-3-project/blob/main/Images/Confusion%20matrix%20h1n1.png)
The labels are used to obtain the scores:
* __Precision:__ 0.68
* __Recall:__ 0.43
* __Accuracy:__ 0.84
* __F1:__ 0.53
