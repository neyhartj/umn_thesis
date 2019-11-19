# `umn_thesis` BookDown Template

## Description

This repository provides a template for compiling, using R Markdown, a thesis with formatting that is compliant with the requirements from the Graduate School of the University of Minnesota.


## Installation

### Step 1. Ensure relevant R packages are installed

Before using this template, the following R packages are required: `bookdown`, `rmarkdown`, `tidyverse`,
`knitr`, and `kableExtra`.

These packages can be installed simultaneously by running this code:

```
install.packages(c("bookdown", "rmarkdown", "tidyverse", "knitr", "kableExtra"))

```


### Step 2. Start a new project in RStudio

You can install this package by starting a new project in RStudio. The simplest method is to create a new project by cloning the GitHub repository containing this template. To do this in RStudio, go to `File` > `New Project` > `Version Control` > `Git` and fill out the information as such:

```
Repository URL: https://github.com/neyhartj/umn_thesis
```

The Project directory name should autofill with the repository name (i.e. `umn_thesis`). You can customize this and the directory for which this new project will be a subdirectory.

Next, click `Create Project`.
