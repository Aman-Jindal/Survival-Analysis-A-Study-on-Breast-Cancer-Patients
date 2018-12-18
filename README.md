
# A report on Statistical Analysis

## Introduction

In this report you will study a detailed statistical analysis of a [dataset](). This dataset is quite famous, it outlines the quality
of wine based on certain attributes. There are two types of wines given here, red and white. There are different number of total observations. We will study each type of wine each separately. According to the source of the dataset this can be viewed as classification or regression. The classes are ordered and not balanced (e.g. there are munch more normal wines than excellent or poor ones).

Number of Instances: red wine - 1599; white wine - 4898.
Number of Attributes: 11 + output attribute.

The reasons why I am analyzing this dataset are:

* To apply and test my recently acquired statistics skills.
* To educate you and myself about the wine characterstics and which are the most important characterstics that makes a good wine.
* Most Importantly, its gonna be fun and educational.

## Research Question and Hypothesis

My research answer the question: Which of the variables affect the quality of wine and if they do are they statistically significant? To answer this question I will identify the variables which are highly correlated with the dependent variable. So, the _null_ and _alternate_ hypothesis goes like this:   

H<sub>o</sub>: There are no variables which affect the wine quality.
H<sub>a</sub>: There are significant number of variables which affect the wine quality.

![equation1](http://www.sciweavers.org/upload/Tex2Img_1545144480/render.png)

![equation2](http://www.sciweavers.org/upload/Tex2Img_1545144518/render.png)

## Experiment Design

I will conduct a Multiple Regression Test to identify which variable are significantly correlated with dependent variable. I choose this test because there are lot of variables in this test and it will time consuming to do tests like t-test, Linear Regression with two variable with two samples or analysis of variance with 2 or more samples(In Anova we take all the variables at once but it will be difficult to conclude which are significant). Also, we can't conduct z-test and Chi-squared goodness of fit because for z-test we should have population data and for chi-squared we should have nominal(categorical) data. Multiple Regression test will be a best choice in this case. However, we can't visualize the data as there are so many variables but we can interpret the coefficients associated with each variable and their corresponding p-value. We will use the _Microsoft Excel_ to do this. 
