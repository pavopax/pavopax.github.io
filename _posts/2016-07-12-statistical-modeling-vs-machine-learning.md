---
layout: post
title: 'Distinguishing between statistical modeling and machine learning'
description: ""
categories: 
---

If you are looking for it, here is one framework to distinguish statistical
modeling from machine learning, and it is based on the desire for **interpretability**.

In summary, if you want to understand a model, and value interpretability, you
are interested in model inference, and therefore are performing **statistical
modeling**. If all you care about are accurate predictions, and not the
interpretability of a model, you are doing **machine learning**.

	statistical modeling <- interested in model inference/understanding a model
	machine learning <- interested in accurate predictions

## Examples

Take two examples. If you want to understand a medical condition, say, heart
disease, based on features like blood pressure, smoking, etc, you will build
simple/parsimonious models, such as:

	heart disease <- elevated blood pressure + chronic smoking + a few other predictors
	
You want to take action (treat the heart disease) so you study how it is
associated with some other things, like blood pressure. You build a model that
you can understand, and interpret.

On the other hand, if you are interested in text processing to convert pictures
of street signs into computer-readable text, you may not care about how the
model really works. All you want is a correct prediction: is this letter a “P”
or a “B”? 

	Is this letter a "P"? <- bunch of data

As long as the model has good predictive power, you will be happy, and won't
care if the data is inter-correlated (collinear) or not, or how many (possibly
transformed) predictors you have, whether 10 or 10,000.

## Explanation

In the first example, you are doing inference with simpler, interpretable
models, and this is **statistical modeling**.

In the second example, the model isn't as important as its predictive power, and
you are doing **machine learning**.

In terms of actual methods, to understand heart disease or another condition,
you may build a logistic regression model with a few predictors. To classify
text or an image, you may implement gradient boosting descent or some
complicated neural network.

## Caveats

To be sure, there is overlap among these two approaches. You may want to make
predictions in the statistical modeling framework, and for sure you can. Also,
logistic regression is often mentioned as a machine learning model.

Still, the framework described here is just that, a framework or a model, and
we all (should) know that in certain ways, "all models are wrong." But to
complete the thought, "... but some are useful."

## Summary and acknowledgment

In summary:

	statistical modeling <- perform **inference** based on interpretable models
	machine learning <- throw a lot of data at a model, make accurate **predictions**. Interpretability not important

This framework was partly inspired by an informal statement from Hadley Wickham.*


## Let me know what you think

If you or someone else have a different take, or
disagree with something in the above,
[let me know here](http://twitter.com/pavopax).


*Essentially, what he says is that "machine learners care about making really
accurate predictions" and "statisticians generally ... want to understand what
is going on". See this podcast from March 31, 2016, around 24:20:
["E634: Hadley Wickham, RStudio Chief Scientist & open source pioneer, on breakthroughs in data science, visualization, statistics."](https://itunes.apple.com/us/podcast/e634-hadley-wickham-rstudio/id315114957?i=1000365906688&mt=2)

