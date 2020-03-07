---
layout: post
title: Predicting Salary with BLS 2019 Dataset
subtitle: With Predictive Modeling 

tags: [Salary, job selection, data science]
---
![alt text](https://miro.medium.com/max/381/1*xLOpEgjdX0sxrE-I7SLJ2A.gif)

## I. Purpose

Wages are affected by multiple factors. The purpose of this post is to predict wage by using machine learning to fit regression models on the dataset and evaluate the accuracy of the models by obtaining mae and/or R². In order to get better prediction and avoid leakages, we would do data wrapping and feature engineering by multiple methods.

## II. Data

My dataset(size(62742 x 21)) is obtained from U.S. Bureau of Labor Statistics(BLS). BLS publishes the most recent American wage information. It is not from UCI datasets. Website : https://www.bls.gov/web/cewqtr.supp.toc.htm.

## III. Description
Wage is affected by multiple factors, such as economics development, region(nation, state, county), ownership(privacy or federal), industry type, employment rate, and so on.
The target is “Average Weekly Wage”(Abbreviated as wage) .
Main features’ details: Employment Location Quotient(an economic indicator), Ownership(Total Covered, Federal, State, and Local Government, private), Industry(10 Total, Natural resources and mining, Construction, Manufacturing, Service, Trade,and so on), St Name(52 states), Area Type(‘Nation, State, County), Employment (April, 2019), etc.
Visualization graph were shown for the data analysis and help to explain the prediction methods.
Libraries I used: Pandas , NumPy , Seaborn , Scikit-learn, Matplotlib, SciPy, category_encoders, matplotlib, numpy, pandas, plotly, scikit-learn, pdpbox, shap, xgboost, etc.


## IV. Data wrapping and feature engineering

### 1. Pandas_profiling is a useful tool for doing the exploratory data analysis. It gives us more insights into the data such as missing values, zero values, duplicates, count, mean, median, , distribution of data, correlation of variables with each other, type of variables, right or left skewed data, and so on.
![[alt text]](https://miro.medium.com/max/222/1*xtESqnnUFvDUKi39itOAGQ.png)
![[alt text]](https://miro.medium.com/max/559/1*O2nEBIdMA1cL1FSC-LP_ag.png)

### 2. I remove the 1% extreme value of target. For feature engineering, I remove the features with null value, high cardinality , duplicate, and the ones suspected for leakage.
![[alt text]](https://miro.medium.com/max/377/1*EFv8xBimvEPVzJZJoFWcrw.png)
### 3,  Beginning with default baseline prediction.
![[alt text]](https://miro.medium.com/max/320/1*va-6b41FbUkCMQaa-65I7A.png)
## V. To build different regression models and evaluated by Mae or R²

![[alt text]](https://miro.medium.com/max/503/1*-FGk55_fFa0aQdvaq0OEdg.png)
## VI. Visualization about relationship between wage and the features
### 1. Wage with ownerships
![[alt text]](https://miro.medium.com/max/334/1*6XKwOx_Av_A8bUvHZ9I_4A.png)
### 2. Wage with industry

![[alt text]](https://miro.medium.com/max/322/1*Rp3tD1jWX0HPe7l59AwIDQ.png)

### 3. Wage with area type

![[alt text]](https://miro.medium.com/max/326/1*H7Y8LmjmKUuQpCTf39hYTw.png)
### 4. Wage with different state
![[alt text]](https://miro.medium.com/max/769/1*PjWZVG66HstfGxn9oShM_g.png)
### 5. Wage prediction with one feature’s Partial Dependence Plots(ICE)
![[alt text]](https://miro.medium.com/max/715/1*oYnOwFDvJf6euFoJ7kxozw.png)
### 6. Wage prediction with two features’ Partial Dependence Plots

![[alt text]](https://miro.medium.com/max/410/1*Ln9tl7kr2FB1atfHEBCLgw.png)
### 7. Wage prediction with two features’ 3D plot
![[alt text]](https://miro.medium.com/max/494/1*zQSrSz8GImfaVnMwtLm97w.png)
### 8. Wage prediction with four features’ Xgboost Shap interactions
![[alt text]](https://miro.medium.com/max/624/1*UoettwmmJUrrJHC7-DP60w.png)

## VII. Summary
· For data cleaning and feature engineering, using pandas profile report saved time.

· Some models show much better prediction, therefore, the model selection is very important .

· Visualization is important . A good picture is worth thousands of words.

· This project can help us to make job and career selection. If you want to get high salary, I persuade you to go federal government , or relocate to Connecticut or DC area, and avoid the service industry, and so on.

[Data resources]( https://www.bls.gov/web/cewqtr.supp.toc.html)
