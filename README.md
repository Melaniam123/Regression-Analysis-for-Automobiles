# Regression-Analysis-for-Automobiles
Determine which attributes may contribute to higher gas mileage to design a more fuel-efficient automobile

# Introduction 

In the study of linear regression, we have analyzed the case study of a car manufacturer known
for making automobiles struggling with sales. Using the data, the analysis will determine which
attributes may contribute to higher gas mileage to design a more fuel-efficient automobile.
Linear Regression is an algorithmic technique used for statistical modeling helpful in qualifying a
relationship between a dependent and one or more than one independent variable represented
in a single line where the goal is to find the best fitting line that establishes a linear relationship
minimizing the difference between observed and predicted values. The study will elaborate on
three parts: Data cleaning techniques, building a linear regression model to predict miles per
gallon (MPG), and optimizing the model.

# Background 
The automobile industry is always evolving, for eg: self-driving cars, tire revolving
capabilities, etc. Due to the significant transformation, environmental sustainability is becoming
increasingly important for consumers and manufacturers. Due to the ongoing global warming,
and scarcity of fuel, car manufacturers are seeking ways to design automobiles by leaning
towards sustainability practices and greener technologies. In the context of this project, we aim
to assist the car manufacturer by leveraging sales data and determining the highest contributing
attribute to gas mileage.

# Problem Statement
The car manufacturer is struggling with sales and requires assistance in designing an
energy-efficient car. Using the data gathered, we can determine which attributes would
contribute to higher gas mileage to design a more fuel-efficient automobile.

# Problem Solution
We will build a linear regression model to accurately predict miles per gallon (MPG)
based on the attributes of a vehicle and observe significant attributes to help build proper cars.

# Methodology
The accuracy of the model will be the key metric to evaluate the reliability and
effectiveness of the model using Ordinary least squares Linear Regression. Higher the accuracy
rate, the more reliable the model can be to correctly classify individuals into the appropriate
income category. By identifying other attributes, policymakers can insights into which factors
have a significant influence on income and understand the factors that may or may not be
contributing to income disparity.

# Exploratory Data Analyis

The data comprised of 398 entries, with a total of 8 data columns which include
cylinder, displacement, horsepower, weight, acceleration, model year, US make including float,
and objects.

Some quick notes
1) The outlier% for the critical columns depicts that Horsepower and Acceleration
have relatively a slightly higher correlation percentage than the rest.
2) Horsepower was the only categorical variable in the data while the rest were numerical.
We converted US Made to Categorical variable 1, representing US Made, and 0 representing
Non-US Made.
3) Obbserved distribution of the Accelerator attribute is uniformly distributed while the
rest have a varied distribution. Acceleration has a distinct set of outliers compared to the other attributes.
4) Attributes such as Horsepower, Displacement and Weight have higher correlation as compared to the other attributes Hence we, further
evaluate their VIF variance inflation factor for multicolinearity. Multicollinearity can be a
problem in a regression model when using algorithms such as OLS (ordinary least squares) in
statsmodels. This is because the estimated regression coefficients become unstable and difficult
to interpret in the presence of multicollinearity (Bhandari, 2023). When multicollinearity is present, the estimated regression coefficients may become large and unpredictable, leading to unreliable inferences about the effects of the predictor variables on
the response variable and hence, it is important to check for multicollinearity and consider
using other regression techniques that can handle this problem, such as ridge regression or
principal component regression (Bhandari, 2023).

![image](https://github.com/Melaniam123/Regression-Analysis-for-Automobiles/assets/97692152/98d93976-c5fb-4d1d-a0fc-f1f0a6d4daf3)
![image](https://github.com/Melaniam123/Regression-Analysis-for-Automobiles/assets/97692152/7b805052-6d9f-41d3-b143-cfd34c785f52)
![image](https://github.com/Melaniam123/Regression-Analysis-for-Automobiles/assets/97692152/f379f36c-66c0-40d5-8dbf-d0a78d45436a)
![image](https://github.com/Melaniam123/Regression-Analysis-for-Automobiles/assets/97692152/2ddadb5a-b3c4-40f3-beb2-f2ee04fcdae5)






# Model Summary 
1. R-squared: The R^square is 0.750 meaning that approximately 75% of the attribute MPG
variability can be explained by the independent variables since the coefficient of
determination measures the proportion of the variance in the dependent variables.
2. Adjusted R-squared: The adjusted R-squared is 0.746 which penalizes the effect of
other variables.
3. F-statistic: The F-statistic is 204.6, and Prob (F-statistic) seems to be very close to zero at
7.16e-81, indicating the statistical significance of the model.
4. Coefficients: The estimated coefficients for each independent variable, along with their
standard errors, t-values, and p-values.
5. Confidence intervals: With the 95% confidence interval we can be confident that the
true population value lies.
6. Omnibus, Prob, Jarque-Bera, Skewness, and Kurtosis: The Prob(Omnibus) and Prob(JB)
values seem low, which indicates that the residuals may not be normally distributed.
7. Durbin-Watson: Durbin-Watson's value of 1.859 indicates that there is little or no
autocorrelation present in the residuals.



![image](https://github.com/Melaniam123/Regression-Analysis-for-Automobiles/assets/97692152/8004fec5-faf4-4bce-be67-239b9acd7b9a)

![image](https://github.com/Melaniam123/Regression-Analysis-for-Automobiles/assets/97692152/3b9f8823-c1b0-43bf-bd7a-3494f3654ea9)


# Conclusion 

The results suggest that the independent variables included in the model which are
Horsepower, Acceleration, Model Year, US Made 0, and US Made 1) have a significant
relationship with the dependent variable (MPG). In our analysis, the coefficients indicate the
direction and magnitude of the relationships, while the p-values suggest that the relationships
are statistically significant.
Among the other included attributes in the data - Horsepower, Acceleration, Model Year,
US Made_0, and US Made_1 are identified as significant contributors to generating a higher
MPG. Positive coefficients of Model Year, US Made_0, and US Made_1 indicate that newer
model years and vehicles made in the US tend to have higher MPG. While the presence of the
negative coefficient of Horsepower in the summary indicates that higher horsepower is
associated with lower MPG and the negative coefficient of Acceleration implies that faster
acceleration is linked to lower MPG.

