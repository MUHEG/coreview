
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
#> [1] "2026-10-09 17:29:27 AEDT"
```

Here are the tests results and package coverage:

``` r
devtools::check(quiet = TRUE)
#> Writing 'NAMESPACE'
#> ℹ Loading coreview
#> Writing 'NAMESPACE'
#> Writing 'combine_reviewed.Rd'
#> Writing 'split_for_review.Rd'
#> ── R CMD check results ──────────────────────────────── coreview 0.0.0.9000 ────
#> Duration: 1m 28.8s
#> 
#> ❯ checking code files for non-ASCII characters ... WARNING
#>   Found the following file with non-ASCII characters:
#>     R/mod_coreview_main.R
#>   Portable packages must use only ASCII characters in their R code and
#>   NAMESPACE directives, except perhaps in comments.
#>   Use \uxxxx escapes for other characters.
#>   Function 'tools::showNonASCIIfile' can help in finding non-ASCII
#>   characters in files.
#> 
#> ❯ checking dependencies in R code ... WARNING
#>   '::' or ':::' imports not declared from:
#>     'jsonlite' 'openxlsx' 'readxl'
#> 
#> ❯ checking Rd cross-references ... WARNING
#>   Missing link or links in Rd file 'combine_reviewed.Rd':
#>     'run_review_app'
#>   
#>   Missing link or links in Rd file 'split_for_review.Rd':
#>     'run_review_app'
#>   
#>   See section 'Cross-references' in the 'Writing R Extensions' manual.
#> 
#> ❯ checking for future file timestamps ... NOTE
#>   unable to verify current time
#> 
#> ❯ checking top-level files ... NOTE
#>   File
#>     LICENSE
#>   is not mentioned in the DESCRIPTION file.
#> 
#> ❯ checking package subdirectories ... NOTE
#>   Problems with news in 'NEWS.md':
#>   No news entries found.
#> 
#> ❯ checking R code for possible problems ... [14s] NOTE
#>   build_extraction_workbook: no visible global function definition for
#>     'createWorkbook'
#>   build_extraction_workbook: no visible global function definition for
#>     'addWorksheet'
#>   build_extraction_workbook: no visible global function definition for
#>     'writeData'
#>   build_extraction_workbook: no visible global function definition for
#>     'addStyle'
#>   build_extraction_workbook: no visible global function definition for
#>     'setColWidths'
#>   build_qa_workbook: no visible global function definition for
#>     'createWorkbook'
#>   build_qa_workbook: no visible global function definition for
#>     'addWorksheet'
#>   build_qa_workbook: no visible global function definition for
#>     'writeData'
#>   build_qa_workbook: no visible global function definition for 'addStyle'
#>   build_qa_workbook: no visible global function definition for
#>     'setColWidths'
#>   build_record: no visible global function definition for 'setNames'
#>   build_rows: no visible global function definition for 'setNames'
#>   red_fill: no visible global function definition for 'createStyle'
#>   Undefined global functions or variables:
#>     addStyle addWorksheet createStyle createWorkbook setColWidths
#>     setNames writeData
#>   Consider adding
#>     importFrom("stats", "setNames")
#>   to your NAMESPACE file.
#> 
#> 0 errors ✔ | 3 warnings ✖ | 4 notes ✖
#> Error:
#> ! R CMD check found WARNINGs
```

``` r
covr::package_coverage()
#> coreview Coverage: 53.97%
#> R/combine_logic.R: 0.00%
#> R/combine_reviewed.R: 0.00%
#> R/extraction_definitions.R: 0.00%
#> R/qa_definitions.R: 0.00%
#> R/run_app.R: 0.00%
#> R/split_for_review.R: 0.00%
#> R/review_io.R: 4.00%
#> R/mod_coreview_main.R: 49.82%
#> R/app_config.R: 100.00%
#> R/app_server.R: 100.00%
#> R/app_ui.R: 100.00%
#> R/golem_utils_server.R: 100.00%
#> R/golem_utils_ui.R: 100.00%
```
