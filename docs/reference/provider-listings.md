# Provider Listing of Symbols and Descriptions

CSV files with provider listings of symbols, descriptions ands related
information.

The listings include those from:

|               |                                          |
|---------------|------------------------------------------|
| amexListing   | Listing from the American Stock Exchange |
| h15Listing    | Listing from the FED H15 Report          |
| nasdaqListing | Listing from the NASDAQ Stock Market     |
| nyseListing   | Listing from the New York Stock Exchange |
| oandaListing  | Listing of OANDAs Foreign Exchange Rates |
| stoxxListing  | Listing of STOXX Indices                 |
| swxListing    | Listing from the Swiss Stock Exchange    |

## Format

All files are given in CSV Excel spreadsheet format. The delimiter is a
semicolon.

## References

Diethelm Wuertz, Yohan Chalabi, and Andrew Ellis, (2010); *Financial
Market Data for R/Rmetrics*, Rmetrics eBook, Rmetrics Association and
Finance Online, Zurich, www.rmetrics.org.

## Examples

``` r
data(package = "fImport")

head(h15Listing)
#>            Symbol                Description
#> 1     H15_NFCP_M2    CommercialPaper2MNonFin
#> 2     H15_NFCP_M3    CommercialPaper3MNonFin
#> 3      H15_FCP_M1 CommercialPaper1MFinancial
#> 4      H15_FCP_M2 CommercialPaper2MFinancial
#> 5      H15_FCP_M3 CommercialPaper3MFinancial
#> 6 H15_CPFFWOUT_M3   CP3MCPFFwithoutsurcharge
head(nyseListing)
#>   Symbol                         Name MarketCap Exchange
#> 1      A   Agilent Technologies, Inc. $12,852.3     NYSE
#> 2     AA                   Alcoa Inc. $28,234.5     NYSE
#> 3    AAI       AirTran Holdings, Inc.    $156.9     NYSE
#> 4    AAP       Advance Auto Parts Inc  $3,507.4     NYSE
#> 5    AAR              AMR CORPORATION     $81.7     NYSE
#> 6    AAV ADVANTAGE ENERGY INCOME FUND  $1,674.4     NYSE
```
