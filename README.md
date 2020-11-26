
<!-- README.md is generated from README.Rmd. Please edit that file -->

# compareRhythms

<!-- badges: start -->

[![](https://img.shields.io/badge/devel%20version-0.99.0-green.svg)](https://github.com/compareRhythms)
[![License:
GPL-3](https://img.shields.io/badge/license-GPL--3-blue.svg)](https://cran.r-project.org/web/licenses/GPL-3)
[![Travis build
status](https://travis-ci.org/bharathananth/compareRhythms.svg?branch=master)](https://travis-ci.org/bharathananth/compareRhythms)
<!-- badges: end -->

The goal of *compareRhythms* is to find features with altered circadian
rhythm parameters (*amplitude* and *phase*) between the control and
experimental groups.

## Installation

You can install the current version of compareRhythms from GitHub with:

``` r
install.packages("devtools")    # if it is not already installed
devtools::install_github("bharathananth/compareRhythms")
```

## Usage summary

The analysis is run using a single function `compareRhythms()`. To
execute this function, the three necessary ingredients are the
timeseries data, the experimental design and parameters to choose and
tune the method. The output of the function is a *data.frame* with the
IDs of the differentially rhythmic features, the category it is
classified under and optionally the rhythm parameters of the feature in
the two groups. The differential rhythmicity categories are **gain** of,
**loss** of, **change** of, or **same** rhythms (with respect to the
reference/control group).

For complete examples, please refer to the vignette titled **User
Guide** by running

``` r
library(compareRhythms)
vignette("UserGuide", package="compareRhythms")
```
