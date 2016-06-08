---
layout: post
title: 'Essential R packages that will dramatically improve your workflow'
description: ""
categories: 
---

R is fantastic, and you can take it to the next level by learning the R
packages `dplyr`, `ggplot`, `broom` and a few others, and the pipe `%>%`
operator.

In fact, this toolkit may completely change your R analysis workflow for the better: that
is, your R code will be easier to use, easier to read, easier to understand
(for you and others), and faster to execute.

The essential packages are:

* `dplyr` - for data manipulation
* `ggplot2` - for graphics

Highly recommended additions include:

* `tidyr` - for reshaping data (long <-> wide)
* `magrittr` - for advanced "piping" with `%<>%` etc (see below)
* `broom` - for easily combining results from many analyses (eg, regressions)

To get started, take a look at these three resources:

1. For a quick start on `dplyr`, `magrittr` pipes, `tidyr` and
`ggplot`, [click here for a post from ZevRoss.com](http://zevross.com/blog/2015/01/13/a-new-data-processing-workflow-for-r-dplyr-magrittr-tidyr-ggplot2/) 
2. Then, to learn `broom` (with `dplyr`),
[take a look at this vignette on CRAN](https://cran.r-project.org/web/packages/broom/vignettes/broom_and_dplyr.html)
3. Finally, [print or save this reference PDF on dplyr and tidyr, from RStudio](https://www.rstudio.com/wp-content/uploads/2015/02/data-wrangling-cheatsheet.pdf)

There are many fantastic posts showing you the essentials, so instead of
re-creating the wheel, I simply link to the above. 

You are most likely already using `ggplot` and probably have heard of the pipe
and `dplyr`. `broom` and the compound operator may be less well-known.  Now is
the time to finally embrace them all.

A few other resources/references follow:

* Reshaping data from wide to long or vice versa is a common task, but I was
not satisfied with the docs for `spread` and
`gather`. [So I still refer to this `gather` and `spread` cookbook on cookbook-r.com](http://www.cookbook-r.com/Manipulating_data/Converting_data_between_wide_and_long_format/)
* The basic pipe `%>%` is just the beginning. Learn the rest (including `%<>%` and `%T>%`),
and **see some neat uses of them all** on [the Github page for `magrittr`](https://github.com/smbache/magrittr).
* [Here are more R cheatsheets from RStudio](https://www.rstudio.com/resources/cheatsheets/)
* [Here is the full `broom` vignette on CRAN](https://cran.r-project.org/web/packages/broom/vignettes/broom.html)
* [And here is another post on `dplyr` and pipes](http://seananderson.ca/2014/09/13/dplyr-intro.html)
