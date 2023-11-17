
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
``` r

```
The output provides many information of the mtcars data, such as coefficients, t-statistics, p-value, 95% confidence intervals, F-statistics, degree freedom, R-squared and adjusted-R-squared, etc.
