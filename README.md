# Research project working repository

** This repository is a work in progress **

 ## Approximate Bayesian Computation (ABC) example
[Approximate Bayesian Computation example.ipynb](ABC_example/Approximate%20Bayesian%20Computation%20example.ipynb) demonstrates the method behind ABC using a 1D gaussian as an example process with the mean as a single latent parameter. As the tolerance of accepted samples increases, the posterior `p(θ|x)` density becomes less concentrated around the true value 0 and approachs the uniform prior.  
<img  src="ABC_example/ABC_ex.png" width="340" align="right" />


## Ridge-Gradients regularisation method
[Ridge-Gradients regularisation example.ipynb](Regularising%20regression%20with%20gradients/Ridge-Gradient%20regularisation%20example.ipynb) demonstrates the Ridge-Gradients regularisation method for linear regression. The Ridge-Gradient method levearges derivatives of the target varaible with respect to model inputs to improve model accuracy relative to standard Ridge regularisation. The left figure compares the test RMSE of a linear model fit with OLS with Ridge regularisation and OLS with Ridge-Gradients regularisation over varying training sizes. The right figure shows the percentage difference between the models performance (positive difference indicates Ridge-Gradient method outperfoms).
<img  src="Regularising%20regression%20with%20gradients/beta_versus_betarg_rmse.png" width="340" align="left" />
<img  src="Regularising%20regression%20with%20gradients/beta_versus_betarg_diff.png" width="340" align="right" />

## Leveraging gradients for surrogate modelling 
### 2D toy problem
### 4D GARCH problem
