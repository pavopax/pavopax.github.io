---
layout: post
title: 'Precision-recall cheat sheet
description: ""
categories: 
---

Plus sensitivity, specificity, false positive rate, AUC, etc

![Precision Recall](/img/blog/precision-recall.jpg)

Precision is "how useful the search results are", and recall is "how complete the results are".

the following are the two sides of the main plot above
	TPR = TP / (TP+FN)
	FPR = FP / (FP + TN)

> In simple terms, high precision means that an algorithm returned
> substantially more relevant results than irrelevant ones, while high recall
> means that an algorithm returned most of the relevant results.

> Precision can be seen as a measure of exactness or quality, whereas recall is
> a measure of completeness or quantity.

# There are two curves

... for which you can compute Area under curve

AUC for ROC curve

- The more popular, well-known one
- TPR vs FPR

AUC for PR curve (precision-recall

- prefereed in the case of imbalanced outcome
- Precision vs recall

## AUC curve

TPR vs FPR

TPR on y, FPR on x

- TPR = recall = sensitivity
- FPR  = 1 - specificity

# References

[Comprehensive table at
wikipedia](https://en.wikipedia.org/wiki/Receiver_operating_characteristic)
