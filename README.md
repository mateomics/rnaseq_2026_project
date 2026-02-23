# RNA-seq 2026 course 

> RNA-seq Analysis from recount3

RNA-seq differential expression analysis project using publicly available data from recount3.

## Project Overview

This repository contains an RNA-seq analysis workflow developed as part of Dr. Leonardo Collado's LCG22 course project (UNAM). The dataset analyzed corresponds to:

- **Dataset:** SRP068976  
- **Platform:** recount3  

The objective of this project is to explore gene expression patterns and perform downstream analyses using reproducible bioinformatics workflows.

---

## Repository Structure

```
.
├── images
│   ├── heatmap.png
│   ├── MA_plot.png
│   ├── mds.png
│   ├── QC_boxplot.png
│   ├── QC_histogram.png
│   ├── volcano_plot.png
│   └── voom_plot.png
├── LICENSE
├── R
│   ├── report_files
│   │   ├── figure-html
│   │   │   ├── unnamed-chunk-15-1.png
│   │   │   ├── unnamed-chunk-16-1.png
│   │   │   ├── unnamed-chunk-20-1.png
│   │   │   ├── unnamed-chunk-23-1.png
│   │   │   ├── unnamed-chunk-23-2.png
│   │   │   ├── unnamed-chunk-24-1.png
│   │   │   └── unnamed-chunk-25-1.png
│   │   └── libs
│   │       ├── bootstrap
│   │       │   ├── bootstrap-0cf178164be81c6ad854e95b21275c80.min.css
│   │       │   ├── bootstrap-icons.css
│   │       │   ├── bootstrap-icons.woff
│   │       │   └── bootstrap.min.js
│   │       ├── clipboard
│   │       │   └── clipboard.min.js
│   │       └── quarto-html
│   │           ├── anchor.min.js
│   │           ├── axe
│   │           │   └── axe-check.js
│   │           ├── popper.min.js
│   │           ├── quarto.js
│   │           ├── quarto-syntax-highlighting-ed96de9b727972fe78a7b5d16c58bf87.css
│   │           ├── tabsets
│   │           │   └── tabsets.js
│   │           ├── tippy.css
│   │           └── tippy.umd.min.js
│   └── report.qmd
├── README.md
├── references.bib
└── results
    ├── report.html
    └── report.pdf

```

---

## Requirements

- R (≥ 4.3 recommended)
- Quarto
- Required R packages:
  - recount3
  - DESeq2
  - tidyverse
  - SummarizedExperiment
  - ggplot2

Install packages in R:

```r
install.packages("tidyverse")
BiocManager::install(c("recount3", "DESeq2", "SummarizedExperiment"))
```

## How to reproduce my analysis
1. Clone my repository (`git clone https://github.com/mateomics/rnaseq_2026_project`)
2. Render the `.qmd` file on your new repository (`quarto render report.qmd`)

## What does the report includes?

The rendered report includes:

- Data acquisition

- Preprocessing

- Exploratory analysis

- Differential expression analysis

- Visualization of results

## Author

Mateo Jimenez-Sotelo
B.Sc. in Genomic Sciences, LCG, UNAM
February 2026