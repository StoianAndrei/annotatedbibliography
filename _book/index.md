---
title: "Annotated Bibliography for Directed study"
author: "Andrei Stoian"
date: "2021-09-01"
site: bookdown::bookdown_site
documentclass: book
bibliography: [book.bib, packages.bib]
url: https://github.com/StoianAndrei/annotatedbibliography
# cover-image: path to the social sharing image like images/cover.jpg
description: "This is a book is an artifact that I deliver as part of my directed study on Veracity. It will describe all the sources that were used to inspire the final solution."
biblio-style: apalike
csl: chicago-fullnote-bibliography.csl
---


```r

path_img <- here::here()
knitr::include_graphics(path = file.path(path_img,"img/books.jpg"),dpi = 600)
```

![](E:/MASTER/DIRECTED_STUDY/MArkus/annotatedbibliography/img/books.jpg)<!-- -->

# About

This is a book is an artifact that I deliver as part of my directed study on Veracity. It will describe all the sources that were used to inspire the final solution.

## Process

Creating an annotated bibliography calls for the application of a variety of intellectual skills:

-   concise exposition

-   succinct analysis

-   informed library research

First, I locate and record citations to books that were provided by my supervisor, articles, periodicals, and documents that may contain useful information and ideas on your topic.

Briefly examine and review the actual items. Then choose those works that provide a variety of perspectives on your topic.

I cite the book, article, or document using the appropriate style. For this purpose I have used APA(7th edition) citation like so:

> Chi, E. (2009). Augmented social cognition: using social web technology to enhance the ability of groups to remember, think, and reason. Proceedings of the 2009 ACM SIGMOD International Conference on Management of Data, 973--984. <https://doi.org/10.1145/1559845.1559959>

Write a concise annotation that summarizes the central theme and scope of the book or article. Include one or more sentences that

1.  evaluate the authority or background of the author

2.  comment on the intended audience

3.  compare or contrast this work with another you have cited

4.  explain how this work illuminates your bibliography topic.

## Structure

Each chapter is an .Rmd file, and each .Rmd file can contain one (and only one) chapter. I will use each chapter for a reference so that we can keep a consistent structure for each book. A chapter *must* start with a first-level heading:

`# A good chapter`, and can contain one (and only one) first-level heading.

Use second-level and higher headings within chapters like:

`## A short section` or

`### An even shorter section`.

The `index.Rmd` file is required, and is also the first book chapter. It will be the homepage when I render the book.

## Instructions to render the book

The book is both render in the HTML version :

1.  Find the **Build** pane in the RStudio IDE, and

2.  Click on **Build Book**, then select your output format, or select "All formats" if you'd like to use multiple formats from the same book source files.

Or build the book from the R console:


```r
bookdown::render_book()
```

But also I render this example to PDF as R command `bookdown::render_book('index.Rmd', 'bookdown::pdf_book')` . I install XeLaTeX and pandoc package thought the command `'tinytex::install_tinytex()` : TinyTeX (which includes XeLaTeX): <https://yihui.org/tinytex/>.

## Preview book

As I build the book chapter by chapter i use the feature called `Visual Editor` that makes `Rmardown` text look like a word page and also I start a local server to live preview this HTML book. This preview will update as you edit the book when you save individual .Rmd files. You can start the server in a work session by using the RStudio add-in "Preview book", or from the R console:


```r
bookdown::serve_book()
```
