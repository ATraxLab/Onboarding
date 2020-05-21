---
output: 
  html_document: 
    keep_md: yes
---

# Onboarding
Links and first steps for new group members. 

(To go here:

1. CITI training
2. Software links: RStudio, LaTeX, Gephi
3. Learning resources: Happy Git with R, R tutorial pages
4. First assignments)


## Software setup

We use R, LaTeX, Github, and sometimes other pieces as well. Here's one path to go through getting all that.

1. Download and install [Rstudio](https://rstudio.com/products/rstudio/download/) -- note that it has you install R as a first step. 
2. Get [LaTeX](https://www.latex-project.org/get/) for your system (Overleaf can work for most purposes in a pinch).
3. If you don't have Github, don't worry about it yet.


## Learning software

Learn to use R! Some tutorial options:

* [This tutorial](http://www.cyclismo.org/tutorial/R/) is a good starting place, especially sections 1-7, 13, and 15. Get in the habit of commenting and saving your work as script (.R) files. 
* [R for Data Science](https://r4ds.had.co.nz/) is a work-through-it-as-you-go book. It will take a while, but you will learn a lot about some modern and very nice tools in R.

Start using markdown in R to keep notes on your work:

1. Install the `knitr` package in R. 
2. Make sure that in RStudio's global options, under the Sweave tab, it's set to weave Rnw files using knitr.
3. Choose your own adventure: LaTeX or Rmarkdown. Both are useful formats and you'll probably end up learning both eventually. I started with all my knitr reports in LaTeX and these days tend to prefer Rmarkdown, but if you're already comfy with TeX, you might prefer that.
  i) The [Introduction to R Markdown](https://rmarkdown.rstudio.com/articles_intro.html) from RStudio
  ii) A [LaTeX knitr tutorial](https://joshldavis.com/2014/04/12/beginners-tutorial-for-knitr/) (stop at "Running knitr" section and just use RStudio's "compile PDF" button)
