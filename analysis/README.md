Homework 2
================

Step-by-step instructions to re-create Lecture 3 analyses
=========================================================

Import tidyverse
----------------

``` r
library(tidyverse)
```

    ## -- Attaching packages ----------------------------------------------------------------------------------------------------------------------------------- tidyverse 1.2.1 --

    ## v ggplot2 3.0.0     v purrr   0.2.5
    ## v tibble  1.4.2     v dplyr   0.7.6
    ## v tidyr   0.8.1     v stringr 1.3.1
    ## v readr   1.1.1     v forcats 0.3.0

    ## -- Conflicts -------------------------------------------------------------------------------------------------------------------------------------- tidyverse_conflicts() --
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

Read the TSV file
-----------------

``` r
data <- read_tsv("https://github.com/gboyle2/tfcb-homework2/tree/master/data") %>% 
  print()
```

    ## Parsed with column specification:
    ## cols(
    ##   `<!DOCTYPE html>` = col_character()
    ## )

    ## # A tibble: 567 x 1
    ##    `<!DOCTYPE html>`                                                       
    ##    <chr>                                                                   
    ##  1 <!DOCTYPE html>                                                         
    ##  2 "<html lang=\"en\">"                                                    
    ##  3 <head>                                                                  
    ##  4 "<meta charset=\"utf-8\">"                                              
    ##  5 "<link rel=\"dns-prefetch\" href=\"https://assets-cdn.github.com\">"    
    ##  6 "<link rel=\"dns-prefetch\" href=\"https://avatars0.githubusercontent.c~
    ##  7 "<link rel=\"dns-prefetch\" href=\"https://avatars1.githubusercontent.c~
    ##  8 "<link rel=\"dns-prefetch\" href=\"https://avatars2.githubusercontent.c~
    ##  9 "<link rel=\"dns-prefetch\" href=\"https://avatars3.githubusercontent.c~
    ## 10 "<link rel=\"dns-prefetch\" href=\"https://github-cloud.s3.amazonaws.co~
    ## # ... with 557 more rows
