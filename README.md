# Principles of Spatial Transcriptomics Analysis with Bioconductor

📖 [Book](https://lmweber.github.io/PrinciplesSTA/devel) [![deployment](https://img.shields.io/github/actions/workflow/status/lmweber/PrinciplesSTA/pages/pages-build-deployment?label=Book%20deployment)](https://github.com/lmweber/PrinciplesSTA/actions/workflows/pages/pages-build-deployment)  
🐳 [Docker](https://github.com/lmweber/PrinciplesSTA/pkgs/container/PrinciplesSTA) [![biocbook](https://img.shields.io/github/actions/workflow/status/lmweber/PrinciplesSTA/biocbook.yml?label=Docker%20image)](https://github.com/lmweber/PrinciplesSTA/actions/workflows/biocbook.yml)


## Overview

This repository contains source files for the 'Principles of Spatial Transcriptomics Analysis with Bioconductor' book.


## Link to book

The development version of the book is available at: https://lmweber.org/PrinciplesSTA/


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


## For developers: image files

Image files are stored separately in the [PrinciplesSTA-resources](https://github.com/lmweber/PrinciplesSTA-resources) repository and linked within chapters using URLs, in order to keep the size of the main repository smaller. Please use this repository for image files in pull requests.


## BiocBook

This book is built using the [BiocBook](https://github.com/js2264/BiocBook) package, developed by [Jacques Serizay](https://jserizay.com/) for building Quarto books with Bioconductor. More details on BiocBook can be found in the [BiocBook book](https://jserizay.com/BiocBookDemo/devel/).
