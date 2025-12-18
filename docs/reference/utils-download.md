# Utilities for composing URL's

Two helpful utilities for assembling URL's.

## Usage

``` r
composeURL(..., prefix="http://")
indexGrep(pattern, x, ...)
```

## Arguments

- ...:

  for `composeURL`, character strings from which the URL will be
  composed; for `indexGrep`, optional arguments to be passed to the
  function `grep`.

- prefix:

  a character string specifying the prefix of the URL.

- pattern:

  a character string containing a regular expression to be matched in
  the given character vector.

- x:

  a character vector where matches are sought.

## References

Diethelm Wuertz, Yohan Chalabi, and Andrew Ellis, (2010); *Financial
Market Data for R/Rmetrics*, Rmetrics eBook, Rmetrics Association and
Finance Online, Zurich, www.rmetrics.org.
