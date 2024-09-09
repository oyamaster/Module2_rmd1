---
title: "Module2 - R Markdown Document 1"
author: "Daniel Oyama"
date: "2024-09-06"
output:
  pdf_document: default
  html_document: default
  word_document: default
---



# This is a level 1 header

## R Markdown

### This is a level 3 header

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

Here is a link to [GOOGLE](http://google.com)

Here is a word in **bold** and another word in __bold__.

Here is a word in *italics* and another word in _italics_.

Whe we compile our document, we are using the `rmarkdown` package. 

Here are some example  R commands:

```
2 + 2 
mean(c(1,2,3,4,5))
```

Here is an example of a non-numbered list:

* Breakfast
  - food
      + eggs
      + toast
      + bacon
  - drink
    + apple juice
* Lunch
  - taco
* Dinner
  - baked chicken
  - broccoli
  - rice

Here is another list:

1. Breakfast
  a. food
      i. eggs
      ii. toast
      iii. bacon
  b. drink
    i. apple juice
2. Lunch
  a. taco
3. Dinner
  a. baked chicken
  b. broccoli
  c. rice

Here is a blockquote:

> teste
> teste 
> 
> 1. teste
> 2. teste

Here is a blockquote:

> teste
> teste 
> 
> > teste

Hre:

>     2 + 2 
>     mean(c(1,2,3,4,5))

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:


``` r
summary(cars)
```

```
##      speed           dist       
##  Min.   : 4.0   Min.   :  2.00  
##  1st Qu.:12.0   1st Qu.: 26.00  
##  Median :15.0   Median : 36.00  
##  Mean   :15.4   Mean   : 42.98  
##  3rd Qu.:19.0   3rd Qu.: 56.00  
##  Max.   :25.0   Max.   :120.00
```

## Including Plots

You can also embed plots, for example:

![](module2_rmd1_files/figure-latex/pressure-1.pdf)<!-- --> 

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.


## Insert Tables


``` r
knitr::kable(head(cars),
             caption = "Top 6 Rows of Cars Dataset")
```



Table: Top 6 Rows of Cars Dataset

| speed| dist|
|-----:|----:|
|     4|    2|
|     4|   10|
|     7|    4|
|     7|   22|
|     8|   16|
|     9|   10|

## Insert an equation

$$ Y = \beta_0 + \beta_1x$$
## Insert images
Here is an image inserted

![sunstar](sunstar.png)
![r logo](https://www.r-project.org/logo/Rlogo.svg)


## Insert text with some footnotes
Here is footnote reference [^1] and another [^longnote]

Here is an inline footnote ^[Inline notes are easier to write, since you dont have to pick an identifier to type]
 
 [^1]: Here is the footnote
 [^longnote]: Here is one with multipleblocks

