# companies-bankruptcy-forecast
## Todo list / Plan

* Combine  Surrogate and Bayesian GLM for interpretability:
 - Combine Surrogtae Decision Tree with pd/ROPE
 - https://cran.r-project.org/web/packages/iml/vignettes/intro.html
 
* Use XGBOOST and GBM
* Expand using other Credit default data


- [ ] Fit Bayesain regression with all variables : Student-t prior and defaults
    - [x] [Use Bayes Rqaured metric] (https://avehtari.github.io/ROS-Examples/Rsquared/rsquared.html) to test the goodness fit
    - [ ] Change the variables

- [x ] Run plain logistic regression
    - [ ] Do causal inference

- [ ] Run Bayesian regression with bayesian variable selected covariates/predictors

- [ ] Run Bayesian regression with covariates/predictors suggested by expert

## Ideas:
* Combine Bayesian Coresets (to reduce 'n') with projpred (to reduce 'p')
    * Generate Bayesian coresets
    * Do Bayesian variable selection using projpred from reduced Bayeisan Coresets
    * Run GLM on reduced n and reduced p
    * Generate minimum error bound!!
 