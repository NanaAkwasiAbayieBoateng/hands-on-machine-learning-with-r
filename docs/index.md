--- 
title: "Hands-on Machine Learning with R"
date: "2018-07-03"
site: bookdown::bookdown_site
output: bookdown::gitbook
documentclass: book
bibliography: [book.bib, packages.bib]
biblio-style: apalike
link-citations: yes
github-repo: bradleyboehmke/hands-on-machine-learning-with-r
description: "A Machine Learning Algorithmic Deep Dive Using R."
---


# Preface {-}

<img src="images/mlr.png"  style="float:right; margin: 0px 0px 0px 0px; width: 40%; height: 40%;" />
Welcome to Hands-on Machine Learning with R.  This book provides hands-on modules for many of the most common machine learning methods to include:

- Generalized low rank models
- Clustering algorithms
- Autoencoders
- Regularized models
- Random forests 
- Gradient boosting machines 
- Deep neural networks
- Stacking / super learner
- and more!

You will learn how to build and tune these various models with R packages that have been tested and approved due to their ability to scale well. However, my motivation in almost every case is to describe the techniques in a way that helps develop intuition for its strengths and weaknesses.  For the most part, I minimize mathematical complexity when possible but also provide resources to get deeper into the details if desired.


## Who should read this {-}

I intend this work to be a practitioner's guide to the machine learning process and a place where one can come to learn about the approach and to gain intuition about the many commonly used, modern, and powerful methods accepted in the machine learning community. If you are familiar with the analytic methodologies, this book may still serve as a reference for how to work with the various R packages for implementation.  While an abundance of videos, blog posts, and tutorials exist online, I've long been frustrated by the lack of consistency, completeness, and bias towards singular packages for implementation. This is what inspired this book. 

This book is not meant to be an introduction to R or to programming in general; as I assume the reader has familiarity with the R language to include defining functions, managing R objects, controlling the flow of a program, and other basic tasks.  If not, I would refer you to [R for Data Science](http://r4ds.had.co.nz/index.html) to learn the fundamentals of data science with R such as importing, cleaning, transforming, visualizing, and exploring your data. For those looking to advance their R programming skills and knowledge of the languge, I would refer you to [Advanced R](http://adv-r.had.co.nz/). 

Instead, this book is meant to help R users learn to use the machine learning stack within R, which includes using various R packages such as `glmnet`, `h20`, `ranger`, `xgboost`, `lime`, and others to effectively model and gain insight from your data. The book favors a hands-on approach, growing an intuitive understanding of machine learning through concrete examples and just a little bit of theory.  While you can read this book without opening R, I highly recommend you experiment with the code examples provided throughout.

## Why R {-}

R has emerged over the last couple decades as a first-class tool for scientific computing tasks, and has been a consistent leader in implementing statistical methodologies for analyzing data. The usefulness of R for data science stems from the large, active, and growing ecosystem of third-party packages: `tidyverse` for common data analysis activities; `h2o`, `ranger`, `xgboost`, and others for fast and scalable machine learning; `lime`, `pdp`, `DALEX`, and others for machine learning interpretability; and many more tools will be mentioned throughout the pages that follow.  

## Structure of the book {-} 

Each chapter of this book focuses on a particular part of the machine learning process along with various packages to perform that process.  

TBD...


## Conventions used in this book {-}

The following typographical conventions are used in this book:

* ___strong italic___: indicates new terms,
* __bold__: indicates package & file names,
* `inline code`: indicates commands or other text that could be typed literally by the user,
* code chunk: indicates commands or other text that could be typed literally by the user


```r
1 + 2
## [1] 3
```

In addition to the general text used throughout, you will notice the following code chunks with images, which signify:

<div class="rmdtip">
<p>Signifies a tip or suggestion</p>
</div>

<div class="rmdnote">
<p>Signifies a general note</p>
</div>

<div class="rmdwarning">
<p>Signifies a warning or caution</p>
</div>


## Additional resources {-}

There are many great resources available to learn about machine learning.  At the end of each chapter I provide a *Learn More* section that lists resources that I have found extremely useful for digging deeper into the methodology and applying with code.  


## Feedback {-}

Reader comments are greatly appreciated.  To report errors or bugs please post an issue at https://github.com/bradleyboehmke/hands-on-machine-learning-with-r/issues.


## Acknowledgments {-} 

TBD


## Software information {-} 

An online version of this book is available at https://bradleyboehmke.github.io/hands-on-machine-learning-with-r/.  The source of the book is available at https://github.com/bradleyboehmke/hands-on-machine-learning-with-r. The book is powered by https://bookdown.org which makes it easy to turn R markdown files into HTML, PDF, and EPUB.

This book was built with the following packages and R version.  All code was executed on 2013 MacBook Pro with a 2.4 GHz Intel Core i5 processor, 8 GB of memory, 1600MHz speed, and double data rate synchronous dynamic random access memory (DDR3). 


```r
# packages used
pkgs <- c(
  "h2o"
)

# package & session info
devtools::session_info(pkgs)
#> Session info -------------------------------------------------------------
#>  setting  value                       
#>  version  R version 3.5.0 (2018-04-23)
#>  system   x86_64, darwin15.6.0        
#>  ui       X11                         
#>  language (EN)                        
#>  collate  en_US.UTF-8                 
#>  tz       America/New_York            
#>  date     2018-07-03
#> Packages -----------------------------------------------------------------
#>  package   * version   date       source        
#>  bitops      1.0-6     2013-08-17 CRAN (R 3.5.0)
#>  graphics  * 3.5.0     2018-04-24 local         
#>  grDevices * 3.5.0     2018-04-24 local         
#>  h2o         3.18.0.11 2018-05-24 CRAN (R 3.5.0)
#>  jsonlite    1.5       2017-06-01 CRAN (R 3.5.0)
#>  methods   * 3.5.0     2018-04-24 local         
#>  RCurl       1.95-4.10 2018-01-04 CRAN (R 3.5.0)
#>  stats     * 3.5.0     2018-04-24 local         
#>  tools       3.5.0     2018-04-24 local         
#>  utils     * 3.5.0     2018-04-24 local
```



