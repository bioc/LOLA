# LOLA: Genomic Locus Overlap Enrichment Analysis

[![Build Status](https://travis-ci.org/nsheff/LOLA.svg?branch=master)](https://travis-ci.org/nsheff/LOLA)
[![Release Build](http://bioconductor.org/shields/build/release/bioc/LOLA.svg)](http://bioconductor.org/checkResults/release/bioc-LATEST/LOLA/)
[![Bioc Devel Build](http://bioconductor.org/shields/build/devel/bioc/LOLA.svg)](http://bioconductor.org/checkResults/devel/bioc-LATEST/LOLA/)

<img src="man/figures/LOLA-logo.png" alt="LOLA logo" width="200"/>

* [Documentation](http://code.databio.org/LOLA).
* [Release version at Bioconductor](http://bioconductor.org/packages/LOLA/).
* [GitHub repository](http://github.com/nsheff/LOLA).

LOLA is an R package providing functions for testing overlap of sets of genomic regions with public and custom databases. You can think of it as testing your `bed file` (genome regions of interest) against a database of other `bed files` (regions from various previous studies) to look for enrichment of overlaps. This enables you to draw connections between newly generated data, and the growing public databases, leading to new hypotheses and annotation sharing.

This README provides a package overview, motivation, and installation instructions. For detailed documentation of functions and additional examples, please see the R documentation.

--------------------------------------------------------------------------------
### Installing LOLA

The release version of LOLA can be installed directly from Bioconductor:

```{r}
if (!requireNamespace("BiocManager", quietly=TRUE))
    install.packages("BiocManager")
BiocManager::install("LOLA")
```

To install the development version directly from github, make sure you have [GenomicRanges](http://www.bioconductor.org/packages/release/bioc/html/GenomicRanges.html) (bioconductor package) installed, then install LOLA with devtools:
```{r}
if (!requireNamespace("BiocManager", quietly=TRUE))
    install.packages("BiocManager")
BiocManager::install("GenomicRanges")

devtools::install_github("nsheff/LOLA")

```

Or, clone the repo and install from there:
```{r}
install.packages("path/to/LOLA", repos=NULL)
```
--------------------------------------------------------------------------------
### Running LOLA

For examples and workflows for LOLA, please check out the R vignettes.

--------------------------------------------------------------------------------
### LOLA Databases

Downloads of core databases and instructions for building your own databases are at [databio.org/regiondb](http://databio.org/regiondb).

