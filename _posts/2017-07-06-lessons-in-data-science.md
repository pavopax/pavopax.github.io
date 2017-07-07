---
layout: post
title: 'Lessons in data science/machine learning (mostly not taught in school'
description: ""
categories: 
---

> Don't start with a hammer. Find the nail first, then grab the right tool.

Or, [why technology alone is not enough](https://developer.apple.com/wwdc/).

From a Fireside Chat at Galvanize SF, July 5 2017, with:

  * [Mark Meloon](https://www.linkedin.com/in/markmeloon) (Caltech, startups,
    teaches data science)
  * [Sean Gerrish](http://www.seangerrish.com)
    (Princeton, Google)
  * [Yunkai Zhou](http://linkedin.com/in/yunkaizhou) (Tsinghua, Google)


See below for some quick take-aways from this talk in regards to "doing" data
science and machine learning in industry.

# Problem solving

Ask the right questions for the problem you're looking at.

* Tip (from SG): Learn "case interview" secrets: they teach very useful
  problem-solving skills.

Don't just look at one angle of the problem: look at the full thing. Knowing
the business context is very important. This is not taught in school.

# Thinking about data

Have a healthy skepticism of data. 

A story from Google (from SG):

> A team of data scientists spent a lot of time creating some report. Showed it
> to Larry Page. After a few seconds, he said "That figure doesn't look
> right". He was a better data scientist than most of the data science team -
> because he had a healthy skepticism of data.

Data you normally get used to in school, Coursera courses, etc is clean. This
doesn't happen in real life. Nothing can compare to playing with real
data. It's a significantly different experience.

# Don't be excited about algorithms

> Don't start with a hammer. Find the nail first, then grab the right tool. (YZ)

In other words, don't be excited about algorithms. First, figure out the right
problem to ask, then understand the context, etc, since:

> 90% of problems can be solved with linear or logistic regression (SG)

Therefore, know well the intuition behind these. Too many people go for more
complex algorithms, needlessly
([see this](https://twitter.com/benhamner/status/837787061864181760) from
@benhhamner (Kaggle/Google)).


# What is important when doing machine learning modeling?

Not the modeling part (at least, not that important).

Instead, what goes in and what comes out are often more important:
	
  * What goes in: data quality (!!), feature engineering, business context
  * What comes out: communication is very important
  
(This is hard stuff! That's why these roles are in demand).

Of course, you want to build a good model. But you may need to prioritize...


# Prioritizing problems

When evaluating different problems for impact, ask yourself:

  * If we got a result, how impactful will it be?
  * How likely are we to get a good result?

Building a good model is just one part of this, but may not be the most
important (see previous section).

# Where is ML/DS effective/not effective?

Machine learning/data science works very well in:

  * consumer-facing companies b/c lots of ways to improve things using ML
  * when you have a lot of data: sales, marketing, (biotech?)

Less well:

  * **when you don't have data infrastructure ready**
  * finance - need more of traditional statistical lessons, not ML, based on
    the types of problems they are solving (In contrast to consumer facing
    companies, where "you don't need to know statistical lessons in many ML
    applications in this industry" (SG))


# If you are starting out

Learn to program: "there are not many people who know both programming
(computer science) and data science/statistics" (SG).

> Startups don't hire statisticians. They hire machine learning engineers
> because they have wider skill set. (SG)

Also, "The job search process is fairly artificial. It's a high pressure
situation for everyone." (MM)

As above, be able to explain well the basic concept in machine learning. Many
people know a bunch of algorithms and their parameters, but can't communicate
well the basics of training/testing, overfitting, etc. But the latter is what
is usually asked in interviews.
