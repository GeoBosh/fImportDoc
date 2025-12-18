# Split downloaded data sets

Helpful dataset and charvec splitting utilities.

## Usage

``` r
dataSplit(x, split=" ", col=-1)
charvecSplit(x, split=" ", col=1, format="%F")
stringSplit(x, split=" ", col=NULL)
```

## Arguments

- x:

  character vector to be splitted.

- split:

  the split character, by default a blank.

- col:

  an integer value or vector, the column(s) to be selected.

- format:

  the date format of the character vector, by default the ISO-8601 date
  format.

## References

Diethelm Wuertz, Yohan Chalabi, and Andrew Ellis, (2010); *Financial
Market Data for R/Rmetrics*, Rmetrics eBook, Rmetrics Association and
Finance Online, Zurich, www.rmetrics.org.
