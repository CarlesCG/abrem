## Abrem 
From [openreliability.org](http://www.openreliability.org/index.html): "The R package 'abrem', a contraction of Abernethy Reliability Methods, is a rework of the original weibulltoolkit package now calling technical functions from pivotals (in future to be abremPivotals) and debias (to become abremDebias).""



## Installation
- R-Forge  
```
install.packages("abrem",repos="http://R-Forge.R-project.org")
```
- GitHub & R-Forge  
```
# Load or install devtools
ifelse(!require(devtools),
  install.packages("devtools", type = "source"),
  library(devtools) ) 
# Install from both sources
install_github( "Abernethy/abremPivotals@dev-public")
install_github( "Abernethy/abremDebias")
install_url("http://download.r-forge.r-project.org/src/contrib/debias_0.1.9.tar.gz")
install_github( "Abernethy/abrem@dev-public")
```
**IMPORTANT NOTES!**  
1. MAC OS X: gfortran dependencies. In order to get lgfortran for Mac OS. Execute at the terminal 
```
curl -O http://r.research.att.com/libs/gfortran-4.8.2-darwin13.tar.bz2
sudo tar fvxz gfortran-4.8.2-darwin13.tar.bz2 -C /
```
2. GitHub version broken  
As it is today the GitHub version have some breakage as is discuss at the [Issue #1](https://github.com/Abernethy/abrem/issues/1) of the original package 

## Learning abrem
- As is today the best way to get started is to follow the code and exmaples at [Using abrem](http://www.openreliability.org/HTML/using_abrem.html) at the openreliability.org webpage. 
- Checkout this old papers using the predecesor package *'weibulltoolkit'*:  
-- ["Weibull Analysis Using R, in a Nutshell"](http://www.openreliability.org/downloads/intro.pdf)  
-- ["Monte Carlo Pivotal Confidence Bounds For Weibull Analysis, With Implementations in R"](http://www.openreliability.org/downloads/MCpivotalbounds.pdf)


##About Openreliability.org  
"Openreliability is dedicated to the development of reliability engineering and operations research applications software under the open source paradigm.
As open source we invite a vigorous peer review of the technical accuracy of the software code in use. An open dialog on the use and application of this software is also encouraged. We appreciate your involvement on any level.
Our first and most active project is Abernethy Reliability Methods based on "The New Weibull Handbook, Fifth Edition", by Robert B. Abernethy. This reference has been the textbook for a Weibull Analysis course that has successfully trained quality and reliability engineers for over three decades."

## Author
Jurgen Symynck <jusy@openreliability.org>     

## License 
GPL-3