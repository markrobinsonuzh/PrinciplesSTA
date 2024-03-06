# Best Practices for Spatial Transcriptomics Analysis with Bioconductor

<!-- [![R build status](https://github.com/lmweber/BestPracticesST/workflows/render-and-publish/badge.svg)](https://github.com/lmweber/BestPracticesST/actions) -->

Repository containing source files for 'Best Practices for Spatial Transcriptomics Analysis with Bioconductor' online book.


## Website

The website for the compiled version of the book is at: https://lmweber.org/BestPracticesST/


## Source files

The main content of the book is in the Quarto `.qmd` files in the [chapters/](chapters/) subdirectory, with one `.qmd` file per chapter.

Rendering and publishing to the website uses the GitHub Actions workflow in: [.github/workflows/](.github/workflows/)


## Render locally

Run `quarto render` to render the book locally.


## Publish manually

Run `quarto publish` to render and publish to GitHub Pages manually (without using GitHub Actions workflow).

