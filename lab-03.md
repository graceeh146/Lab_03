Lab 03 - Nobel laureates
================
Enhui Wang
2025.1.23

### Load packages and data

``` r
library(tidyverse) 
```

``` r
nobel <- read_csv("data/nobel.csv")
```

## Exercises

### Exercise 1

Nobel has 935 observations and 26 variables.Each row presents a Nobel
laureate such as names, the year they won,biographical information, and
etc.

``` r
nrow(nobel)#the number of rows (observations)
```

    ## [1] 935

``` r
ncol(nobel)#the number of columns (variables)
```

    ## [1] 26

### Exercise 2

``` r
nobel_living <- nobel %>%
  filter(!is.na(country),#laureates for whom country is available
  gender != "org", #exclude organizations
  is.na (died_date))# still live people

#check the number of observations
nrow(nobel_living)
```

    ## [1] 228

### Exercise 3

Remove this text, and add your answer for Exercise 1 here. Add code
chunks as needed. Don’t forget to label your code chunk. Do not use
spaces in code chunk labels.

### Exercise 4

…

### Exercise 5

…

### Exercise 6

…
