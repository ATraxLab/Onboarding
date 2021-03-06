---
title: "Onboarding"
output: 
  html_document: 
    toc: true
    keep_md: yes
---

Links and first steps for new group members. 


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

If you're doing a network analysis project, you may need [Gephi](https://gephi.org/). The flexibility of writing R scripts is worth the extra trouble for most of what we do, but Gephi is a nice way to get started and play around with visualization options (which is, spoiler alert, not R/igraph's best thing). 


# Learning software

## R

Some tutorial options (see below for more):

* [This tutorial](http://www.cyclismo.org/tutorial/R/) is a good starting place, especially sections 1-7, 13, and 15. Get in the habit of commenting and saving your work as script (.R) files. 
* [R for Data Science](https://r4ds.had.co.nz/) is a work-through-it-as-you-go book. It will take a while, but you will learn a lot about some modern and very nice tools in R.

Start using markdown in R to keep notes on your work:

1. Install the `knitr` package in R. 
2. Make sure that in RStudio's global options, under the Sweave tab, it's set to weave Rnw files using knitr.
3. Choose your own adventure: LaTeX or Rmarkdown. Both are useful formats and you'll probably end up learning both eventually. I started with all my knitr reports in LaTeX and these days tend to prefer Rmarkdown, but if you're already comfy with TeX, you might prefer that.
  i) The [Introduction to R Markdown](https://rmarkdown.rstudio.com/articles_intro.html) from RStudio
  ii) A [LaTeX knitr tutorial](https://joshldavis.com/2014/04/12/beginners-tutorial-for-knitr/) (stop at "Running knitr" section and just use RStudio's "compile PDF" button)


## LaTeX

1. For Windows, I recommend [TeXstudio](https://texstudio.org/) as a free editing program. (The MiKTeX distribution comes with TeXworks, which is fine but pretty barebones.) For Mac, check the [Getting LaTeX](https://www.latex-project.org/get/) page above.
2. The [Cambridge engineering page](http://www-h.eng.cam.ac.uk/help/tpl/textprocessing/) has a lot of LaTeX help links, ranging from from basic tutorials to the ins and outs of tables and bibliographies. 


## git and Github 

Not gonna lie, this one is a bit of a journey. 

1. The best guide I've found for our purposes is Jenny Bryan's [Happy Git with R](https://happygitwithr.com/). Don't try to wade through it all at once; plan for this to take time, and do it in installments. Start early, since you'll need to start keeping an updated repo for your source code and lab notebook. 
2. Once you have a Github account, you should apply for the [student developer pack](https://docs.github.com/en/free-pro-team@latest/github/teaching-and-learning-with-github-education/applying-for-a-student-developer-pack), which gives access to various pro features and tools.


## `knitr`

Sooner or later, adding comments to source code isn't enough, and you want to be able to display code and output in a longer report. Enter `knitr`. 

1. Start by reading Yihui Xie's [minimal examples page](https://yihui.org/knitr/demo/minimal/), which has a brief explanation/demo of how it works and then gives starter files. Look at the .Rnw files for LaTeX, or the .Rmd file for Rmarkdown. 
2. Save a copy of one of those files locally, open in RStudio, and try to compile it. Once you get it working, you can do your stats and report writing all from RStudio. 

Two extra notes if you're using Rnw/LaTeX (skip if you're using Rmarkdown):

1. Under Rstudio's `Tools > Global Options`, in the SWeave tab, set the "Weave Rnw files using:" option to **knitr**.
2. If you're on Windows and using MiKTeX as your LaTeX distribution, you probably need to let it [install missing packages on-the-fly](https://stackoverflow.com/questions/55763116/r-sweave-rnw-wont-produce-a-pdf-file-exit-code-1).



## Reference management

* [Pick a reference manager](https://en.wikipedia.org/wiki/Comparison_of_reference_management_software) if you don't already have one. Zotero or Mendeley are both popular. 
* If you're using LaTeX/BibTeX, here's a starter kit:
  + [This page](http://www.bibtex.org/Using/) gives a very minimal example of how to get it working. 
  + [JabRef](https://www.jabref.org/) is a frontend to manage BibTeX files. It's not a replacement for Zotero or Mendeley, but it's great for cleaning up and maintaining `.bib` files after they're exported from your main reference software. (`File > Append database` is your friend.)
  + [natbib](http://merkel.texture.rocks/Latex/natbib.php) is a very commonly used package which implements citations better than base LaTeX. 
  + There's a [list of entry types](https://kmh-lanl.hansonhub.com/spie/bibtex-overview.html) and their required/optional fields if you need to fill in missing information on some obscure entry.



## Other software

The topics/links below are a bit more project-dependent.

### Networks in R with `igraph`

Once you have R/RStudio working, you can do network stuff with the `igraph` package. In recommended order...

* [Getting started](https://igraph.org/r/) gives installation instructions if you don't already have the package.
* [R igraph manual pages](https://igraph.org/r/doc/aaa-igraph-package.html) gives a very brief rundown of how `igraph` objects are structured. They're a bit more complicated than data frames, so take a look.
* [Static and dynamic network visualization with R](https://kateto.net/network-visualization) is an awesome and thorough tutorial by Katya Ognyanova. Working up through 4.2 (Network layouts) is a good idea, and 4.3-4.4 may also be useful. 


# Other resources

I haven't tried all of these, but they've all been recommended to me. 

* [R tutorials from twotorials.com](https://www.twotorials.com) - short and focused
* [R tutorials from Google developers](https://www.youtube.com/playlist?list=PLOU2XLYxmsIK9qQfztXeybpHvru-TrqAP) - somewhat longer
* [Git tutorials](https://www.gitkraken.com/resources/learn-git) from GitKraken are a pretty good intro to many of the concepts.
