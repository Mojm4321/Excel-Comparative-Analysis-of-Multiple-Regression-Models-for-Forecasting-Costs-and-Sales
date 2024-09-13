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

![Diagram 4](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/original%20data%20table.png)

Diagram 4

Scatter plots provider further clarity. The plot in Diagram 5 shows a positive linear relationship between distance and taxi ride costS as most data points closely following the trendline. Outliers such as ride that cost significantly more or less than expected may be explained by factors like traffic, which are not accounted for in the model. 

In contrast, Diagram 6 and Diagram 7 illustrate the plots for duration and age, respectively. Both demonstrate no clear trends or patterns with data points scattered inconsistently. This reinforces the conclusion that these variables did not meaningfully contribute to predicting taxi ride costs, therefore, excluding them made them more accurate and easier to interpret.

![Diagram 5](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/original%20data%20table.png)


Diagram 5


![Diagram 6](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/Duration%20Minutes%201.png)


Diagram 6


![Diagram 7](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/Passenger%201.png)


Diagram 7
 
# Model 2: Predicting Monthly Production Costs

Diagram 8 shows the relationship between monthly production costs and the key drivers: the number tables, chairs, doors and fridges.

![Diagram 8](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/2nd%20model%201.png)


Diagram 8


In the original linear model for predicting production costs, all four variables were included : tables, chairs, doors and fridges. However, regression analysis revealed that while tables (pvalue = 0.00865) and fridges (pvalue = 0.02414) were significant predictors, chairs (pvalue = 0.9934) and doors (pvalue = 0.47114) were not, as shown in Diagram 9. The inclusion of these insignificant variables contributed to a lower Adjusted R² of the  0.5423, indicating that the original model was less accurate due to unnecessary variables.

![Diagram 9](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/2nd%20model%202.png)


Diagram 9

The finalised model retained only the significant predictors, tables and fridges, which resulted in an improved Adjusted R² of 0.64798, demonstrating a better fit to the data. In this refined model, both tables (pvalue=0.00539) and fridges (pvalue=0.02079) remained very low, illustrated in Diagram 10,  indicating their strong influence on production costs.

To forecast the product cost, the final regression equation was simplified to (92.3507 x tables produced) + (83.7226 x fridges produced)+10313.83231. For example,for the production of 500 Tables and 400 Fridges, the model predicts a total cost of approximately £89,978.21, as shown in Diagram 11.

![Diagram 10](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/2nd%20model%203.png)


Diagram 10


![Diagram 11](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/2nd%20model%208.png)


Diagram 11


The scatter plot in Diagram 12 shows a clear positive linear trend between cost and the number of tables produced, with 52% of the variation in production costs explained by the number of tables (R² = 0.5204). Similarly, Diagram 13 shows a similar, though weaker, relationship between cost adn the number of fridges produced, with an R² of 0.3711.

However, the scatter plots for costs vs chairs and costs vs doors showed no meaningful pattern. This lack of clear trends confirms their insignificance in predicting production costs. Therefore, the exclusion of these variables guaranteed an improved higher predictive accuracy by focusing on the key drivers of production costs - tables and fridges, as shown in Diagram 14 and 15.

![Diagram 12](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/tables%201.png)


Diagram 12


![Diagram 13](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/fridges%201.png)


Diagram 13


![Diagram 14](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/chairs%201.png)


Diagram 14


![Diagram 15](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/doors%201.png)


Diagram 15

# Model 3: Predicting Sales Performance

Diagram 16 illustrates the relationship between sales for songs and weekly airplays, song attractiveness and advertising expenditure.

![Diagram 16](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/3rd%20model%201.png)


Diagram 16


The original linear regression model has the highest adjusted R² of the three models, at 0.67855, indicating that 67.9% of the variability in sales can be explained by the predictors. Airplays and attractiveness are also highly significant predictors, with pvalues of 0.0117 and 0.0221, respectively. Advertising is also borderline significant with a pvalue of 0.0631. This is illustrated in Diagram 17.

![Diagram 17](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/3rd%20model%202.png)


Diagram 17


The regression equation to predict song sales includes all 3 variables: Sales = 947730 + (52081.98 x airplays per week) + (172677.09 x attractiveness level) + (594.10 x advertising amount), as shown in Diagram 18.

![Diagram 18](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/3rd%20model%206.png)


Diagram 18


The scatter plot of Sales vs Airplays (Diagram 19) illustrates a clear positive linear trend, with an R² of 0.4716, indicating that airplays explain nearly 47.2% of the variation in sales. The relatively tight clustering of data points around the trendline further confirms that airplays are a reliable predictor of sales.

Similarly, the scatter plot of Sales vs Attractiveness (Diagram 20) reveals a positive realtionship, with an R² of 0.4202. This suggests that song attractiveness accounts for 42% of the variation in sales, making it another key factor. While there is some scatter around the trendline, the overall positive trend is still evident, reinforcing the importance of song attractiveness as a predictor.

In contrast, the scatter plot of Sales vs Advertising (Diagram 21) illustrates a much weaker relationship, with an R² of 0.0811, indicating that adverstising expenditure explains only a small portion of sales variation. Further, the wide scatter of data points reflects the borderline significance of this variable, which is why it's contributiion is considered less impactful compared to airplays and attractivess. However, the decision to keep advertising in the model was made based on it's pvalue of 0.0631, suggesting that it may still have a small but relevant influence on sales.


![Diagram 19](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/3rd%20model%203.png)


Diagram 19


![Diagram 20](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/3rd%20model%204.png)


Diagram 20


![Diagram 21](https://github.com/Mojm4321/Excel-Comparative-Analysis-of-Multiple-Regression-Models-for-Forecasting-Costs-and-Sales/blob/main/3rd%20model%205.png)


Diagram 21


# Conclusion

After evaluating all 3 models, Model 3 (Sales Prediction) emerges as the best performing model, with the highest Adjusted R² and strong predictive power from airplays and attractiveness. The scatter plots confirm the strength of these relationships, while advertising plays a smaller role.

Model 2 (Production Costs) is the second best, explaining a significant portion of cost variability using tables and fridges. The scatter plots further validates the model by showing clear trends for these predictors, while chairs and doors were correctly removed.

Model 1 (Taxi Ride Costs), although effective, ranks third due to the prescence of outliers and some unexplained differences in costs, possibly due to facotrs not captured by distance alone. Nevertheless, the model still provides a reliable and simple forecast for taxi ride costs, making it useful for predicting costs based solely on distance travelled.