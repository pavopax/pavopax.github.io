---
layout: post
title: 'Which Wilcoxon test to use?'
description: ""
categories: 
---

Wilcoxon rank sum? Wilcoxon signed rank? Wilcoxon one-sample? Two sample?
Mann-Whitney U? If you are confused, read on.

All of these are basically non-parametric versions of the t-test.

That is, you want to check if two groups of numbers have a similar
distribution/center (without the normal distribution assumption in a t-test).

Here is a quick guide that I made for myself (and you!):

# Wilcoxon rank sum (same as "Mann–Whitney U test")

Basically, like your standard t-test to compare two samples from two
*different* populations.

In R:

	wilcox.test(df$X, df$Y)   # both numeric
	wilcox.test(y ~ A)        # A is a group/factor


# Wilcoxon signed-rank

Use when comparing two related samples, matched samples, or repeated
measurements on a single sample.

In R:

	wilcox.test(df$Y1, df$Y2, paired=TRUE) 
   
# MoRe

A handy R reference for this:

[www.statmethods.net/stats/nonparametric.html](https://www.statmethods.net/stats/nonparametric.html)
