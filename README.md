# Employee Attrition Analyzing using Machine Learning Models
This is the final project on Big Data Analytics & Data Mining class (Course code：10920IEEM612400) at National Tsing Hua University. 

The original version is accomplished with my teammates. But this new version is finished by myself, I joined GridsearchCV approach to search hyper-parameters and perform cross-validation on the optimized model, analyzed multicollinearity through VIF, and tried to use the PCA approach to found that whether it could reduce the effect. As the result, the classifications' accuracy also progresses. 

## Outline 
- Introduction
- Data Exploration
- Data Interpretation
- The training model and comparison

## Introduction
With the development of the knowledge economy, human resource management has become increasingly important, and how to integrate human demand and employee turnover rate has become a major problem. In addition, the high turnover rate will not only have a negative impact on the company’s funds, but also on the corporate culture and service quality. I expect to use data mining method to continue to analyze human resource for technology companies, and discussed the factors based on the data. I hope that this result can be provided to the company’s decision makers to better management recommendations and methods to build predictive models.

## Data Exploration
The data set used in this study is IBM HR Analytics Employee Attrition & Performance from [kaggle](https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset). This data set is a simulation data created by IBM data scientists, which contains 1470 employee and 35 variables. At this part, we mainly used charts to reveal each variable relations with each other. At the same time, I filtered the vaiables which only had unique data levels or unrelevant.

## Data Interpretation
According to the dataset and variables' mutually relation, I concluded three phenomena and guessed these were the important implication causing employees to quit.

## The training model and comparison
We perform supervised learning to train our model. So, we choose five models to test the accuracy. These include :
- Logistic regression model
- Decision tree model
- Random forest model
- XGBoost classifier
- Gradient boosting classifier

All classifiers utilized the GridsearchCV approach to search hyper-parameters and performed cross-validation to optimize the accuracy.
In addition to this, I analyzed multicollinearity through variance inflation factor and tried to reduce the effect using the PCA approach.
After training different models, we made the ROC graph to compare each model as follows.

![下載](https://user-images.githubusercontent.com/84038124/136109759-5d35727e-9d2d-4d8d-bc9d-70471ae7ad2b.png)
