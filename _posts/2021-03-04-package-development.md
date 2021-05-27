---
layout: post
title: "Developing an R Package"
subtitle: ":package: Steps to start creating your own Bioconductor package"
tags: [R, Bioconductor, development]
comments: true
---

Interested in building your own R package? Here I'll outline the steps
I took to create my own! Note this will be tailored specifically to creating
Bioconductor packages, not CRAN. So just keep that in mind.

# Useful resources

* [R packages by Hadley Wickham and Jenny Bryan](https://r-pkgs.org/index.html)
* [Bioconductor package guidelines](https://www.bioconductor.org/developers/package-guidelines/)
* [biocthis package](https://lcolladotor.github.io/biocthis/articles/biocthis.html)

# Getting started

# Project tree

```
| - .github
  | -- ISSUE_TEMPLATE
    | --- issue_template.md
  | -- workflows
    | --- check-bioc.yml
    | --- R-CMD-check.yaml
    | --- test-coverage.yaml
| - R
  | -- data.R
  | -- fedup.R
  | -- femap.R
  | -- genes.R
  | -- pathways.R
  | -- plot.R
| - data
  | -- geneDouble.rda
  | -- geneMulti.rda
  | -- geneSingle.rda
  | -- pathwaysGMT.rda
  | -- pathwaysTXT.rda
  | -- pathwaysXLSX.rda
| - inst
  | -- extdata
    | --- Human_Reactome_November_17_2020_symbol.gmt
    | --- NIHMS1587165-supplement-1587165_Sup_Tab_2.txt
    | --- SAFE_terms.xlsx
  | -- figures
    | --- fedup.png
    | --- fedupDotplot-1.png
    | --- fedupEM.png
  | -- script
    | --- genes.R
    | --- pathwaysGMT.R
    | --- pathwaysTXT.R
    | --- pathwaysXLSX.R
  | -- NEWS.Rd
| - man
| - tests
  | -- testthat
    | --- test_1_pathways.R
    | --- test_2_genes.R
    | --- test_3_enrichment.R
    | --- test_4_plot.R
    | --- test_5_em.R
  | -- testthat.R
| - vignettes
  | -- figures
    | --- fedupEM_geneDouble.png
    | --- fedupEM_geneMulti.png
    | --- fedupEM_geneSingle.png
  | -- fedup_doubleTest.rmd
  | -- fedup_multiTest.rmd
  | -- fedup_singleTest.rmd
| - .Rbuildignore
| - .gitignore
| - .travis.yml
| - DESCRIPTION
| - LICENSE
| - NAMESPACE
| - README.Rmd
| - README.md
```

## .github
## R
## data
## inst
## man
## tests
## vignettes
