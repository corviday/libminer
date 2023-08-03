
<!-- README.md is generated from README.Rmd. Please edit that file -->

# libminer

<!-- badges: start -->

[![R-CMD-check](https://github.com/corviday/libminer/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/corviday/libminer/actions/workflows/R-CMD-check.yaml)
<!-- badges: end -->

The goal of libminer is to provide a summary of the user’s R libraries.
It is a toy package developed in a workshop and not meant for serious
use.

## Installation

You can install the development version of libminer from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("corviday/libminer")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(libminer)

lib_summary()
#>                                          library n_packages
#> 1 /home/lzeman/R/x86_64-pc-linux-gnu-library/4.3        108
#> 2     /tmp/Rtmp2yRT0J/temp_libpath3b974a1083b9ac          1
#> 3                             /usr/lib/R/library         29

## you can also ask it to calculate sizes

lib_summary(sizes = TRUE)
#>                                          library n_packages  lib_size
#> 1 /home/lzeman/R/x86_64-pc-linux-gnu-library/4.3        108 219157255
#> 2     /tmp/Rtmp2yRT0J/temp_libpath3b974a1083b9ac          1     41400
#> 3                             /usr/lib/R/library         29  59321890
```
