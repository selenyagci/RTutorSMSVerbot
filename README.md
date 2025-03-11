This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

--- Add **brief** description of content and link to original paper ---

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.
```s
install.packages("RTutor",repos = c("https://skranz-repo.github.io/drat/",getOption("repos")))

if (!require(devtools))
  install.packages("devtools")

devtools::install_github("selenyagci/RTutorSMSVerbot")
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.
```s
library(RTutorSMSVerbot)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorSMSVerbot")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorSMSVerbot",
       auto.save.code=TRUE, clear.user=FALSE)
```
If everything works fine, a browser window should open, in which you can start exploring the problem set.
