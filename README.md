This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

In their paper "History and Industry Location: Evidence from German Airports" the authors Stephen J. Redding, Daniel M. Sturm and Nikolaus Wolf developed a body of evidence that the relocation of Germany´s air hub frum Berlin to Frankfurt in response to division is a shift between multiple steady states.

The paper can be found under the following link:
https://dataverse.harvard.edu/dataset.xhtml?persistentId=hdl:1902.1/17402

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.
```s
if (!require(devtools))
  install.packages("devtools")
source_gist("gist.github.com/skranz/fad6062e5462c9d0efe4")
install.rtutor(update.github=TRUE)

devtools::install_github("pl90/RTutorAirports", upgrade_dependencies=FALSE)
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.
```s
library(RTutorAirports)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorAirports")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorAirports",
       load.sav=TRUE, sample.solution=FALSE)
```
If everything works fine, a browser window should open, in which you can start exploring the problem set.
