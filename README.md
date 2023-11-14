
# linearregression

<!-- badges: start -->
[![R-CMD-check](https://github.com/MiaojinHu/biostat625hw3/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/MiaojinHu/biostat625hw3/actions/workflows/R-CMD-check.yaml)
[![Codecov test coverage](https://codecov.io/gh/MiaojinHu/biostat625hw3/branch/main/graph/badge.svg)](https://app.codecov.io/gh/MiaojinHu/biostat625hw3?branch=main)
<!-- badges: end -->

The linearregression R package is designed to compute data related to linear regression. Providing with a dataframe, dependent variable, and covariates, it will return a list including residuals, coefficients, degrees of freedom, t/F statistic values, and p-values, among others. 

## Installation

You can install the development version of linearregression from [GitHub](https://github.com/MiaojinHu/biostat625hw3), with the following code:
``` r
# install.packages("devtools")
devtools::install_github("MiaojinHu/biostat625hw3")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(linearregression)
data(mtcars)
result=linear_regression_function(mtcars, "mpg", c("cyl","disp","hp"))
result
```

