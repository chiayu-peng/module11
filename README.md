# Car Price Analysis
**Report Summary**

The following steps are performed in this notebook:
- Defined business problem: to find which features in used cars are the most relevant in determining price, to help fine-tuning dealers' inventory
- Loaded `vehicle.csv` and performed exploratory data analysis
- Narrowed down and cleaned data
- Created a ridge regresion model and a LASSO regression model to predict car prices based on seleceted features
- Chose the ridge regression model, with Train MSE of 0.3778 and Test MSE of 0.3742, at alpha = 100
- Interpreted the resulting coefficents. The most important factors affecting the used car price are age (`year`) and mileage (`odometer`) of cars, followed by other features such as car types and manufacturers. Newer cars are priced higher, and cars with more mileage are priced lower. Types of cars also influence the prices, for example, trucks would be priced higher than sedans. Cars from certain manufactueres are also valued more than others. Positive coefficents denote features increasing car prices, whereas negative coefficients denote features decreasing car prices
- Suggested possible next step, which is to factor actual sales data to improve the model performance
