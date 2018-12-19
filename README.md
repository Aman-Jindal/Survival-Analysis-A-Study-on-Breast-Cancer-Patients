
# A report on Statistical Analysis

## Introduction

In this report you will study a detailed statistical analysis of a [dataset](). This dataset The dataset contains cases from a study that was conducted between 1958 and 1970 at the University of Chicago's Billings Hospital on the survival of patients who had undergone surgery for breast cancer. 
Number of Instances: 306
Number of Attributes: 4 (including the class attribute)
Attribute Information:
   1. Age of patient at time of operation (numerical)
   2. Patient's year of operation (year - 1900, numerical)
   3. Number of positive axillary nodes detected (numerical)
   4. Survival status (class attribute)
         1 = the patient survived 5 years or longer
         2 = the patient died within 5 year.
         
The reasons why I am analyzing this dataset:
* To apply and test my recently acquired knowledge of statistics.
* Most Importantly, its gonna be fun and educational.

## Research Question and Hypothesis

Now we have the information about the dataset, we begin with the assumption that the sample we have is able to fairly approximate the population. That means we have sufficiently large value on n(no. of instances). Our job is to see:
* Combined effect of each variable on the survival status.
* Individual effect of each variable on the survival status.
H<sub>o</sub>: There are no variables which affect the survival status.
H<sub>a</sub>: There are significant number of variables which affect survival status.

![equation1](http://www.sciweavers.org/upload/Tex2Img_1545144480/render.png)

![equation2](http://www.sciweavers.org/upload/Tex2Img_1545144518/render.png)

## Experiment Design

I will fit a Logistic Regression Model to identify which variable are significantly correlated with dependent variable. I choose this test because other test like t-test and ANOVA are done to analyze two samples or more than 2 samples. Also, we can't conduct z-test and Chi-squared goodness of fit because for z-test we should have population data and for chi-squared we should have nominal(categorical) data. Multiple Regression test is done when your dependent variable is continous so Logistic Regression is our best choice in this case. We will use the _Microsoft Excel_ to do this. The step by step process is given in this notebook.

## Result
