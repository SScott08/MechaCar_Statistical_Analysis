##MechaCar_Statistical_Analysis

Objective-

In this repository I will use techniques using R and statistical analysis to provide analysis for AutosRUs a car manufacturer. 
The team had provided 2 complete datasets. The first dataset is comprised of different design specification such as vehicle length, vehicle weight, ground clearance, MPG.The second dataset consists of MechaCar coil suspension test results from different manufacturing lots. 

## Linear Regression to Predict
Using Multiple Linear Regression analysis on the MechaCar MPG prototypes. The variables displayed significant relationships with other variables, such as MPG and vehicle length. Using regression analysis at each dependent variable, low p-values were found to have less random variance to the linear model. These variables have more impact on the MPG. These were vehicle length and ground clearance.

The Y-intercept also had a small p-value, which suggests that not many factors contributed to the regression of MPG. Since p-value was higher for vehicle weight, spoiler angle, and AWD (all-wheel drive), those variables offered more random variability, thus they have a less chance of affecting MPG.

The calculation of the regression slope and y intercept determines the distance between each data point of a dataset. The slope was found not to be zero since, assuming the significance level of 0.05% within normal, the multiple regression p-value is 5.35e-11, which portrays the slope is not zero, reject the null hypothesis.

The result of this test was to use a linear model to predict MPG of MechaCar prototypes effectively. The linear model can predict the MPG since the r-squared value is .71, meaning 71% of all mpg predictions will be correct when using this linear model and our p-value is much smaller than 0.05%, which would suggest that the overall slope of our linear model is not zero.


## Summary Statistics on Suspension Coils
In this test, the team needed a summary statistic for the suspension coil’s PSI (pounds-per square inch) and verify the variance of PSI. The current manufacturing data met this design specification since the variance of PSI is 76.23, which is under 100 psi.

## T-Test on Suspension Coils
This test relied on the Student T-Test which should determine if the suspension coil’s PSI results are statistically different from the mean population results of 1,500 PSI. Taking 30 sample datapoints from the 150 datapoints from the population dataset, the density graphs of both population and sample look similar. Since we are comparing mean population dataset and sample dataset, the use of one-sample t-test would make sense.

Since 0.05% is the significance level, our p-value of .63 is above our significance level, which suggests that the two means are statistically similar. The test also has a 95% confidence interval of 1494.9-1502.4, which would mean the population mean of 1500 falls under the 95% confidence interval.

##Study Design: MechaCar vs Competition

The team wanted to further expand their MechaCar prototype testing to evaluate similar vehicles from the ompetition. One design study that would require further research could be comparing fuel efficiencies of MechaCar prototypes with their competition. A possible null hypothesis could be whether top performing MPG of MechaCar Prototypes have the same fuel efficiency as the competitors cars’ MPG. The alternate hypothesis would be whether MPG of MechaCar samples have a positive delta change, thus MechaCar would be beating out other competitors’ fuel efficiency.

The collected data needed for statistical analysis could be collected from top 5 samples of MechaCar prototypes that have varying design specifications from vehicle lengths and ground clearance since those specifications affect MPG the most. Then we could match those specifications with the competitors’ cars and analyze both MPG. Another method could be to call a subset for each manufacturing lot and perform a t-test to see which lot is not meeting the standard.
