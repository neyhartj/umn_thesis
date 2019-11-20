# `umn_thesis` Bookdown Template

## Description

This repository provides a template for compiling, using R Markdown, a thesis with formatting that is compliant with the requirements from the Graduate School of the University of Minnesota. This template relies on [bookdown](https://bookdown.org/) and follows the same typsetting format specified by [`rmarkdown`](https://rmarkdown.rstudio.com/).


## Installation

### Step 1. Ensure relevant R packages are installed

Before using this template, the following R packages are required: `bookdown`, `rmarkdown`, `tidyverse`,
`knitr`, and `kableExtra`.

These packages can be installed simultaneously by running this code:

```
install.packages(c("bookdown", "rmarkdown", "tidyverse", "knitr", "kableExtra"))

```

### Step 2. Install additional software for compiling LaTeX 

The `umn_thesis` template compiles a book into a PDF. If you are using a Windows operating system, you will need to install a LaTeX compiler. [MiKTeX](https://miktex.org/download) is a good option.

> Note: If using MiKTeX, you will need to allow it to install packages on-the-fly. To do this (after installing MiKTeX), open the MiKTeX Console, go to Settings, and select the "Always install missing packages on-the-fly" radio button. 



## Getting started

### Step 1. Create a new project

To create a new bookdown project using the `umn_thesis` template, you need to create a new project in RStudio

#### Option A. Use Git

The simplest method to create a new project is by cloning the GitHub repository containing this template. To do this in RStudio, go to `File` > `New Project` > `Version Control` > `Git` and fill out the information as such:

```
Repository URL: https://github.com/neyhartj/umn_thesis
```

The Project directory name should autofill with the repository name (i.e. `umn_thesis`). You can customize this and the directory for which this new project will be a subdirectory.

Next, click `Create Project`.


#### Option B. Download the ZIP file

Instead of using Git, you can also simply download the `.zip` file containing the `umn_template` repository and create a new project within the unzipped folder.

1. On the GitHub page for this project, click the green `Clone or download` button. Then click `Download ZIP`.
2. After the ZIP file downloads, move it to the directory of your choosing, and unzip the file.
3. In RStudio, go to `File` > `New Project` > `Existing Directory` and navigate to the folder created after unzipping the ZIP file.


#### Project folder orientation

After creating the project, you will have a directory with many different folders and files. Here is a breakdown of what each is for:


| Folder/file name            | Use
|-----------------------------|----------------------------------------------
| bibliographyStyle           | Contains templates for formatting the bibliography
| figures                     | A folder to place your figures, with some examples
| tables                      | A folder to place your tables, with some examples
| latexTemplate               | Contains the LaTeX template for compiling the thesis
| _bookdown.yml               | Information for naming the end product; use caution when modifying
| _output.yml                 | Information for formatting the output; use caution when modifying
| abstract.txt                | Place Abstract text here; use the same notation for text in RMarkdown
| abbreviations.txt           | Place Abbreviation text here; use the same notation for text in RMarkdown
| preface.txt                 | Place Preface text here; use the same notation for text in RMarkdown
| example.bib                 | An example bibliography file containing the references cited in the thesis
| 01-chapter1.Rmd             | An example chapter file; edit this file and use it as a template to create additional chapters
| 02-chapter2.Rmd             | An example of a second chapter
| 99-epilogue.Rmd             | An example epilogue chapter; note that chapters are compiled in the order of the numbers that prefix the file names
| index.Rmd                   | RMarkdown file that specifies the front matter of the thesis, including title, author, adviser, etc. Also specified are format settings, bibliography location, etc.

                            

You can ignore the `README.md` and `.gitignore` files.


### Step 2. Write!

Include the text, equations, figures, tables, or whatever you would like in the `chapter` RMarkdown files. The formatting of text, equations, citations, etc. is the same as any RMarkdown document. Below are some helpful resources for formatting text for RMarkdown:

+ [RMarkdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/)  
+ [bookdown: Authoring Books and Technical Documents with R Markdown](https://bookdown.org/yihui/bookdown/)  
+ [RStudio Cheat Sheets](https://rstudio.com/resources/cheatsheets/)  



### Step 3. Compile

When you are ready to compile the thesis, run the following command:

```
rmarkdown::render_site()
```

or click the `Build Book` button under the `Build` tab in RStudio.

The final thesis will be compiled into a PDF in the `_book` folder.




## Issues

If you have comments or issues, please [file theme here](https://github.com/neyhartj/umn_thesis/issues/new).













