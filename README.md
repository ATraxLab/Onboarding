---
title: "Onboarding"
output: 
  html_document: 
    keep_md: yes
---

Links and first steps for new group members. 

(To go here:

1. ~~CITI training~~
2. Software links: ~~RStudio~~, ~~LaTeX~~, Gephi
3. Learning resources: ~~Happy Git with R~~, ~~R tutorial pages~~
4. First assignments)


# CITI training

Before doing research on human subjects through the university, you need to do some training on the ethical issues surrounding that type of research. 

1. Go to WSU's Institutional Review Board (IRB) website. It's currently [here](https://www.wright.edu/research/research-compliance/irb-general-information) (they seem to reorg every six months, so submit a pull request if the link is outdated). Click the CITI link and make an account, giving WSU as your institution.  
2. The IRB website has a list of the required training. As of June 2020, the required modules are the *Social/Behavioral Investigators Basic Course*, *IPS for Researchers*, and *Conflict of Interest*. You may be able to choose these directly, or you may need to answer a questionnaire about the kind of research you'll be doing. 
3. If you're working on an NSF-supported project, you'll also need to take the *Responsible Conduct for Researchers* course. 
4. After you complete each module, download PDFs of the completion certificates, and send those to me once they're all finished. 

**Note on the training**: This stuff is not thrilling reading; take it seriously anyway. If you're not sure afterwards about the relevance, talk to me! This is important, but I'll be the first to admit that hours of reading + multiple-choice quizzes are not the ideal way to teach that significance. 



# Software setup

We use R, LaTeX, Github, and sometimes other pieces as well. Here's one path to go through getting all that.

1. Download and install [Rstudio](https://rstudio.com/products/rstudio/download/) -- note that it has you install R as a first step. 
2. Get [LaTeX](https://www.latex-project.org/get/) for your system (Overleaf can work for most purposes in a pinch).
3. If you don't have Github, don't worry about it yet--the learning git section below has you covered.




# Learning software

## Learn to use R! 

Some tutorial options (see below for more):

* [This tutorial](http://www.cyclismo.org/tutorial/R/) is a good starting place, especially sections 1-7, 13, and 15. Get in the habit of commenting and saving your work as script (.R) files. 
* [R for Data Science](https://r4ds.had.co.nz/) is a work-through-it-as-you-go book. It will take a while, but you will learn a lot about some modern and very nice tools in R.

Start using markdown in R to keep notes on your work:

1. Install the `knitr` package in R. 
2. Make sure that in RStudio's global options, under the Sweave tab, it's set to weave Rnw files using knitr.
3. Choose your own adventure: LaTeX or Rmarkdown. Both are useful formats and you'll probably end up learning both eventually. I started with all my knitr reports in LaTeX and these days tend to prefer Rmarkdown, but if you're already comfy with TeX, you might prefer that.
  i) The [Introduction to R Markdown](https://rmarkdown.rstudio.com/articles_intro.html) from RStudio
  ii) A [LaTeX knitr tutorial](https://joshldavis.com/2014/04/12/beginners-tutorial-for-knitr/) (stop at "Running knitr" section and just use RStudio's "compile PDF" button)


## Learn to use git! 

Not gonna lie, this one is a bit of a journey. The best guide I've found for our purposes is Jenny Bryan's [Happy Git with R](https://happygitwithr.com/). 

Don't try to wade through it all at once; plan for this to take time, and do it in installments. Start early, since you'll need to start keeping an updated repo for your source code and lab notebook. 


# Other resources

I haven't tried all of these, but have seen them recommended. 

* [R tutorials from twotorials.com](https://www.twotorials.com) - short and focused
* [R tutorials from Google developers](https://www.youtube.com/playlist?list=PLOU2XLYxmsIK9qQfztXeybpHvru-TrqAP) - somewhat longer
