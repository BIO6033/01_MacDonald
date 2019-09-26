---
title: "Punaises"
author: "Andrew"
date: "26/09/2019"
output: 
  html_document:
    keep_md: true
---




```r
library(tidyverse)
```


```r
extermin <- read_csv("declarations-exterminations-punaises-de-lit.csv")
```

```
## Parsed with column specification:
## cols(
##   NO_DECLARATION = col_double(),
##   DATE_DECLARATION = col_datetime(format = ""),
##   DATE_INSP_VISPRE = col_date(format = ""),
##   NBR_EXTERMIN = col_double(),
##   DATE_DEBUTTRAIT = col_date(format = ""),
##   DATE_FINTRAIT = col_date(format = ""),
##   No_QR = col_character(),
##   NOM_QR = col_character(),
##   NOM_ARROND = col_character(),
##   COORD_X = col_double(),
##   COORD_Y = col_double(),
##   LONGITUDE = col_double(),
##   LATITUDE = col_double()
## )
```

```r
head(extermin)
```

```
## # A tibble: 6 x 13
##   NO_DECLARATION DATE_DECLARATION    DATE_INSP_VISPRE NBR_EXTERMIN
##            <dbl> <dttm>              <date>                  <dbl>
## 1           4254 2012-10-28 16:36:04 2012-09-21                  1
## 2            830 2011-09-16 09:45:58 2011-07-13                  1
## 3           1380 2011-11-08 14:01:04 2011-11-02                  1
## 4            455 2011-08-10 09:53:47 2011-08-09                  1
## 5           1243 2011-10-26 10:11:32 2011-09-16                  1
## 6           4331 2012-11-08 14:23:14 2012-10-10                 NA
## # … with 9 more variables: DATE_DEBUTTRAIT <date>, DATE_FINTRAIT <date>,
## #   No_QR <chr>, NOM_QR <chr>, NOM_ARROND <chr>, COORD_X <dbl>,
## #   COORD_Y <dbl>, LONGITUDE <dbl>, LATITUDE <dbl>
```


