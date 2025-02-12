# Used Cars Analysis
What drives the price of a car?
## This project sought to analyse a dataset on used cars and inform car dealerships what are the factors of used cars that buyers care about the most.
In other words this can be said as what are the factors that have the highest influence on the price of a car (That affect can be both positive and negative)

## Business Understanding
What factors of used cars do buyers care about the most. What factors will drive the price up and which will bring the price down? Our goal is to answer this question and inform car dealerships information about what people are going to care about most. This can benefit the dealerships in how they source their cars or how they present them in their sale tactics. 

In more mathematical terms, we can boil this understanding down to a simple question. Which features will be the best predictors of the price of a car. 

## Data Understanding
- Begin with importing all relevant libraries and packages
- Read in our vehicles.csv file
- Describe our DataFrame
- Check for null values
- Creation of simple visualizations to understand data
### Features
- region
- price
- year
- manufacturer
- model
- condition
- cylinders
- fuel
- odometer
- title_status
- transmission
- VIN
- drive
- size
- type
- paint_color
- state
  
## Data Preparation 
- Filter DataFrame to eclude outliers from top 1% and lower bound price of $500
- Drop columns=['year', 'VIN', 'id'] Deemed erroneous to price of a car
- Drop null values from the numeric features 'year', 'price', and 'odometer'
- Fill null values with 'unknown' for categorical columns
- Check to make sure all null values have been handled.

## Modeling
- Train test split to split our Data
- Simple Linear Regressions on 'Year' and 'Odometer'
- Multiple linear regression on all our numeric features

## Evaluation
- get_dummies on our categorical columns
- StandardScaler()
- Using PCA and Sequential Feature Selection
- Ridge and Lasso Regressions
- GirdSearchCV to pick hyper-parameters

## Deployment
- Plots to compare actual vs predicted prices

## Conclusion
This analysis allows me to conclude that the two facotrs that consumers care for most in a used car are 'year' and 'odometer' with 'odometer' being the most important. Put mathematically, a cars odometer was the best single factor about that car to predict its price. 

Car dealerships could use this information to better understand how to properly price used cars with relatively low milage. 









