# Bayesian-Hierarchical-Model
#### I) The Prediction Model was developed using SparkR(Azure Databricks to the rescue) and uses the Leinhardt Dataset from the CAR Package in R.

##### About The Data Set

1. The Data set consists of 105 observed values of each of the 4 variables named income, infant mortality rate, region and Oil.
2. We are calculating the infant mortality rate based on the other variables present in the dataset.

![ScreenShot](https://raw.github.com/uttasarga9067/Bayesian-Hierarchical-Model/screenshots/1.PNG)

##### II) Here is the screenshot for correlation between the variables
![ScreenShot](https://raw.github.com/uttasarga9067/Bayesian-Hierarchical-Model/screenshots-1/2.png)

##### III) Then, We are taking the log of both the variables (infant mortality and Income) for better and efficient computation.
##### IV) For this model, we are using JAGS (Just another Gibbs Sampler) for efficient sampling of Markov Chains that we create while initializing the Model and passing the data set in the model.
##### V) Below, we are plotting the convergence of our MCMC chains for the parameters or Co-effecients that we had initialized when building the model.

![ScreenShot](https://raw.github.com/uttasarga9067/Bayesian-Hierarchical-Model/screenshots-1/3.png)

The Convergence diagnostics are great as the Hierarchical regression model converged each co-eeficients that we are using for our Model.
In the Below screenshots, you can see that the results from the model are predicted and stored in a vector format (y_hat). The Infant mortality rate(data1_jags$y) is predicted 92% to be accurate with our model prediction which means that the Infant mortatlity is dependent on the Income of the Families while looking at the geographical factors such as country, state or zip for much refined details.

![ScreenShot](https://raw.github.com/uttasarga9067/Bayesian-Hierarchical-Model/screenshots-1/4.PNG)



![ScreenShot](https://raw.github.com/uttasarga9067/Bayesian-Hierarchical-Model/screenshots-1/5.PNG)
