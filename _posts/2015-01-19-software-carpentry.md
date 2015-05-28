---
layout: post
title: "Software Carpentry"
description: ""
categories: 
---

<i>Below are notes from a talk at the Harvard Innovation Lab by Jim Waldo, CTO and instructor, Harvard University, on January 19, 2015. The following notes cover about 85% of the talk. See bottom for a bonus.</i>

### Introductory remarks
If you're embarrassed by your code (by going open source) then you should not be distributing it to people in the first place.

You can't do agile and fast development without practicing some basic principles. That is, "fail fast and often" only works if you're working well.

### (1) Follow A Style Guide

But it should be neither Deuteronomy nor chaos - requires a balance. Just find one and use.

### (2) Use Source Code Control

Doesn't matter which, just use one.

Use this branching, in descending order of 'polish':  

* MAIN LINE - always works, always ready when a demo is required by VC or something  

* feature/dev branch  

* current branch  

* experimental branch (do what you want)  

How often to check in? about every 50-400 lines

Merging process:  

* first, (always) *pull* from main line  

* then, test/fix code  

* pull *again* - in case new updates made while you tested  

* only then, when no conflicts are present, actually push to main line  

You should merge:  

* code  

* tests  

* docs  

* review results  

[definition: a unit test tests small chunks of code]

### (3) Document your work, and your software
Good documentation makes it seem like the software is easy to use.

What the code is actually doing is not too important. Instead, document interface between objects/functions, the implementation, and the design.

Have a *dev log*: keep a text file open as you develop and take notes on what/why/how. This will be useful when debugging. Back in the day engineers wrote logs in actual notebooks.

### (4) Misc

**Track Bugs**

Some stats claim 10-20 bugs per 1k code-lines. Microsoft claims 1 bug per 2k lines ['still a \****load of bugs'].

Space shuttle program was able to achieve exactly zero bugs - on 250k lines of code  - but took years to develop. And by the way, in these situations, the "oh, just download the patch" is not going to cut it :) 

**Use Builds**

a build:  

* builds  

* runs tests  

* generates a report  

Reproducibility is important (make it automated). 

**Use an IDE** - which should implement many of the above practices out of the box.

### Other Notes

Good design comes from good designers. Good designers produce good design. They often learn from other good designers (cf. Fred Brooks, The Design of Design. [And see this Wired article.](http://www.wired.com/2010/07/ff_fred_brooks/)).

Audience question on hiring good devs. Three things to do:  

1. ask: how do you protect yourself form unexpected failures?  

2. ask: how do you review your/someone else's code?  

3. and also look at their code: does it have structure?  

Documentation, and code, is like literature. We speak of 'writing code.'

### Bonus: two things of which there two types, from Jim Waldo

There exist two types of code:  

* code that is tested  

* code that doesn't work  

There exist two types of data:  

* data that you've backed up  

* data that you're about to lose  
