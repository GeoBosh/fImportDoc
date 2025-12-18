# Links Browser interface

Uses the Links Text Browser to read a web page.

## Usage

``` r
read.links(url, intern = TRUE, bin = NULL, pipe = FALSE, ...)
```

## Arguments

- url:

  a character string specifying the URL of the web page.

- intern:

  a logical which indicates whether to make the output of the command an
  R object.

- bin:

  a string with the path of your lynx binary or NULL if lynx binary is
  available in the operating system path.

- pipe:

  a logical which indicates whether the result should be returned as a
  [`pipe()`](https://rdrr.io/r/base/connections.html) commmand.

- ...:

  optional arguments passed to links binary.

## Value

the downloaded text

## References

Diethelm Wuertz, Yohan Chalabi, and Andrew Ellis, (2010); *Financial
Market Data for R/Rmetrics*, Rmetrics eBook, Rmetrics Association and
Finance Online, Zurich, www.rmetrics.org.

## See also

Alternative text browser functions are the Rmetrics functions
[`read.lynx`](https://geobosh.github.io/fImportDoc/reference/read-lynx.md)
and
[`read.w3m`](https://geobosh.github.io/fImportDoc/reference/read-w3m.md).

To download `xls` and `xlsx` spread sheets use the functions
`gdata::read.xls` and `xlsx::read.xlsx` from the contributed packages
`gdata` and `xlsx`, respectively.

To download text files line by line use the Rmetrics function
[`read.lines`](https://geobosh.github.io/fImportDoc/reference/read-lines.md)
which wraps the function `readLines` from R's base evironment.

To postprocess downloaded files use the Rmetrics functions
[`indexGrep`](https://geobosh.github.io/fImportDoc/reference/utils-download.md),
[`dataSplit`](https://geobosh.github.io/fImportDoc/reference/utils-split.md),
[`charvecSplit`](https://geobosh.github.io/fImportDoc/reference/utils-split.md),
and
[`stringSplit`](https://geobosh.github.io/fImportDoc/reference/utils-split.md).
