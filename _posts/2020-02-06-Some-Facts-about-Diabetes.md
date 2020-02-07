---
layout: post
title: Diabetes is an Evil Disease
subtitle: Some Facts about Diabetes

tags: [diabetes, data science]
---

_The diabetes patients has risen 4 times in 34 years (1980 to 2014). It can cause blindness, kidney failure, heart attacks, stroke and lower limb amputation.

Almost half of all deaths before the age of 70 years are attributable to diabetes.It is the seventh leading cause of death in 2016._

## Some facts :

It is strongly associated to age, obesity, pregnancy, blood pressure, genetic factor . Diabetes can be treated with diet, physical activity, medication .

## How I did?

I collected, cleaned, analyzed, and visualized the data (size 768 x 9).

## Useful ?

    To see clearly how some factors take so import on causing this disease.
    To make a model to diagnose diabetes for medical remote diagnosis in the future.

# Methods & Analysis:

## I. To build a correlation coefficients matrix 
![Correlation Coefficients Matrix](https://miro.medium.com/max/879/1*Gzzi5g8u5bZPNswjcvVhyA.png)


We can see glucose level shows positive correlation with insulin (r= 33.13%), age (r= 26.35%), BMI (r= 22.11%), blood pressure (r= 15.26%), genetic factor (13.73%), pregnancy (r= 12.95%), Skin Thickness(r= 5.73%).

## II. Seanborn Pairplot Graph1
![Seanborn Pairplot Graph1](https://miro.medium.com/max/1144/1*uk3jEFXDZCeRybhasmW9iA.png)


## III. Seanborn Pairplot graph 2
![Seanborn Pairplot Graph1](https://miro.medium.com/max/1349/1*otYsp9K0m2JA04vvq4IlEw.png)

## IV. Seanborn pairplotting
![Seanborn Heatmap](https://miro.medium.com/max/328/1*0JcOIMP_jkVVD5E7pSU4RA.png)



# Conclusion:

Diabetes is positive correlated to body weight, age, pregnancy, blood pressure, genetic factor, and so on. 
We can use such facts diagnose this disease and improve the therapy. 
E.g. , higher BMI is correlated to diabetes, so lose wight, diet, physical activit can help to treat this disease.

In the future, we can  make a model to diagnose diabetes for long distnace diagnosis.

[Data resources](https://data.world/anaozp/diabetes/workspace/file?filename=diabetes.csv)
