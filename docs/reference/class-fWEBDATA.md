# Class "fWEBDATA"

The class fWEBDATA represents a time series downloaded from the
internet.

## Objects from the Class

Objects can be created by calls of the import or series functions.

## Slots

- `call`::

  Object of class `"call"`: the call of the applied function.

- `data`::

  Object of class `"data.frame"`: the downloaded data formatted as a
  `"timeSeries"` object.

- `param`::

  Object of class `"character"`: a character vector whose elements
  contain the values of selected parameters of the argument list.

- `title`::

  Object of class `"character"`: a character string with the name of the
  download. This can be overwritten specifying a user defined input
  argument.

- `description`::

  Object of class `" character"`: a character string with an optional
  user defined description. By default just the current date and user
  when the test was applied will be returned.

## Methods

- show:

  `signature(object = "fWEBDATA")`: prints an object of class
  'fWEBDATA'.

## Note

The import and series functions like
[`fredImport`](https://geobosh.github.io/fImportDoc/reference/import-fred.md)
and
[`fredSeries`](https://geobosh.github.io/fImportDoc/reference/import-fred.md)
are typical examples which show how to implement download functions as
simple `timeSeries` objects or as more complicate `fWEBDATA` S4 objects.
Inspect the R code and feel free to create your own download functions
and objects.

## References

Diethelm Wuertz, Yohan Chalabi, and Andrew Ellis, (2010); *Financial
Market Data for R/Rmetrics*, Rmetrics eBook, Rmetrics Association and
Finance Online, Zurich, www.rmetrics.org.

## See also

[`fredImport`](https://geobosh.github.io/fImportDoc/reference/import-fred.md),
[`fredSeries`](https://geobosh.github.io/fImportDoc/reference/import-fred.md),
