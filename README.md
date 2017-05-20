This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

The problem set "The Effect of the Tsetse on African development" takes the reader on a economic journey through the same-named paper by Marcella Alsan (2015).
The original paper can be found on https://www.aeaweb.org/articles?id=10.1257/aer.20130604
The economic findings, analytic steps and explanations of the development economic theory behind it are described in an interactive way. 

To install RTutor and work on the problem set you follow these steps:

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.
```s
if (!require(devtools))
  install.packages("devtools")
source_gist("gist.github.com/skranz/fad6062e5462c9d0efe4")
install.rtutor(update.github=TRUE)

devtools::install_github("vanessaschoeller/RTutorTseTse", upgrade_dependencies=FALSE)
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.
```s
library(RTutorTseTse)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorTseTse")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorTseTse",
       load.sav=TRUE, sample.solution=FALSE)
```
If everything works fine, a browser window should open, in which you can start exploring the problem set.
