# MechaCar_Statistical_Analysis
UT McCombs Data Boot Camp Module 15: Statistics and R
## Linear Regression to Predict MPG
The MechaCar dataset contains a sample size of 50 protoypes measuring the miles per gallon across mulitple variables.  The linear regression was calculated using R in RStudio. 
1. RStudio v.1.4.1103 
2. dplyr library v.1.0.3
### Linear Regression
R script was applied to the dataset on several variables to get the following coefficients.  
![Pic 1](https://github.com/Baylex/MechaCar_Statistical_Analysis/blob/main/Images/1_lin_reg.PNG)
### Summary of Linear Regession model
A summary of the linear regression can be displayed to determine the quality of the dataset.  In this distributuion of the residuals, the dataset fits in with the normal parameters, where the absolute value of the min and max are comparable |-19.47|~|18.58| and the median -.07 is close to zero.

![Pic 2](https://github.com/Baylex/MechaCar_Statistical_Analysis/blob/main/Images/2_sum_stat.PNG)

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
A 95% level of confidence was predeteremined, meaning the p-value should be compared to .05 level of significance to verify if statistically significant.

Coefficeints: 
mpg: 0 < .05, statistically significant, non-random amount of variance 
vehicle length: 0 < .05, statistically significant, non-random amount of variance
vehicle weight: .08 > .05 not statistically significant, random amount of variance
spoiler angle: .31 > .05 not statistically significant, random amount of variance
ground clearance: 0 > .05 statistically significant, non-random amount of variance
AWD: .19>=.05 not statistically significant, random amount of variance

In summay, vehicle length and ground clearance varaibles represent non-random amounts of variance as applied to the mpg values.

2. Is the slope of the linear model considered to be zero? Why or why not?
Converting from scientific notation, all of the slopes of the variables are shown to be non-zero even though some are close to zero: 

Coeffiecients: 
vehicle length: 6.267
vehicle weight: .001
spoiler angle: .069
ground clearance: 3.546
AWD: -3.411

The multiple linear regession formula for mpg = -.01 + 6.267(vehicle length)+.001(vehicle weight)+.069(spoiler angle)+3.546(ground clearance)-3.411(AWD), which results in a non-zero slope.

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
R-squared is .7149, which is a strong correlation for the dataset and shows the dataset is an effective dataset.  However, r-squared is not the only consideration for effectiveness.  There may be other variables not included in the dataset contributing to the variation in the mpg. 

## Summary Statistics on Suspension Coils
### Total Lot Summary
![Pic 3](https://github.com/Baylex/MechaCar_Statistical_Analysis/blob/main/Images/3_tot_sum.PNG)
### Summary by Manufacturing Lot
![Pic 4](https://github.com/Baylex/MechaCar_Statistical_Analysis/blob/main/Images/4_lot_sum.PNG)

1. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not? 
2. There is a summary that addresses the design specification requirement for all the manufacturing lots and each lot individually

✓The csv file is imported and read into a dataframe. ✓The total summary dataframe has ALL FOUR metrics for all the manufacturing lots. ✓The lot summary dataframe has ALL FOUR metrics for each manufacturing lot. ✓The summary addresses the design specification requirement for all the manufacturing lots and ALL THREE lots.


## T-Tests on Suspension Coils
### T-test for all Lots
![Pic 5](https://github.com/Baylex/MechaCar_Statistical_Analysis/blob/main/Images/5_lot_all.PNG)
### T-test for Lot 1
![Pic 6](https://github.com/Baylex/MechaCar_Statistical_Analysis/blob/main/Images/6_lot_1.PNG)
### T-test for Lot 2
![Pic 7](https://github.com/Baylex/MechaCar_Statistical_Analysis/blob/main/Images/7_lot_2.PNG)
### T-test for Lot 3
![Pic 8](https://github.com/Baylex/MechaCar_Statistical_Analysis/blob/main/Images/8_lot_3.PNG)
1. briefly summarize your interpretation and findings for the t-test results. Include screenshots of the t-test to support your summary.

✓An RScript is written for a t-test that compares all manufacturing lots against the mean PSI of the population. ✓An RScript is written for ALL THREE t-tests that compare each manufacturing lot against the mean PSI of the population. ✓The summary addresses the results across all manufacturing lots and ALL THREE lots.


## Study Design: MechaCar vs Competition
1. Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.
2. In your description, address the following questions:
3. What metric or metrics are you going to test?
4. What is the null hypothesis or alternative hypothesis?
5. What statistical test would you use to test the hypothesis? And why?
6. What data is needed to run the statistical test?


The statistical study design has the following: ✓A metric to be tested is mentioned. ✓A null or alternative hypothesis is described. ✓A statistical test is well described to test the hypothesis. ✓The data for the statistical test is well described.

An updated README.md that has the written summaries for Deliverables 1, 2, and 3 and your design for a statistical study comparing vehicle performance of the MechaCars against other manufacturers’ vehicles.
To submit your challenge assignment in Canvas, click Submit, then provide the URL of your MechaCar_Statistical_Analysis GitHub repository for grading.
