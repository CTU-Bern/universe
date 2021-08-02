CTU Berns R Package universe
================

R package universes are similar a bit like mini-CRANs. ‘The system
automatically tracks registered git repositories containing R packages,
builds binaries for Windows and MacOS, renders vignettes, and makes all
data available through dashboards, feeds and APIs on personal
subdomains’. [See here for further details of
universes](https://ropensci.org/blog/2021/06/22/setup-runiverse/)

Briefly, packages should be added to [packages.json](packages.json).
They are then tracked on
[r-universe](https://github.com/r-universe/ctu-bern) and built each
hour. A dashboard of the included packages and build status can be found
[here](https://ctu-bern.r-universe.dev/ui#builds). All vignettes are
also accessible via the [articles
button](https://ctu-bern.r-universe.dev/ui#articles).

To use the universe, in R, do the following, which adds the universe to
your list of repos (when installing packages, R will cycle through the
repos until it finds the appropriate package)…

``` r
options(repos = c(CTU = "https://ctu-bern.r-universe.dev",
        CRAN = "https://cran.rstudio.com/"))
```

It is then possible to install universe packages as if they were CRAN
packages…

``` r
install.packages("accrualPlot")
```

## Packages in the universe

| package     | status                                                  |
| :---------- | :------------------------------------------------------ |
| accrualPlot | ![](https://ctu-bern.r-universe.dev/badges/accrualPlot) |
| btabler     | ![](https://ctu-bern.r-universe.dev/badges/btabler)     |
| CTUtemplate | ![](https://ctu-bern.r-universe.dev/badges/CTUtemplate) |
| kpitools    | ![](https://ctu-bern.r-universe.dev/badges/kpitools)    |
| presize     | ![](https://ctu-bern.r-universe.dev/badges/presize)     |
| secuTrialR  | ![](https://ctu-bern.r-universe.dev/badges/secuTrialR)  |
