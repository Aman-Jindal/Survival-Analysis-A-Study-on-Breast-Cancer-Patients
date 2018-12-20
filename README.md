
# A report on Statistical Analysis

## Introduction

In this report you will study a detailed statistical analysis of a [Haberman’s Survival Data Set](http://archive.ics.uci.edu/ml/datasets/Haberman%27s+Survival). This dataset contains cases from a study that was conducted between 1958 and 1970 at the University of Chicago's Billings Hospital on the survival of patients who had undergone surgery for breast cancer.        
Number of Instances: 306                              
Number of Attributes: 4 (including the class attribute)

Attribute Information:
1. Age of patient at time of operation (numerical)
2. Patient's year of operation (year - 1900, numerical)
3. Number of positive axillary nodes detected (numerical)
4. Survival status (class attribute)                                     
   1 = the patient survived 5 years or longer                               
   2 = the patient died within 5 year.                   

Dependent variable = 'Survival status'.                                    
Independent variables = 'Age', 'Patient's year of operation', 'Number of positive axilliary nodes detected'.

The reasons why I am analyzing this dataset:
* To apply and test my recently acquired knowledge of statistics.
* Most Importantly, its gonna be fun and educational.

## Research Question and Hypothesis

Now we have the information about the dataset, we begin with the assumption that the sample we have is able to fairly approximate the population. That means we have sufficiently large value on n(no. of instances). Our job is to see the effect of each independent variable with the dependent variable(see the correlation between the variables). So, our hypothesis goes like this:
H<sub>o</sub>: There are no variables which affect the survival status.
H<sub>a</sub>: There are significant number of variables which affect survival status.

![equation1](https://github.com/Aman-Jindal/Statistical-Analysis/blob/master/images/eq1.png)

![equation2](https://github.com/Aman-Jindal/Statistical-Analysis/blob/master/images/eq2.png)

Here ![mu](https://github.com/Aman-Jindal/Statistical-Analysis/blob/master/images/mu.png) represents the number of independent variable.

## Experiment Design

Let's see what are type(measurement scale) of independent and dependent variable. You can see the dependent variable is 'nominal'(categorical)  and all the independent variables are 'Interval'(values with equal intervals and an absolute zero). As our dependent variable is 'nominal' we will perform chi-square test to check the significance of correlation between the variables.(There are also other type of test which we can perform here but they were not covered in this course). 

I choose this test because other test like t-test and ANOVA are done to analyze two samples or more than 2 samples. Also, we can't conduct z-test and Chi-squared goodness of fit because for z-test we should have population data and for chi-squared we should have nominal(categorical) data. Multiple Regression test is done when your dependent variable is continous so Logistic Regression is our best choice in this case. We will use the _Microsoft Excel_ to do this.

The step by step process is given in this notebook.

## Result

### Descriptive Statistics

![table1](https://github.com/Aman-Jindal/Statistical-Analysis/blob/master/images/descriptive_result.jpg)

### Inferential Statistics

* Test between 'Number of axilliary nodes' and 'Survial'.

alpha = 0.001                                        
chi_square(2) = 35.27, p < 0.001, one tailed 

The p-value of chi-square test is less than 0.001 which shows that there is significant correlation between the variables and the value of crammer's V confrims that there is indeed a strong relationship.

* Test between 'Age of patient at the time of operation' and 'Survival'

alpha = 0.05                                                   
chi_square(2) = 2.31, p > 0.05, one tailed 

The p-value of chi-square test is more than 0.05 which shows that there is not significant correlation between the variables.

* Test between 'Year of Operation' and 'Survival'

alpha = 0.05                                               
chi_square(2) = 2.07, p > 0.05, one tailed 

The p-value of chi-square test is more than 0.05 which shows that there is not significant correlation between the variables.

So, We will reject the null as there is significant variables(more than 0) which affect the dependent variable.

## Conclusion

The results of the report are not in favour of null hypothesis. We also see that 'Age at the time of Operation' and 'Year of Operation' does not have a significant correlation with the dependent variable. This may be because our sapmle does not approximate the population well. Moreover, there can also be individual reasons maybe age does not influence your survival its more depends on cancer cells and for year of operation there might not be significant improvement in the technology or research in that time period. We are not sure, future research is required to make further analysis.

## References

1. Haberman, S. J. (1976). Generalized Residuals for Log-Linear Models, Proceedings of the 9th International Biometrics Conference, Boston, pp. 104-122.
2. Landwehr, J. M., Pregibon, D., and Shoemaker, A. C. (1984), Graphical Models for Assessing Logistic Regression Models (with discussion), Journal of the American Statistical Association 79:61-83.
3. Lo, W.-D. (1993). Logistic Regression Trees, PhD thesis, Department of Statistics, University of Wisconsin, Madison, WI.

