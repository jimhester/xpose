
ggxpose <a href="https://guiastrennec.github.io/ggxpose/"><img src="logo.png" align="right" /></a>
==================================================================================================

[![build\_status](https://travis-ci.org/guiastrennec/ggxpose.svg?branch=master)](https://travis-ci.org/guiastrennec/ggxpose) [![app\_veyor](https://ci.appveyor.com/api/projects/status/3w06ve94gne2xg91?svg=true)](https://ci.appveyor.com/project/guiastrennec/ggxpose) [![cran\_version](http://www.r-pkg.org/badges/version/ggxpose)]() [![codecov](https://codecov.io/gh/guiastrennec/ggxpose/branch/master/graph/badge.svg)](https://codecov.io/gh/guiastrennec/ggxpose)

### Overview

[ggxpose](https://guiastrennec.github.io/ggxpose/) was designed as a [ggplot2](https://github.com/tidyverse/ggplot2)-based alternative to [xpose4](http://xpose.sourceforge.net). ggxpose aims to reduce the post processing burden and improve diagnostics commonly associated the development of non-linear mixed effect models.

### Installation

Install the development version from github

``` r
# install.packages('devtools')
devtools::install_github('guiastrennec/ggxpose')
```

### Getting started

Load ggxpose

``` r
library(ggxpose)
```

Import run output

``` r
xpdb <- xpose_data(runno = '001')
```

Generate diagnostics

``` r
# DV vs. IPRED plot
dv_vs_ipred(xpdb)
```

<img src="inst/img/readme_example_figure-1.png" width="50%" style="display: block; margin: auto;" />

``` r
# CWRES vs. PRED plot
cwres_vs_pred(xpdb)
```

<img src="inst/img/readme_example_figure-2.png" width="50%" style="display: block; margin: auto;" />

### Recommended reading

The [ggxpose website](https://guiastrennec.github.io/ggxpose/) contains several useful articles to make full use of ggxpose

When working with ggxpose, a working knowledge of ggplot2 is recommended. Help for ggplot2 can be found in:

-   The ggplot2 [documentation](http://docs.ggplot2.org/current/)
-   The ggplot2 [mailing list](https://groups.google.com/forum/?fromgroups#!forum/ggplot2)
-   Internet resources (stack overflow, etc.)
