# MechaCar_Statistical_Analysis
An analysis of production data to assist the manufacturing team 


## Overview
### Jeremy is contacted by AutosRUs that their special prototype in development, the "MechaCar" is suffering from production setbacks which in turn is creating a roadblock for the team's progress. Upper management from AutosRus is asking Jeremy and the analytics team to take a look at the production data and give advice to the manufacturing team on how to proceed. 

### A few goals for the project:
* What variables affect MPG for vehicles/prototypes
* View the summary statistics on the PSI on suspencion coils
* If manufacturing lots are statistically different from the average population
* Finally, design an analysis to contrast MechaCar's performance against the vehicles of other manufacturers.

## Linear Regression to Predict MPG!
![Screen Shot 2022-07-03 at 9 06 26 PM](https://user-images.githubusercontent.com/102098068/177069338-442b3c53-97e4-4a97-807e-bb91edaeb145.png)

* In this linear regression model, the variables that appear to have a significant contribution to a vehicle's mileage are the ground clearance and the length of the vehicles variables. In the summary view of the linear regression, there are three asterisks for both variables, which indicate a statistically significant result. The intercept is also interpreted as statistically significant, however, this only indicicates that there are other factors not included in the linear regression that has a large impact on the mileage.

* The p-value for the slope of the linear model is 5.35x10^-11, which is extremely low, rejecting the null hypothesis. With the rejection of the null hypothesis, we can assert that the relationship between the variables of the dataset and the milage of the vehicle is affected by more variables than by random coincidence.

* The r-squared value is in the 0.7 range, thus asserting that the model is around 70%-72% accurate, however, as with all data models, more data could be used and inserted to increase the value of the r-square for a more accurate model. 

## Summary Statistics on Suspension Coils
![Screen Shot 2022-07-03 at 9 09 49 PM](https://user-images.githubusercontent.com/102098068/177069524-c9706048-bc7a-48ea-9e85-800f3d42e1b0.png)

![Screen Shot 2022-07-03 at 9 09 38 PM](https://user-images.githubusercontent.com/102098068/177069541-7923c846-a7e9-4818-8391-7d1c4a9e1b26.png)


* The specifications are met overall as the summary data shows that it is under 100 psi and meets the specifications. Despite this, there is one lot in particular, Lot 3, that is shown to have variable that is above the acceptable threshold at 170.28

## T-Tests on Suspension Coils

![Screen Shot 2022-07-03 at 9 11 25 PM](https://user-images.githubusercontent.com/102098068/177070200-7e9b97a6-a428-4e9d-827b-a00a35ef98eb.png)

* Review of the T-test results shows that the suspension coils from all manufacturing lots show that they are not statistically different from the population average, and the p-value is too high to reject the null hypothesis. 

![Screen Shot 2022-07-03 at 9 16 45 PM](https://user-images.githubusercontent.com/102098068/177070225-f6c53d5c-5c76-4a91-857d-4eba7c320c98.png)

* For the t-test for the Lot 1 suspension coils, the results show that they are not statistically different from the average of the population, with the p-value too high to reject the null hypothesis.

![Screen Shot 2022-07-03 at 9 18 29 PM](https://user-images.githubusercontent.com/102098068/177070301-d5fe9ec6-9c78-4fd7-b6b7-e5e84345118d.png)

* For the t-test on Lot 2 suspension coils, it is not statistically different enough from the population average, and the p-value is too high to reject the null hypothesis.

![Screen Shot 2022-07-03 at 9 19 42 PM](https://user-images.githubusercontent.com/102098068/177070403-6c53b66c-54fc-4538-9211-12e8a864c485.png)

* T-test on the suspension coils for Lot 3 shows that it is statistically different from the population mean. Also, the p-value is lower than the others and it is enough to reject the null hypothesis. Either the lot needs to be disposed of or more closely examined. 

## Study Design: MeechaCar vs Competition 
### Every individual considers different factors while deciding on a car to purchase. With the advent of other factors such as ridesharing coming into the fold in the past decade, the average individual is looking for the most economical vehicle and whether it meets their preferences. Therefore, many important factors would be milage (miles per gallon), reliability, size, etc. 

## Which metrics should be tested?
### The average carbuyer would look for a vehicle to suit their needs, therefore, a consideration for a vehicle purchase would be the size of the vehicle. Thus, a metric that could be tested for this would be the amount of capacity in storage in cubic inches in comparision to other vehicles. 

## Null and Alternative Hypotheses
### Null Hypothesis: The prototype for MechaCar has a similar carrying capaicity to other vehicles in the same vehicle class.
### Alternative Hypothesis: The prototype for MechaCar is statistically different (either above or below) the competitot vehicles.

## Best Statistical Test to Use
### For this examination, a two-sample t-test will be used. Data for cubic space would be needed from all of the MechaCar prototypes along with data from major competitor vehicles.

