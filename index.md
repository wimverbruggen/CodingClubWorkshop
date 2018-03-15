# EVENET Code Club Workshop
## Wim Verbruggen

## 1. Import the data and load the libraries

```r
# Get data
load("traits.RData")
load("traits_sum.RData")

# Load libraries
library(corrplot)
library(ggplot2)
```

### 2. Plot trait correlations

```r
(correlation <- corrplot(cor(traits[,2:5], use = "pairwise.complete.obs")))
```