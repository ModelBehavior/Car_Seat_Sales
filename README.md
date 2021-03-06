# [Project 1: Car Seats Cost What!?](https://github.com/ModelBehavior/Car_Seat_Sales/blob/main/Project1.Rmd)
## Regression Analysis of Car Seat Sales
### Questions:
- What is the relationship between Sales and Price?
- Can we explain car seat sales by Price, urban(YES or NO), and US(YES or NO)?
- What can we tell from the coefficients of the model?
- Can any predictors be removed from the model?
- How well can this model predict sales?
- Can this model be extended (can we improve this analysis)?
### Data:
The data used for this project comes from the ISLR package. There are 400 observations and 11 variables. 3 of which are factors, and the other 8 are numeric.
### Methods and Results:
Regression analysis with Sales as the response and Price, Urban and the US as the explanatory variables. 
10-fold Cross-validation to see how well the model will fit new data using RMSE as the metric.
I dropped the Urban variable because of its non-significance in the model.
Residual plots to check assumptions of the linear model.
From the coefficients, we can conclude that the average unit sales among stores not in the US are 13.031.
The average car seat sales among stores in the US is 1200 units higher than stores not in the US.
With all other variables held constant, on average sales will fall by roughly 54 seats for every $1 increase in price.
Using 10-fold cross-validation, we have an average RMSE of 2.4478658, which means we can expect our predictions to be off by 2.4478658 on average when applied to a new set of data.

![](https://github.com/ModelBehavior/Shawn_Portfolio/blob/main/images/project1_image)

### Limitations and Next Steps:
This analysis only included 2 explanatory variables out of 10. It could be possible for this analysis to give different or better results using more or varying subsets of the explanatory variables, such as the income variable.
