# Leveraging Gradient Information to Optimise Supervised Learning Model Prediction and Complexity

 ## Approximate Bayesian Computation (ABC) example
[Approximate Bayesian Computation example.ipynb](ABC_example/Approximate%20Bayesian%20Computation%20example.ipynb) demonstrates the method behind ABC using a 1D gaussian as an example process with the mean as a single latent parameter. As the tolerance of accepted samples increases, the posterior `p(θ|x)` density becomes less concentrated around the true value 0 and approachs the uniform prior.  
<img  src="ABC_example/ABC_ex.png" width="340" align="center" />



## Ridge-Gradients regularisation method
[Ridge-Gradients regularisation example.ipynb](Regularising%20regression%20with%20gradients/Ridge-Gradient%20regularisation%20example.ipynb) demonstrates the Ridge-Gradients regularisation method for linear regression. The Ridge-Gradient method levearges derivatives of the target varaible with respect to model inputs to improve model accuracy relative to standard Ridge regularisation. The left figure compares the test RMSE of a linear model fit with OLS with Ridge regularisation and OLS with Ridge-Gradients regularisation over varying training sizes. The right figure shows the percentage difference between the models performance (positive difference indicates Ridge-Gradient method outperfoms).

<img  src="Regularising%20regression%20with%20gradients/beta_versus_betarg_rmse.png" width="340" align="left" />
<img  src="Regularising%20regression%20with%20gradients/beta_versus_betarg_diff.png" width="340" align="left" />

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />

## Leveraging gradients for surrogate modelling 
Full code for all experiments along with saved models can be found in the [public google drive](https://drive.google.com/drive/folders/1J7srZbZPS6UhE43GFXP3Gkd3TmEvT-6f?usp=sharing) **MOVE FOLDERS IN TO PUBLIC**

This repository contains example code that shows how surrogatae training and evaluation was conducted along with latent parameter inference code.
### 2D toy problem
[2D_surrogate_AccTest_nTrain50_EXAMPLE.ipynb](Surrogate%20modelling/2D/2D_surrogate_AccTest_nTrain50_EXAMPLE.ipynb) contains the code used to train and evaluate surrogate model accuracy, comparing the performance of neural networks trained with and without gradients. The results are discussed in Section 3.2 and show gradient trained surrogates are more accurate for small sample sizes and low model complexities. 

<img  src="Surrogate%20modelling/2D/2d_complexity.png" width="340" align="left" />


[MLE and MH latent parameter inference 2D problem.ipynb](Surrogate%20modelling/2D/MLE%20and%20MH%20latent%20paramater%20inference%202D%20problem.ipynb) contains the code used to utilise the surrogate models in an inference pipeline under Maximum likelihood estimation and Metropolis-Hastings sampling. Results are discussed in Section 3.2.2 and principally show improved latent parameter estimation using gradient traing surrogates for small smaple sizes.

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />

<img  src="Surrogate%20modelling/2D/2d_MLE_diff_55.png" width="340" align="left" />
<img  src="Surrogate%20modelling/2D/2d_MH_diff_55.png" width="340" align="left" />

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />

### 4D GARCH problem

## Tuning model complexity
### Determining complexity upper bound
