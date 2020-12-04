# MechaCar_Statistical_Analysis
## Linear Regression to Predict MPG


- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

    ![](/img/lm.PNG)
Vehicle_length and ground_clearance provide are statistically to provide non-random amount of variance to the mpg values in the dataset as vehicle_length and ground_clearance have the lease Pr(>|t|) value comparing to other variables. Intercept is statistically significant, it means there are other variables and factors that contribute to the variation in mpg that have not been included in our model.  


- Is the slope of the linear model considered to be zero? Why or why not?

      ![](/img/lm_summary.PNG)
The slope of the linear model is not considered to be zero. This is because from the linear regression model, 
p-value of our linear regression analysis is 5.35e-11, which is much smaller than our assumed significance level of 0.05%. Therefore, we can state that there is sufficient evidence to reject our null hypothesis, which means that the slope of our linear model is not zero.


   
- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
The linear model predicts mpg of MechaCar prototypes effectively. This is because the r-squared value of the dataset is 0.6825 which means roughly 68% of all mpg predictions will be correct when using this linear model. 

## Summary Statistics on Suspension Coils


 - The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

    ![](/img/summary_coil.PNG)

    ![](/img/lot_summary_coil.PNG)

 Based on the summary, the overall variance is 62.29 which meets manufacturing specification. However, when looking at the lots level, lot1 and lot2 meet the manufacturing specification with variance of 0.98 PSI and 7.47 PSI. Lot3 does not meet the manufacturing specification with variance of 170.29 PSI which is over the 100 pounds per square inch requirement. Therefore, manufacturing team should work on improving the manufaturing in lot3. 


 ## T-Tests on Suspension Coils

 - By using significance level of 95%, our p-value 0.06028 is above our significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis that PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch, and the two means are statistically similar. By looking at the p-value at the lot level, lot1 has p-value of 1, lot2 has p-value of 0.6072 and lot3 has p-value of 0.04168. Therefore, we do not have sufficient evidence to reject the null hypothesis that lot is not statistically different from the population mean of 1,500 pounds per square inch for all lots result, lot1 and lot2. We would reject lot3 because p-value is below 0.05 percent which means lot3 is statistically different from the population mean.
    ![](/img/All_t_test.PNG)
    ![](/img/lot1_t_test.PNG)
    ![](/img/lot2_t_test.PNG)
    ![](/img/lot3_t_test.PNG)

## Study Design: MechaCar vs Competition
- Cost, city or highway fuel efficiency, horse power are the main three factors would be of interest to a consumer. In order to compare the MechaCar vehicles with other competitions, I would use cost, city or highway fuel efficiency, horse power to perform analysis between MechaCar vs Competitions. 
- The null hypothesis I wil use is assuming the MechaCar assuming there is no difference between MechaCar and competition for the vehicles performance in the same cost range. The alternative hypothesis is there is material difference between MechaCar and competition for the vehicle's performance comparing to price.
- I will use analysis of variance (ANOVA) test, which is used to compare the means of a continuous numerical variable across a number of factors.
- The required data would be sufficient cost, city or highway fuel efficiency, horse power data for vehicles from other competitions. 