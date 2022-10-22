# Linear Regressions

## Reading:
### Linear Regression:
- Linear regression is a basic and commonly used type of predictive analysis.These regression estimates are used to explain the relationship between one dependent variable and one or more independent variables.  The simplest form of the regression equation with one dependent and one independent variable is defined by the formula y = c + b*x, where y = estimated dependent variable score, c = constant, b = regression coefficient, and x = score on the independent variable.
- The overall idea of regression is to examine two things:
1. Does a set of predictor variables do a good job in predicting an outcome (dependent) variable?
2. Which variables in particular are significant predictors of the outcome variable, and in what way do they–indicated by the magnitude and sign of the beta estimates–impact the outcome variable?

### Uses of Regression Analysis:
1. Determining the strength of predictors
2. Forecasting an effect
3. Trend forecasting

### Types of Linear Regression:
1. Simple Linear Regression
2. Multiple Linear Regression
3. Logistic regression
4. Ordinal regression
5. Multinomial regression
6. Discriminant analysis

### Linear Regression in Python:
- There are five basic steps when you’re implementing linear regression:
1. Import the packages and classes you need.
2. Provide data to work with and eventually do the regression.
3. Create a regression model and fit it with existing data.
4. Check the results of model fitting to know whether the model is satisfactory.
5. Apply the model for predictions.

### Train & Test Splits:
- Overfitting means that model we trained has trained “too well” and is now, well, fit too closely to the training dataset. This usually happens when the model is too complex (i.e. too many features/variables compared to the number of observations). This model will be very accurate on the training data but will probably be very not accurate on untrained or new data.
- Underfitting means that the model does not fit the training data and therefore misses the trends in the data. It also means the model cannot be generalized to new data. As you probably guessed (or figured out!), this is usually the result of a very simple model (not enough predictors/independent variables).