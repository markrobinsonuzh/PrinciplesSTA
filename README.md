# Principles of Spatial (Transcript)omics Analysis with Bioconductor

📖 [Book](https://lmweber.github.io/PrinciplesSTA/devel) [![deployment](https://img.shields.io/github/actions/workflow/status/lmweber/PrinciplesSTA/pages/pages-build-deployment?label=Book%20deployment)](https://github.com/lmweber/PrinciplesSTA/actions/workflows/pages/pages-build-deployment)  
🐳 [Docker](https://github.com/lmweber/PrinciplesSTA/pkgs/container/PrinciplesSTA) [![biocbook](https://img.shields.io/github/actions/workflow/status/lmweber/PrinciplesSTA/biocbook.yml?label=Docker%20image)](https://github.com/lmweber/PrinciplesSTA/actions/workflows/biocbook.yml)


## Overview

This repository contains source files for the "Principles of Spatial (Transcript)omics Analysis with Bioconductor" book.


## Link to book

The development version of the book is available at: https://lmweber.org/PrinciplesSTA/


## For developers

The book is built using [BiocBook](https://github.com/js2264/BiocBook). To preview and build the book locally, run the following code:

```
library(BiocBook)
bb <- BiocBook(".")
preview(bb)
```

You may also need to first install the set of dependency packages:

```
if (!require("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install("BiocParallel","SingleCellExperiment",
                     "reticulate","zellkonverter","BiocFileCache",
                     "STexampleData","SpatialExperiment","igraph",
                     "lobstr","rtracklayer","scater","scran",
                     "spatialLIBD","Banksy","RANN","RColorBrewer",
                     "hoodscanR","igraph","imcRtools","ExperimentHub",
                     "STexampleData","ggplot2","dplyr","nnSVG",
                     "patchwork","pheatmap","tidyr","ggspavis",
                     "scran","scater","SpatialExperiment")
```


## For admins

To make changes and publish an updated version of the book, first manually commit and push any changes to files that are located outside the `inst/` directory, and then run the following code using the `BiocBook` package to commit and publish changes to files in `inst/` (e.g. `inst/assets/_book.yml` and `inst/pages/chapter-name.qmd` if adding a new chapter):

```
library(BiocBook)
bb <- BiocBook(".")
publish(bb, message = "commit message")
```


## Image files

Image files are stored separately in the [PrinciplesSTA-resources](https://github.com/lmweber/PrinciplesSTA-resources) repository and linked within chapters using URLs, in order to keep the size of the main repository smaller. Please use this repository for image files in pull requests.


## BiocBook

The [BiocBook](https://github.com/js2264/BiocBook) package was developed by [Jacques Serizay](https://jserizay.com/) for building Quarto books with Bioconductor. More details on BiocBook can be found in the [BiocBook book](https://jserizay.com/BiocBookDemo/devel/).
