
# linearregression

<!-- badges: start -->
[![R-CMD-check](https://github.com/MiaojinHu/biostat625hw3/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/MiaojinHu/biostat625hw3/actions/workflows/R-CMD-check.yaml)
[![Codecov test coverage](https://codecov.io/gh/MiaojinHu/biostat625hw3/branch/main/graph/badge.svg)](https://app.codecov.io/gh/MiaojinHu/biostat625hw3?branch=main)
<!-- badges: end -->

The linearregression R package is designed to calculate data related to linear regression. Providing with dataframe, dependent variable, and covariates, it will return a list including residuals, coefficients, 95% confidence intervals, degree of freedom, t-statistics, F-statistic values, and p-values, etc. 

## Installation

You can install the development version of linearregression from [GitHub](https://github.com/MiaojinHu/biostat625hw3), with the following code:
``` r
# install.packages("devtools")
devtools::install_github("MiaojinHu/biostat625hw3")
```

## Example

This is a basic example which shows you how to solve a common problem:
The mtcars are the data we want to explore, the mpg is the variable name of the outcome, the cyl, disp, and hp are the covariates names.

``` r
library(linearregression)
data(mtcars)
result=linear_regression_function(mtcars, "mpg", c("cyl","disp","hp"))
result
```

The output will be a list containing following information:

<img width="442" alt="1" src="https://user-images.githubusercontent.com/149199735/283658356-87edaa33-d137-49c5-aaeb-9594fb284dbd.png">

<img width="397" alt="2" src="https://user-images.githubusercontent.com/149199735/283658372-ff72e6fb-cf7a-4f97-8e8b-b9a9fb27861b.png">

<img width="517" alt="3" src="https://user-images.githubusercontent.com/149199735/283658384-76497cae-a4c2-4762-b23f-c236779dab96.png">

The first image provides information of residuals standard error, F-statistics, p-value of F statistics, degree freedom, R-squared and adjusted-R-squared.
The second image provides information of residuals.
The third image provides information of coefficients, including estimates, standard error of estimates, 95% confidence intervals, t-statistics, and p-value. 
