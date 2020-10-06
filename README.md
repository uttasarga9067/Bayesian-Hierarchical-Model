# Bayesian-Hierarchical-Model
#### I] The Prediction Model was developed using SparkR(Azure Databricks to the rescue) and uses the Leinhardt Dataset from the CAR Package in R.

##### About The Data Set

1. The Data set consists of 105 observed values of each of the 4 variables named income, infant mortality rate, region and Oil.
2. We are calculating the infant mortality rate based on the other variables present in the dataset.

![ScreenShot](https://raw.github.com/uttasarga9067/Bayesian-Hierarchical-Model/screenshots/1.PNG)

##### Here is the screenshot for correlation between the variables
![ScreenShot](https://raw.github.com/uttasarga9067/Bayesian-Hierarchical-Model/screenshots-1/2.png)

##### Then, We are taking the log of both the variables (infant mortality and Income) for better and efficient computation.
##### For this model, we are using JAGS (Just another Gibbs Sampler) for efficient sampling of Markov Chains that we create while initializing the Model and passing the data set in the model.
##### Below, we are plotting the convergence of our MCMC chains for the parameters or Co-effecients that we had initialized when building the model.

![ScreenShot](https://raw.github.com/uttasarga9067/Bayesian-Hierarchical-Model/screenshots-1/3.png)
