## Repository for the Team Kendra project from the February 2015 CodeAcross hackathon

### R Prototype

The R prototype uses the Socrata API to pull data about a single property from http://data.cityofboston.gov.
There are two versions of the prototype. `BostonAddressLookup.Rmd` is a standalone R Markdown file that 
displays data on a hard-coded address. `BostonAddressLookupShiny.Rmd` is an R Markdown file that uses the `shiny` 
package to create an interactive web page where different addresses may be tried.

Both R prototypes require several R packages including `leaflet`, `stringr`, `RSocrata` and the supporting packages for R Markdown.
`leaflet` should be installed with `devtools::install_github('rstudio/leaflet)`. `RSocrata` should be installed with 
`devtools::install_github('kent37/RSocrata)`. Other packages are available from CRAN. Note: as of this writing, the Chicago 
RSocrata package has a bug which prevents it from retrieving empty records containing date fields. This is fixed in the kent37 version.
See https://github.com/Chicago/RSocrata/issues/24.