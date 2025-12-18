# Read from a text file line by line

Reads from a text file line by line. Wrapper to readLines() function.

## Usage

``` r
read.lines(con=stdin(), n=-1, ok=TRUE, warn=FALSE, encoding="unknown")
```

## Arguments

- con:

  a connection object or a character string.

- n:

  an integer, the (maximal) number of lines to read. Negative values
  indicate that one should read up to the end of input on the
  connection.

- ok:

  a logical, is it OK to reach the end of the connection before n \> 0
  lines are read? If not, an error will be generated.

- warn:

  a logical, warn if a text file is missing a final EOL. The default is
  FALSE, note different from function `readLines`.

- encoding:

  a character string, the encoding to be assumed for input strings.

## Value

the downloaded text. Same output as readLines() function.

## References

Diethelm Wuertz, Yohan Chalabi, and Andrew Ellis, (2010); *Financial
Market Data for R/Rmetrics*, Rmetrics eBook, Rmetrics Association and
Finance Online, Zurich, www.rmetrics.org.
