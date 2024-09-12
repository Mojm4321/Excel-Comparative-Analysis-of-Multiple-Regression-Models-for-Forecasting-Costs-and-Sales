# Comparative Analysis of Multiple Regression Models for Forecasting Costs and Sales By Jolly Madamedon

# Introduction
Multiple regression allows us to explore the relationships between a dependent variable and several independent variables, providing insights into which factors most influence the target outcome.

This report aims to compare the forecasting abilities of three multiple regression models and identify which is most effective for its specific scenario. This evaluation focuses on analysing the performance of each model in predicting outcomes across different business contexts.

The first model predicts taxi rides costs based on distance travelled, duration of the tax ride and age of the passengers. The second model assesses the drivers of monthly production costs for different manufactured goods - specifically tables, chairs, doors and fridges. The third model forecasts sales performance of a song based on airplay frequency, product attractiveness and advertising expenditure. 

The accuracy and performance of these models are judged using three main factors: Adjusted R², which tell us how well the model explains the variation in the data; P-values, which shows how important each factor is in predicting the outcome and Scatter plots, which provide a visual check to see how well the predictions match the actual data and help identify any outliers that don't fit the pattern.

# Model 1 : Predicting Taxi Ride Costs

Diagram 1 shows the relationship between taxi ride costs and the key influencing factors, such as distance travelled, ride duration and passenger age.

![Diagram 1](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/original%20data%20table%201.png)


Diagram 1

In the original linear regression model  for predicting taxi ride costs all three independent variables were included. However, the regression analysis revealed that distance was the only significant predictor with a p-value of 0.04304, while duration (p = 0.99176) and age (p = 0.85337) were statistically insignificant. 

A pvalue below 0.05 indicates that the variable has a meaningful impact on the predicted outcome, whereas higher pvalues suggests that the variables have little influence on the outcome and should be excluded to improve model accuracy. Therefore, both duration and age were poor contributors to predicting taxi ride costs, and their inclusion led to a lower Adjusted R² of 0.50142, as shown in Diagram 2

![Diagram 2](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/original%20data%20table%202.png)


Diagram 2

By refining the model to focus solely on distance travelled, the predictive accuracy improved a lot.
Removing the insignificant variables resulted in an Adjusted R² of 0.62309, indicating a better fit for the data. The p-value for distance decreased to 0.00403 further confirming its strong influence on taxi ride costs, as shown in Diagram 3.

![Diagram 3](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/original%20data%20table%203.png)


Diagram 3

To forecast the cost of a taxi ride, the final regression equation was simplified to 9.7127*(journery distance)+7.1504. For example, for a 20 mile journey the model predicts a taxi fare of approximately £187.10, as shown in Diagram 4.

![Diagram 4](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/original%20data%20table%207.png)

Diagram 4

Scatter plots provider further clarity. ThE plot in Diagram 5 shows a positive linear relationship between distance and taxi ride costS as most data points closely following the trendline. Outliers such as ride that cost significantly more or less than expected may be explained by factors like traffic, which are not accounted for in the model. 

In contrast, Diagram 6 and Diagram 7 illustrate the plots for during and age, respectively. Both demonstrate no clear trends or patterns with data points scattered inconsistently. This reinforces the conclusion that these variables did not meaningfully contribute to predicting taxi ride costs, therefore, excluding them made them more accurate and easier to interpret.

![Diagram 5]()


Diagram 5


![Diagram 6]()


Diagram 6


![Diagram 7]()


Diagram 7
 
# Model 2: Predicting Monthly Production Costs
