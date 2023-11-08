# QuickIntro2R-src

This is the markdown + R source for a short introduction to R/RStudio, which can be compiled into a PDF file of ca. 20 pages. For a recent build, see [QuickIntro2R](https://github.com/alexploner/QuickIntro2R "QuickIntro2R - the document"). 

## Installation 

Clone the repository to a convenient working directory by running

```
git clone https://github.com/alexploner/QuickIntro2R-src.git
```

in a shell in the intended directory. All text and code are contained in file `Intro2R_short.Rmd`. 

You will also need to have R packages `tufte` and `tint` installed to be able to build the document, so you may need to run 

```
install.packages(c("tufte", "tint"))
```

at the R prompt. 

## Setup 

For the in-document examples, the document pretends to read files from a fictituous directory, by default `Z:/OmicsDataAnalysis` (i.e. we are pretending to be on a Wondows machine). This fictitious directory is defined in a freely modifiable string at the top of the document, in line

```
.showDir <- "Z:/OmicsDataAnalysis"
```

If you want to display a different location in the compiled document, just edit the string as required.

## Compilation

The PDF file can be built via the R command line as

```
rmarkdown::render("Intro2R_short.Rmd")
```

or knitted as usually from within the RStudio Source pane (choose `Knit to tintPDF`). 

## Licence

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

