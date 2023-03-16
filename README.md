# Overview

Presto performs a fast Wilcoxon rank sum test and auROC analysis. Latest benchmark ran 1 million observations, 1K features, and 10 groups in 16 seconds (sparse input) and 85 seconds (dense input). 


# Installation

Install presto from CRAN:

```{r}
install.packages('presto')
```

# Usage

Run presto on a matrix, Seurat, or SingleCellExperiment input object. 

```
wilcoxauc(X, y)
wilcoxauc(seurat_object, 'group_name')
wilcoxauc(sce_object, 'group_name')
```

For examples, see `?wilcoxauc` and the [vignette](https://rdrr.io/github/immunogenomics/presto/f/vignettes/getting-started.Rmd)
