# CleanR
This package cleans a dataset and returns summary statistics as well as number, proportion and location of NA values for string and number column inputs. Data cleaning made easy!

### Collaborators
Heather Van Tassel, Phuntsok Tseten, Patrick Tung

## Overview
There is a dire need for a good data cleaning package, and we are trying to develop our version of a good data cleaning package that will help users clean their data in a meaningful way. Data cleaning is usually the first step in any data science problem, and if you don’t clean your data well, it might be really difficult to proceed further. So our motivation for coming up with this idea was to address this very issue of messy data.

CleanR is especially developed to create a streamlined process to give you an easy to read summary statistics table about your data. CleanR is able to easily locate all the missing data for you and allow you to locate where exactly it occurs. Not only are you able to locate missing data, you can also define how you would like to deal with your missing data. 

## Functions
**Function 1)**


**Function 2)** `locate_na`: Returns a list of the count and indices of NA values.  This function takes in a dataframe and finds NA values and returns the location of these missing values.

```
#' Locate NAs
#'
#' @description
#' Locate and return the indices to all missing values within an inputted dataframe.
#' Each element of the returned list will be a column in a dataframe, which will hold
#' the row indices of the missing values.
#'
#' @param data (tbl_df, df, data.frame) dataframe that the function will use to locate NAs
#'
#' @return a list containing indices of missing values
#' @export

locate_na <- function(data) {

}

```

**Function 3)**`replace_na`:Replaces missing NA values with either min, max, median, or average (default) values of the column(s). There will be an option to remove the rows with NAs.
```
#' `replace_na`
#' @description
#'This function replaces na values with either the min, max, #'median or average value or removes the rows.

#' @param input_df dataframe, dataframe that the  function #'will use to replace NAs.

#' @returns
#'A list of tuples where each NAs will be replaced by either #'min, max, median or average.
#'Each tuple in the list represents  the indices of a NA in #'the dataframe. 
   
#' @exports
#' replace_na<- input_df %>% 
        group_by(input_df) %>% 
        summarize(input_df)
```

## CleanR and R's Ecosystem
Sometimes it can get quite annoying dealing with data, so it is always nice to get some information about a quick summary of the data. A similar function in R that is implemented is the `summary()` function. CleanR's `summary()` function is very similar in the sense that it also produces summary statistics, but presented in a much more intuitive manner. Our `summary()` function also has more information such as the number of missing values, as well as provide summaries of text information. In regards to our `locate_na()` and `replace_na()`, there is no similar function created in the current R ecosystem that we know of. The only way to do this is to mannually combine a few functions including `is.na()`.

## Installation
*Will be developed next milestone*

You can install the released version of CleanR from [CRAN](https://CRAN.R-project.org) with:

``` r
install.packages("CleanR")
library(CleanR)
```

## R Dependencies

# Do we have any??
