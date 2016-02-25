---
title       : Predicting Children's Height
subtitle    : Using Linear Regression
author      : Malay Das
job         : Tata Consultancy Services
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Prediction Basis :

1. The App predicting Children's height, is based on dataset "Galton" (available in UsingR package).

2. Famous mathematician Francis Galton , published it in his 19th century paper (Regression Toward Mediocricity in Hereditary Stature).

3. Galton (1886) presented these data in a table, showing a cross-tabulation of 928 adult children born to 205 fathers and mothers.

4. Data frame observations was on the following 2 variables. 
      - parent a numeric vector: height of the mid-parent (average of father and mother) and 
      - child a numeric vector: height of the child 

5. A linear regression fitted on top of these 928 observation essentially helped me to determine children's height.

--- 

## How to operate

1. Two numeric input boxes will captures height (in inch) of both the parents .

2. Average of heights of both the parents ultimately will be feeded to the linear model.

3. Press calculate to show the result.

---

## Graphical Representation

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1-1.png)

- Above plot depicts the Galton dataset, with linear fitted model (blue line). 

- Ultimate calculation of child's height is based on an equation formulated using linear regression (In next slide).

---

## Regression Formula -

1. y=mx+c ; 

- Here y is the child's height.
- x is the avarage of both the parent's height (input).
- m and c are the coefficients mentioned below (respectively) $$ mod\$coeff[2], and  \mod\$coeff[1] $$      
- where mod=lm(child~parent,data=Galton)

