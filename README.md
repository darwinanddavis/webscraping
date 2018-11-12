# Webscraping with `R`  

### Matthew Malishev<sup>1*</sup>

##### _<sup>1</sup> Department of Biology, Emory University, 1510 Clifton Road NE, Atlanta, GA, USA, 30322_    

##### *Corresponding author: matthew.malishev@gmail.com  

:link: [Link to Github](https://github.com/darwinanddavis)    

File extensions:   
.R  
.Rmd     
.pdf  
.html  

******  

## Overview      

This document outlines useful tools for webscraping with `R`, including how to use xpaths, navigating XML and JSON, and useful `R` packages.  

## Initial steps  
1. Search CRAN for packages that access the API for the site for webscraping, e.g. search 'Spotify' for `Rspotify` package.  
2. Use `rvest` or `rjson` to scrape.    
3. Use `regex` functions to parse text blocks.  

## Selecting individual webpage elements  

xpath finder: webpage plugin to isolate HTML elements, e.g. tables on webpage and turn them into XML. Once passed to `R`, packages like `rvest` scrape only that XML element. 

Use `tidytext` in R to parse and clean scraped text.    

## Geocodes    
1. Use Google API to get geocode values from webpage.  
2. Run xpath expression to isolate the geocode values e.g "XML parse" function.  

## PubMed 
Search pubmed in `R` package on CRAN.  
Use the HTML element web app to find which HTML elements of the page you want to scrape, e.g. <a> = link.  
To scrape the pure text of i.e. just abstract text without the author and affiliation text lines, but across multiple web pages, use the XML search home page to search for and apply an xpath term, e.g. 'abstracttextonly'.  

### How to programmatically bypass the 'Show more results' button on webpages  
1. Use `RSelenium` package.  
2. Find the HTML element on the webpage for the 'Show More' button and access this XML path using the package.    




## References  

[Webscraping with R, Steve Pittard](https://steviep42.github.io/webscraping/book/)  

## Maintainer  
**Matt Malishev**   
:mag: [Website](https://www.researchgate.net/profile/Matt_Malishev)    
:bird: [@darwinanddavis](https://twitter.com/darwinanddavis)  
:email: matthew.malishev [at] gmail.com    
