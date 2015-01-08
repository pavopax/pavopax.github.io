---
layout: post
title: '"Summary Statistics Obscure Important Details"'
description: ""
categories: 
---

[Boston Data Festival was this week](http://www.bostondatafest.com), packed with excellent talks on topics from "Quantifying Culture" to "Evaluating Trading Algorithms Using Probabilistic Programming." 

And while the focus in data science today seems to be on big data and novel methods like "deep learning," David Weisman, a 30-year veteran of the field, decided to focus on the basics during his presentation on Friday night.

Here are David's fundamental principles to keep in mind:  

* Summary statistics (mean, median, correlation) obscure important details   

* Small samples have high variance  

* When looking at your (observed) data, also think about unobserved data  

* Correlation is a summary statistic itself, and only measures ONE type of relationship  

* Big data can increase spurious corrleations  

Regarding the first point, researchers often summarize data to uncover patterns (even a regression is a summary, David pointed out). But quantifying the variance (spread) of the data is equally important - and that is why graphical summaries are so critical (boxplot with overlaid jitter plot is my favorite).

Further, large effect sizes must be considered with caution, especially when they come from small sample sizes. The latter tend to have high variance - increasing the possibility that the effects are misleading.

Last, to illustrate how big data can show spurious correlation (and the need for careful thinking and analysis), David recommended this amusing collection:  

[http://tylervigen.com](http://tylervigen.com)  
*Don't forget to ["Discover a New Correlation"](http://tylervigen.com/discover)*



### References
David's slides include an excellent set of exercises to help you "think about your data." [They are available from the Boston Data Festitval website, under "Friday"](http://www.bostondatafest.com/slides/).

[David recommended Judea Pearl's work to learn about causality](http://bayes.cs.ucla.edu/jp_home.html)

Also check out [this article from Science Magazine](http://gking.harvard.edu/publications/parable-google-flu%C2%A0traps-big-data-analysis) where the authors also emphasize balancing the new with the tried and tested. 


Andrew Gelman from Columbia on large effects:
> For instance it is not uncommon in an underpowered study for a researcher to state that although his estimate is not statistically significantly different from 0, that could simply be a function of the overly large standard error. <b>Ironically, however, large estimates are actually a byproduct of large standard errors.</b> [Emphasis added]  

From ["Why We (Usually) Don’t Have to Worry About Multiple Comparisons" (Gelman, Hill, Yajima, 2009), p. 7](http://arxiv.org/abs/0907.2478)



