# MechaCar Statistical Analysis

A statistical study using **R** to compare vehicle performance.

## Overview of the analysis: 

The following study contains three technical analysis deliverables and a proposal presented as follows::

1. Deliverable 1: **Linear Regression to Predict MPG**
2. Deliverable 2: **Summary Statistics on Suspension Coils**
3. Deliverable 3: **T-Test on Suspension Coils**
4. Deliverable 4: **Design Proposal** a Study Comparing the MechaCar to the Competition

## Linear Regression to Predict MPG

- We designed a linear model that predicts the **mpg** of MechaCar prototypes using several variables from the `MechaCar_mpg.csv` and the resulting model can be viewed on the image below:

	![alt text](https://github.com/Karenjakins/MechaCar_Statistical_Analysis/blob/main/Resources/Deliverable%201.png "Deliverable 1")
	
	**SUMMARY**

	From the results above:

	* Which **variables/coefficients** provided a non-random amount of **variance to the mpg values** in the dataset?

	In this dataset the **vehicle_length**, **ground_clearance** (as well as the **intercept**) provided non-random amounts of variance to the mpg values. 

	* Is the slope of the linear model considered to be zero? Why or why not?

	The linear model's slope is not considered to be zero as the **p-Value** for this model is `5.35e-11` which is significantly smaller than the **significance level = 0.05%**. 

	* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

	This linear model predicts prototypes of mpg MechaCar effectively since the **r-squared** value is **0.7149**, which means that about **71%** of all mpg predictions will be effectively determined by this model.


## Summary Statistics on Suspension Coils

- The `Suspension_Coil.csv` file contains data on the results of testing weight capacities of various suspension coils from several production lots to determine overall consistency.

	**SUMMARY**

	**Total Summary**

	![alt text](https://github.com/Karenjakins/MechaCar_Statistical_Analysis/blob/main/Resources/Deliverable%202%20-%20Total%20Summary.png "Deliverable 2 - Total Summary")

	**Lot Summary**

	![alt text](https://github.com/Karenjakins/MechaCar_Statistical_Analysis/blob/main/Resources/Deliverable%202%20-%20Lot%20Summary.png "Deliverable 2 - Lot Summary")

	From the results above:

	The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch (**PSI**). Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not? 

	For this model, **Lot 1** and **Lot 2** meet design specifications, having very close **mean** and **median** values, with variances of **0.97** and **7.47**. However, **Lot 3** has the most variance amongst the three, **170.28** and does not meet the manufacturing expectations.

## T-Tests on Suspension Coils

- T-tests were conducted on the `Suspension_Coil.csv` to determine if there is a **statistical difference** on this dataset. Using the sample population mean of **1500**, these are our findings:

	**SUMMARY** 

	![alt text](https://github.com/Karenjakins/MechaCar_Statistical_Analysis/blob/main/Resources/T-test%20for%20all%20lots.png "T-test for all lots")
	
	We can observe from the results that the true mean is **1498.78** which was also on our summary statistics table for **Deliverable 2**. The t-test shows there is not enough evidence to reject the null hypothesis since the **p-value** for all manufacturing lots is **0.06028** higher than the common significance level of 0.05. 

	**Lot 1**
	![alt text](https://github.com/Karenjakins/MechaCar_Statistical_Analysis/blob/main/Resources/T-tests%20for%20Lot%201.png "T-tests for Lot 1")
	**Lot 2**
	![alt text](https://github.com/Karenjakins/MechaCar_Statistical_Analysis/blob/main/Resources/T-tests%20for%20Lot%202.png "T-tests for Lot 2")
	**Lot 3**
	![alt text](https://github.com/Karenjakins/MechaCar_Statistical_Analysis/blob/main/Resources/T-tests%20for%20Lot%203.png "T-tests for Lot 3")

	For each individual lot, *Lot 1 had a p-value of 1 and Lot 2 had a p-value of 0.60*, both statistically similar which means we cannot reject the null hypothesis. For **Lot 3**, the sample mean is **1496.14** with a **p-Value of 0.04**, lower than the significance level of 0.05 which indicates that the sample mean and the presumed population mean are not statistically different.

## Study Design: MechaCar vs Competition

- sjhfbadkfbd

## Resources

**Data Source:** MechaCar_mpg.csv, Suspension_Coil.csv

**Software:** RStudio, R