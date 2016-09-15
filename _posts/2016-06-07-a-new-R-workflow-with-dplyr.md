---
layout: post
title: 'Essential R packages that will dramatically improve your workflow'
description: ""
categories: 
---

R is a fantastic tool for data analysis, and you can take it to the next level by
learning the pipe `%>%` operator and using the packages `dplyr`, `ggplot2`,
`broom` and a few others.

In fact, this toolkit may completely change your R analysis workflow for the
better. That is, your R code will be easier to use, easier to read, easier to
understand (for you and others), and faster to execute.

Instructions to get started, as well as some more detailed tutorials, are near
the bottom, in the **Quick Start**.

Here, I'll show a few *very brief* motivating examples (see the links below for
details). 

You can probably guess what this first snippet is doing:

	iris %>%
        group_by(Species) %>%
        summarise(avg = mean(Sepal.Width)) %>%
        arrange(avg)

We take the `iris` data frame, and use the pipe `%>%` along with a few
functions from `dplyr` to get average Sepal Width, by Species. Last, we sort
the results.

What is the pipe? It's absolutely amazing. The pipe `%>%` "passes the object on
the left hand side as the first argument (or .  argument) of the function on
the right-hand side:"

	x %>% f(y) is the same as f(x, y)

	y %>% f(x, ., z) is the same as f(x, y, z )

Here is another example. Both of the following snippets are equivalent (base R is first). Which
looks easier to write, and understand?

	paste0("(", gsub(".", "_", tolower(names(iris)), fixed=TRUE), ")")

OR:

	names(iris) %>%
		tolower %>%
		gsub(".", "_", ., fixed=TRUE) %>%
		paste0("(", ., ")")

Using the pipe makes the code more readable: we immediately know what's being
analyzed (the names of the `iris` data frame), and the rest of the actions
follow in a logical sequence, arranged for maximum readability.

This syntax also alleviates usage of nested parentheses, which can be hard to
keep track of, even with a good text editor. You will wish something like the
pipe was available in other languages (I SO miss it in
Python... [But see here](https://github.com/dodger487/dplython)).

The package `dplyr` provides a handful of intuitive functions for data
manipulation, like `select`, `filter`, `summarise`, and `mutate`, and works
especially well with the pipe. I can't remember the last time I used `lapply`
or the other base R `*apply` functions. I think that's for the better. Instead,
I use the above new syntax in almost every line of R code I write.

Here is what you need to get started:

## Quick Start

The essential packages are:

* `dplyr` - for data manipulation
* `ggplot2` - for graphics

Highly recommended packages include:

* `tidyr` - for reshaping data (long <-> wide)
* `magrittr` - for advanced "piping" with `%<>%` etc (see below)
* `broom` - for easily combining results from many analyses (eg, regressions)

Install the packages as usual.

The following three resources should get you started quickly. Don't forget about #3:

1. For a more detailed overview of `dplyr`, `magrittr` pipes, `tidyr` and
`ggplot2`, [click here for a post from ZevRoss.com](http://zevross.com/blog/2015/01/13/a-new-data-processing-workflow-for-r-dplyr-magrittr-tidyr-ggplot2/) 
2. Then, to learn `broom` (with `dplyr`),
[take a look at this vignette on CRAN](https://cran.r-project.org/web/packages/broom/vignettes/broom_and_dplyr.html)
3. Finally, [print or save this `dplyr/tidyr` reference PDF from RStudio](https://www.rstudio.com/wp-content/uploads/2015/02/data-wrangling-cheatsheet.pdf)


Here are a few other resources/references:

* Reshaping data from wide to long or vice-versa is a common task, but I was
not satisfied with the docs for `spread` and
`gather`. [So I still refer to this `gather` and `spread` cookbook on cookbook-r.com](http://www.cookbook-r.com/Manipulating_data/Converting_data_between_wide_and_long_format/)
* The basic pipe `%>%` is just the beginning. Learn the rest (including `%<>%` and `%T>%`),
and **see some neat uses of them all** on [the Github page for `magrittr`](https://github.com/smbache/magrittr).
* [Here are more R cheatsheets from RStudio](https://www.rstudio.com/resources/cheatsheets/)
* [Here is the full `broom` vignette on CRAN](https://cran.r-project.org/web/packages/broom/vignettes/broom.html)
* [And here is another post on `dplyr` and pipes](http://seananderson.ca/2014/09/13/dplyr-intro.html)
