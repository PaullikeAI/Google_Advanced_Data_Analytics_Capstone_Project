# Google Data Analytics Capstone Project

## Overview 

The goal of this project was to create a model to predict whether or not an employee would leave the company. The final XGBoost model performed with 97.89% accuracy and a 93% recall of the employees leaving.

The features deemed to be most important in determining whether an employee would leave were employee satisfaction, time spent at the company and the number of projects they were working on. The number of hours worked was also a strong indicator within a subset of employees who worked very long hours.
 
## Exploratory Data Analysis

This was a small dataset with 15,000 rows and 9 features. The dataset was imbalanced with 83.4% of employees not having left the company. The skew of each features distribution was analysed, along with the counts and percentages of certain features, such as salary.
A chi-square analysis was then done between the features salary and department, as it was noted that a high percentage of employees in management had a high salary, and it was found that there was link between these features.
Pair plots and correlation heatmaps were then used to visualise patterns in the data. Additionally monthly hours and last evaluation score were put plotted, and it was noted that every employee who worked for over 288 hours a month left the company.

## Modelling and Evaluation 

Several single models were tested, with Naïve Bayes as the baseline. The results are shown below.

![Single model reults](https://github.com/user-attachments/assets/bcba7c93-51dc-4bf2-8e26-65c748b50058)


Ensemble models were then tested, results shown below. 

![Ensemble model results](https://github.com/user-attachments/assets/7851a6f2-a2aa-4a76-8e78-0b1f3c57f755)


The XGBoost model was chosen to dive deeper into the analysis of feature importances, feature permutations and SHAP. From these conclusion were drawn and business recommendations given.

## Conclusions and Business Recommendations

To retain employees, I would make the following recommendations, based on the model results and EDA. Cap the number of projects an employee is working on a one time, to prevent burn out. Cap the number of overtime hours an employee is allowed to do, unless a special exception is made. The long hours do not help with employee satisfaction, so ensure employees are fairly rewarded for working them if absolutely necessary.
