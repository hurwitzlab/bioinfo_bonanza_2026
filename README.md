# Introduction to omics analyses with R 
## Two sessions in the Bioinformatics Bonanza 2026 (BRC-NCSU)

Hands-on training workshops on omics data analyses with R for the Bioinformatics Bonanza 2026 at the BRC-NCSU. 
Each workshop is a self-contained, roughly two-hour session —
they build on eachother, so we recommend you take them in the order presented. 

Live documentation: <https://hurwitzlab.github.io/omics_with_R_2026/>

## Workshops

- **Foundations of R with the Tidyverse** ([`r_tidyverse_workshop.qmd`](r_tidyverse_workshop.qmd)) —
  R basics (objects, data types, vectors) and the dplyr core verbs (`filter`,
  `select`, `mutate`, `arrange`, `summarize`), group operations, and a first
  `ggplot2` plot, using the built-in `starwars` dataset.
- **RNA-seq and Transcriptomics** ([`rnaseq_workshop.qmd`](rnaseq_workshop.qmd)) —
  Bulk RNA-seq expression table analysis, differential expression analysis, 
  and interpreting DESeq2 output.

## Rendering

The site is built with [Quarto](https://quarto.org) and requires R with
tidyverse installed.

```bash
quarto render
```

## CI/CD

On every push to `main`, GitHub Actions (`.github/workflows/render-and-deploy.yml`)
installs R and the tidyverse, renders the site with Quarto, and publishes it
to GitHub Pages.
