# actions

Within this repository, we store customized configurations for
[GitHub Actions](https://github.com/features/actions) based off
of the [GitHub Actions for R Language](https://github.com/r-lib/actions). 

For the workflows being used, please see 
[tmsalab/actions/workflow](https://github.com/tmsalab/actions/tree/master/workflows)
directory. 

## Types

To initialize with the appropriate GitHub Actions template, please use the
`usethis` package v1.6.0 or greater. 

### full public repository check matrix

```r
usethis::use_github_action(
  url = "https://raw.githubusercontent.com/tmsalab/actions/master/workflows/R-CMD-check.yaml"
)
```

### private repository check matrix 

```r
usethis::use_github_action(
  url = "https://raw.githubusercontent.com/tmsalab/actions/master/workflows/check-private.yaml", 
  save_as = "R-CMD-check.yaml"
)
```

### pkgdown


```r
usethis::use_github_action(
  url = "https://raw.githubusercontent.com/tmsalab/actions/master/workflows/pkgdown.yaml"
)
```