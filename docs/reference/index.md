# Package index

## Overview of package fImport

- [`fImport-package`](00fImport-package.md)
  [`fImport`](00fImport-package.md) : Import data from the web

## Import data from internet

Currently, only the FRED database is supported. The listings from the
stock markets should still be useful but have not been updated for
years.

- [`fredSeries()`](import-fred.md) [`fredImport()`](import-fred.md) :
  Import Market Data from the Federal Reserve Database
- [`providerListings`](provider-listings.md)
  [`amexListing`](provider-listings.md)
  [`h15Listing`](provider-listings.md)
  [`nasdaqListing`](provider-listings.md)
  [`nyseListing`](provider-listings.md)
  [`oandaListing`](provider-listings.md)
  [`stoxxListing`](provider-listings.md)
  [`swxListing`](provider-listings.md) : Provider Listing of Symbols and
  Descriptions

## class fWEBDATA

- [`fWEBDATA-class`](class-fWEBDATA.md) : Class "fWEBDATA"
- [`show-methods`](methods-show.md)
  [`show,fWEBDATA-method`](methods-show.md) : WEBDATA Download Show
  Methods

## Utilities

- [`composeURL()`](utils-download.md) [`indexGrep()`](utils-download.md)
  : Utilities for composing URL's
- [`dataSplit()`](utils-split.md) [`charvecSplit()`](utils-split.md)
  [`stringSplit()`](utils-split.md) : Split downloaded data sets

## Read webpages using a browser

- [`read.links()`](read-links.md) : Links Browser interface
- [`read.lynx()`](read-lynx.md) : Lynx Browser interface
- [`read.w3m()`](read-w3m.md) : w3m Browser interface
- [`read.lines()`](read-lines.md) : Read from a text file line by line
