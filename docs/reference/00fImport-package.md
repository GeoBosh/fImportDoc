# Import data from the web

The Rmetrics "fImport" package is a collection of utility functions to
download and manage data sets from the Internet or from other sources.

## 1 Introduction

The major content of this package is to provide download functions for
financial market data from the Internet. For this we have implemented
the web text browsers "Lynx", "Links", and "W3M" for an easy and
straightforward download of data from the Internet.

Furthermore helpful utility functions are included to split numerical
data matrices, to split date character vectors, and to split strings
from downloads. This allows to create in a very easy way `timeSeries`
objects.

Examples are provided for downloading data from the Federal Reserve data
base in St. Louis web portal.

The data part contains instruments listings from the American Stock
Exchange, from the FED H15 Report, from the NASDAQ Stock Market, from
the New York Stock Exchange, of OANDAs Foreign Exchange Rates, of STOXX
Indices, and from the Swiss Stock Exchange.

For the download of spread sheets from the Internet we refer to the
functions `gdata::read.xls` and `xlsx::read.xlsx` for the contributed R
packages `gdata` and `xlsx` respectively.

## 2 Download Functions

The package makes functions available to download financial market data
from the internet. Currently functions are available for the follwing
web sites. The functions are:

        fredSeries      downloads data from research.stlouisfed.org
        fredImport      downloads data from research.stlouisfed.org
        
        
        

The economic and financial time series data are extracted as objects of
class `"timeSeries"`.

## 3 Readers and Web downloaders

The package comes with the following tailored readers and web
downloaders:

        read.lines      a synonym function call to readLines
        read.links      uses the links browser to read from a web page
        read.lynx       uses the lynx browser to read from a web page
        read.w3m        uses the w3m browser to read from a web page
        

## 4 Split Function Utilities

This section provides functions to split numerical data matrices, to
split date character vectors, and to split strings from downloads:

        dataSplit       splits a data matrix from a downloaded file
        charvecSplit    splits a charvec vector from a downloaded file
        stringSplit     splits a string vector from a downloaded file
        

## About Rmetrics

The `fImport` Rmetrics package is written for educational support in
teaching "Computational Finance and Financial Engineering" and licensed
under the GPL.
