
<!-- README.md is generated from README.Rmd. Please edit that file -->

# `{coreview}`

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
<!-- badges: end -->

## Installation

You can install the development version of `{coreview}` like so:

``` r
# (Only necessary if the remotes package is not installed).
utils::install.packages("remotes")
```

``` r
remotes::install_github("MUHEG/coreview")
```

## Run

You can launch the application by running:

``` r
coreview::run_app()
```

## About

You are reading the doc about version : 0.0.0.9000

This README has been compiled on the

``` r
Sys.time()
#> [1] "2026-10-08 13:09:41 AEDT"
```

Here are the tests results and package coverage:

``` r
devtools::check(quiet = TRUE)
#> ══ Documenting ═════════════════════════════════════════════════════════════════
#> ℹ Installed roxygen2 version (7.3.3) doesn't match declared (7.1.1)
#> ✖ `check()` will not re-document this package.
#> ℹ Do you need to re-run `document()`?
#> ── R CMD check results ──────────────────────────────── coreview 0.0.0.9000 ────
#> Duration: 1m 2.9s
#> 
#> ❯ checking for future file timestamps ... NOTE
#>   unable to verify current time
#> 
#> ❯ checking top-level files ... NOTE
#>   File
#>     LICENSE
#>   is not mentioned in the DESCRIPTION file.
#> 
#> 0 errors ✔ | 0 warnings ✔ | 2 notes ✖
```

``` r
covr::package_coverage()
#> coreview Coverage: 0.00%
#> R/app_config.R: 0.00%
#> R/app_ui.R: 0.00%
#> R/run_app.R: 0.00%
```
