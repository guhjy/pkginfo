
<!-- README.md is generated from README.Rmd. Please edit that file -->

# pkginfo

> Tools for retrieving package
information

[![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/pkginfo)](https://cran.r-project.org/package=pkginfo)
[![Travis-CI Build
Status](https://travis-ci.org/rsquaredacademy/pkginfo.svg?branch=master)](https://travis-ci.org/rsquaredacademy/pkginfo)
[![AppVeyor Build
Status](https://ci.appveyor.com/api/projects/status/github/rsquaredacademy/pkginfo?branch=master&svg=true)](https://ci.appveyor.com/project/aravindhebbali/pkginfo)
![](https://img.shields.io/badge/lifecycle-experimental-orange.svg)

## Installation

You can install the development version from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("rsquaredacademy/pkginfo")
```

## Usage

#### Download Statistics

``` r
get_cran_downloads("olsrr")
#> # A tibble: 1 x 4
#>   latest last_week last_month total
#>    <dbl>     <dbl>      <dbl> <dbl>
#> 1    160       989       3915 35465
```

#### Travis Build Status

``` r
get_status_travis("olsrr", "rsquaredacademy")
#> [1] "Success"
```

#### Appveyor Build Status

``` r
get_status_appveyor("olsrr", "rsquaredacademy")
#> [1] "success"
```

#### Code Coverage

``` r
get_code_coverage("olsrr", "rsquaredacademy")
#> [1] "84.42623"
```

#### GitHub Statistics

``` r
get_gh_stats("olsrr", "rsquaredacademy")
#> # A tibble: 1 x 3
#>   stars issues forks
#>   <int>  <int> <int>
#> 1    59      4    10
```

## Community Guidelines

Please note that this project is released with a [Contributor Code of
Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree
to abide by its terms.
