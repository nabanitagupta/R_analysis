# R_analysis
# MPG Regression
## Question: Provide a small writeup of your interpretation of the multiple linear regression results. Be sure to include the following details:
# •	Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
# •	Is the slope of the linear model considered to be zero? Why or why not?
# •	Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

Following picture captures the summary of the linear model (lm) for the mpg values in the MechaCar dataset.

![alt text] (https://github.com/nabanitagupta/R_analysis/blob/master/MPG_Regression_MLR.png) 

As per the lm, 2 variables – (a) vehicle length and (b) ground clearance provide non-random variance to the mpg values in the MechaCar dataset. One can consider vehicle weight as non-random indicator of mpg values. However, it has very little significance. 
The slope is non-zero because the p-value: 5.35e-11; very small.

This lm does a good job of predicting mpg of MechaCar prototypes as indicated by 0.71 R-squared value. 
#####################################################################################
# Suspension Coil Summary
## Question: Calculate summary statistics for quantitative variables.
# Be sure to include the following metrics:
•	Mean
•	Median
•	Variance
•	Standard deviation
# The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per inch. Does the current manufacturing data meet this design specification? Why or why not?

Following is the summary statistics for the suspension coil summary
![alt text] (https://github.com/nabanitagupta/R_analysis/blob/master/Summary_SuspensionCoil.png)

As indicated in the summary table, lot1and lot 2 meet the design specification, whereas the lot 3 has much higher variance: 170.286. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per inch. Hence, lot 3 doesn’t meet the design specification. 

# Suspension Coil T-Test
## Question: 
# •	Using the same suspension coil data and the MechaCarChallenge.RScript file, determine if the suspension coil’s pound-per-inch results are statistically different from the mean population results of 1,500 pounds per inch. (Hint: Refer to the t-test section of this module to determine which statistical test to use.)
# •	In the MechaCarWriteUp.txt text file, provide a small writeup of your interpretation and findings for the t-test results.

Lot 1 and lot 2 have population mean as the entire population i.e. 1500 psi. Lot 3 has same mean but the p-value (0.042) is below the significance level. Hence, it can be concluded that lot 3 is statistically different from population mean. 

# Design Your Own Study
## Question: Write a short description of a statistical study that can quantify how the MechaCar outperforms the competition. In your study design, be sure to write about the following considerations:
# •	Think critically about what metrics you would think would be of interest to a consumer (cost, fuel efficiency, color options, etc.).
# •	Determine what question we would ask, what the null and alternative hypothesis would be to answer that question, and what statistical # test could be used to test this hypothesis.
# •	Knowing what test should be used, what data should be collected?

Two foremost parameters come to mind regarding cars are horsepower along with mpg. Hence, it will be good to include horsepower data from other competitor cars and multiple datapoints for the MechaCar’s horsepower and run a statistical analysis. The hypothesis to test would be:
Ho: There is no statistical difference between horsepower of MechaCar and the competitor car. 
Ha: There is statistical difference between horsepower of MechaCar and the competitor car. 
We can use one-sample t-test, where the population data will be all datapoints including competitor data and data from MechaCar. 
Again, we will need to include horsepower data from other competitor cars and multiple datapoints for the MechaCar’s horsepower for the above mentioned analysis. 

