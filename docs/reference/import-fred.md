# Import Market Data from the Federal Reserve Database

Imports financial time series data from fred.stlouisfed.org.

## Usage

``` r
fredSeries(symbols, from = NULL, to = Sys.timeDate(), 
    nDaysBack = 366, ...)
    
fredImport(query, file = "tempfile", source = NULL, frequency = "daily", 
    from = NULL, to = Sys.timeDate(), nDaysBack = NULL,
    save = FALSE, sep = ";", try = TRUE)
```

## Arguments

- symbols:

  a character string with the symbols to be downloaded.

- from:

  the start date of the time series to extract.

- to:

  the end date of the data download, by default the current date.

- nDaysBack:

  the number of days back.

- ...:

  optional arguments to be passed to `fredImport`.

- query:

  a character string, denoting the location of the data at the web site.

- file:

  where to save the downloaded data, a character string with filename,
  usually having extension ".csv".

- source:

  a character string setting the URL of the source. If `NULL`, then the
  URL will be set automatically to its default value.

- frequency:

  a character string, one of `"auto"`, `"quarterly"`, `"monthly"`, or
  `"daily"`, defining the frequency of the data records. Only needed if
  the import function fails to autodetect the frequency of the time
  series to be dowwnloaded.

- save:

  a logical value, if set to `TRUE` the downloaded data file will be
  stored under the path and file name specified by the string `file`. By
  default FALSE.

- sep:

  a character value specifying the column separator.

- try:

  a logical value, if set to TRUE the Internet access will be checked.

## Value

for `fredSeries`, an object of class `timeSeries`.

for `fredImport`, an object of class `fWEBDATA` with the following
slots:

- @call:

  the function call.

- @data:

  the downloaded data as an object from class `"timeSeries"`.

- @param:

  a character vector whose elements contain the values of selected
  parameters of the argument list.

- @title:

  a character string with the name of the download. This can be
  overwritten specifying a user defined input argument.

- @description:

  a character string with an optional user defined description. By
  default just the current date when the test was applied will be
  returned.

## Note

**Internet Download Functions:**

IMPORTANT NOTE: If the service provider changes the data file format it
may become necessary to modify and update the functions.

Feel free to inspect the code of the functions and to create your own
download function from other Internet web sites and Portals.

## Author

Diethelm Wuertz for the Rmetrics R-port.

## References

Diethelm Wuertz, Yohan Chalabi, and Andrew Ellis, (2010); *Financial
Market Data for R/Rmetrics*, Rmetrics eBook, Rmetrics Association and
Finance Online, Zurich, www.rmetrics.org.

## Examples

``` r
# \donttest{
a <- fredImport("DEXSZUS")
#> Loading required namespace: rvest
head(a@data)  # a@data is a "timeSeries" object
#> GMT 
#>            DEXSZUS
#> 1971-01-04  4.3180
#> 1971-01-05  4.3117
#> 1971-01-06  4.3113
#> 1971-01-07  4.3103
#> 1971-01-08  4.3109
#> 1971-01-11  4.3102

b <- fredSeries("DEXSZUS")
head(b) # a "timeSeries" object
#> GMT 
#>      DEXSZUS
# }
```
