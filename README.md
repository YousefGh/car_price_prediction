# Car Price Prediction (Simple Regression)

## Outline
- Introduction
- Setup Environment
- Load Data
- Data Analysis (Quality Check)
- Data Analysis (General)
- Data Analysis (Hypothesis-Wise)
- Feature Selection
- Modeling
- Evaluation
	- MAE: Used for robustness against outlier errors
	- MSE: Used to penalize all range of error values
	- Residual Plot: Used to make sure no pattern appears in the error variance within the range


## Intorduction
**Quick Notes:** 
- No metadata was offered. 
- → symbol means a developer's conversion is needed

Our goal in this project is to predict the selling_price, our response variable, using the best explantory or independant variable/s. For that, an assumption is made: One or more of the variables present can be a predictor of the price. One problem is that the data is scarce and thus, might not represents the actual distribution. Hence, train/test split will not be done before analysis (A rigorous technique to validate model's quality).

**Target Value:**

- selling_price (Continuous Float)

**Features:**

- year (Float → Ordinal but can be scaled immediately)
- mileage (Discrete Integer)
- fueltype (String → ternary Nominal)_
- sellertype (String → Binary Nominal)_
- transmissiontype (String → Binary Nominal)_
- previousowners (Discrete Integer)_