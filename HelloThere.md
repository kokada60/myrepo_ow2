HelloThere
================
Ken
11/10/2020

Hello Hello This is my very first R Markdown line composed entirely on
my own. Yay\!\!

``` r
library(tidyverse)
```

    ## -- Attaching packages ----------------------------------------- tidyverse 1.3.0 --

    ## v ggplot2 3.3.2     v purrr   0.3.4
    ## v tibble  3.0.4     v dplyr   1.0.2
    ## v tidyr   1.1.2     v stringr 1.4.0
    ## v readr   1.4.0     v forcats 0.5.0

    ## -- Conflicts -------------------------------------------- tidyverse_conflicts() --
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
ae_uk <- read_csv("data/ae_uk.csv", col_names = TRUE)
```

    ## 
    ## -- Column specification ----------------------------------------------------------
    ## cols(
    ##   gender = col_character(),
    ##   type_injury = col_character(),
    ##   arrival_time = col_character()
    ## )

``` r
ae_uk
```

    ## # A tibble: 773,779 x 3
    ##    gender type_injury arrival_time 
    ##    <chr>  <chr>       <chr>        
    ##  1 male   minor       1/1/2010 0:35
    ##  2 male   minor       1/1/2010 0:57
    ##  3 male   minor       1/1/2010 0:42
    ##  4 male   minor       1/1/2010 0:02
    ##  5 male   minor       1/1/2010 0:24
    ##  6 female major       1/1/2010 0:48
    ##  7 female minor       1/1/2010 0:10
    ##  8 male   minor       1/1/2010 0:39
    ##  9 female minor       1/1/2010 0:56
    ## 10 female minor       1/1/2010 0:05
    ## # ... with 773,769 more rows
