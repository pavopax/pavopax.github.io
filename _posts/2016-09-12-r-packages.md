---
layout: post
title: 'Popular R packages (latest)'
description: ""
categories: 
---

I'm keeping a list of R packages for a variety of applications. 

The goal is to keep this list fresh. Therefore, I exclude older versions of
packages which have been replaced (eg, I exclude `reshape2` in favor of the
newer `tidyr`).

Naturally, there is a preference for [Hadley's](http://hadley.nz) packages.

If you only want the essentials, then this is my list:  
`dplyr, tidyr, magrittr, ggplot2`

Let me [know what you think!](http://twitter.com/pavopax)

# Data wrangling
- dplyr
- tidyr
- magrittr

# Special data wrangling
- lubridate for dates
- stringr for strings
- httr - pulling data from APIs
- matrix [Sparse and Dense Matrix Classes and Methods]

# Load data
- haven - for SAS, SPSS (replaces foreign)

# Vis, graphics
- ggplot2
- lattice
- rCharts
- RColorBrewer - colors


# Vis apps
- Shiny
- ggvis
- manipulate! (RStudio only?)


# Machine learning - general
- modelr
- caret
- gmodels

# Machine learning - specific
- vcd - Visualization tools and tests for categorical data
- glm
- glmnet [Lasso and Elastic-Net Regularized Generalized Linear Models]
- randomforest
- e1071 for SVM
- gbm - gradient boosting machine
- zoo for time series

# Parallelization
- doMc
- doParallel

# Development
- devtools - An essential suite of tools for turning your code into an R package.
- testthat - provides an easy way to write unit tests for your code projects.
- roxygen2 - A quick way to document your R packages. roxygen2 turns inline code comments into documentation pages and builds a package namespace.

# Other
- Rcpp
- digest for hash digests (?)
