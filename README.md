README
======

LaTeX class for preparing MS Software Engineering final year project report. It could also be extended to other courses and departments with a few tweaks.

###Requirements

A Win/Linux/Mac system with some variant of LaTeX2e installed. We recommend [TeXworks](https://www.tug.org/texworks/), since its available for all platforms and maintained by an active community. The class mostly uses in-built packages, but if something is not available in your system you can get it from [CTAN](http://www.ctan.org).

###Overview

The class has been extended from the standard **report** class, so whatever applies to report also applies here. The title page and various other standard pages are generated by simple macros, for which the calls can be made in the order your project report demands (called from the report.tex file). You have to pass on your project specific data to these macros like *regno*, *name*, *project title*, etc.

###Files

- **vitmsprojectreport.cls** - The class file that controls the layout of the project report and declares macros for standard pages. There's no need to touch this file unless you're trying to extend the class.
- **report.tex** - This is where you'll have to place your content.
- **Biblography.bib** - You have to place your bibliography items in this file, in the standard bibtex format.
- **vit.png** - The official VIT Logo. Don't touch this!

Your LaTeX compiler will generate many files that may look like junk, \*.toc, \*.lof, \*.blg, \*.aux, \*.log, \*.bbl, etc. However, these files act like a cache and store useful pieces of information for later reference. They can be regenerated anytime by compiling your .tex file.

###Compilation

The class has been tested using **pdflatex** and **bibtex**, 2011 distribution. The specific steps for compilation can be obtained from your TeX distribution. From the command line, the generic procedure is to compile with: **pdflatex** -> **bibtex** -> **pdflatex** -> **pdflatex** in order. We need to compile these many times because LaTeX has to make a few passes to resolve the references. Finally, you get a pdf output file, **report.pdf**.

###Citations

###Cross-References

###Images

###Tables

###Lists

###Algorithms

###Code Listings