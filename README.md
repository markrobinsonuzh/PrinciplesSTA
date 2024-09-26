# Best Practices for Spatial Transcriptomics Analysis with Bioconductor

📖 [Book](https://lmweber.github.io/BestPracticesST/devel) [![deployment](https://img.shields.io/github/actions/workflow/status/lmweber/BestPracticesST/pages/pages-build-deployment?label=Book%20deployment)](https://github.com/lmweber/BestPracticesST/actions/workflows/pages/pages-build-deployment) 🐳 [Docker](https://github.com/lmweber/BestPracticesST/pkgs/container/BestPracticesST) [![biocbook](https://img.shields.io/github/actions/workflow/status/lmweber/BestPracticesST/biocbook.yml?label=Docker%20image)](https://github.com/lmweber/BestPracticesST/actions/workflows/biocbook.yml)


## Overview

This repository contains source files for the 'Best Practices for Spatial Transcriptomics Analysis with Bioconductor' book.


## Link to book

The development version of the book is available at: https://lmweber.org/BestPracticesST/


## For developers: publish updated version of book

To make changes and publish an updated version of the book, first manually commit and push any changes to files that are located outside the `inst/` directory, and then use the following code using the `BiocBook` package to commit and publish changes to files in `inst/` (e.g. `inst/assets/_book.yml` and `inst/pages/chapter-name.qmd` if adding a new chapter):

```
library(BiocBook)
bb <- BiocBook(".")
publish(bb, message = "commit message")
```


## For developers: preview locally

To build and preview the book locally, use the following code:

```
library(BiocBook)
bb <- BiocBook(".")
preview(bb)
```


## BiocBook

The book is built using the [BiocBook](https://github.com/js2264/BiocBook) package, developed by [Jacques Serizay](https://jserizay.com/) for building Quarto books with Bioconductor. For more details on building a book with BiocBook, see the [BiocBook book](https://jserizay.com/BiocBookDemo/devel/).
