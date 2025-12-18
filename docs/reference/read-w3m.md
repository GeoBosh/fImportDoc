# w3m Browser interface

Uses the w3m Browser to read a web page.

## Usage

``` r
read.w3m(url, intern = TRUE, bin = NULL, pipe = FALSE, ...)
```

## Arguments

- url:

  a character string specifying the URL of the web page.

- intern:

  a logical which indicates whether to make the output of the command an
  R object.

- bin:

  a string with the path of your w3m binary or NULL if w3m binary is
  available in the operating system path.

- pipe:

  a logical which indicates whether the result should be returned as a
  [`pipe()`](https://rdrr.io/r/base/connections.html) commmand.

- ...:

  optional arguments passed to w3m binary. For a list of options, see
  the w3m manual page.

## Value

the downloaded text

## References

Diethelm Wuertz, Yohan Chalabi, and Andrew Ellis, (2010); *Financial
Market Data for R/Rmetrics*, Rmetrics eBook, Rmetrics Association and
Finance Online, Zurich, www.rmetrics.org.

## See also

Alternative text browser functions are the Rmetrics functions
[`read.links`](read-links.md) and [`read.lynx`](read-lynx.md).

To download `xls` and `xlsx` spread sheets use the functions
`gdata::read.xls` and `xlsx::read.xlsx` from the contributed packages
`gdata` and `xlsx`, respectively.

To download text files line by line use the Rmetrics function
[`read.lines`](read-lines.md) which wraps the function `readLines` from
R's base evironment.

To postprocess downloaded files use the Rmetrics functions
[`indexGrep`](utils-download.md), [`dataSplit`](utils-split.md),
[`charvecSplit`](utils-split.md), and [`stringSplit`](utils-split.md).
