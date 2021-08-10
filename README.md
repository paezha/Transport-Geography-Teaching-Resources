
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Transport Geography Teaching Resources

<!-- badges: start -->
<!-- badges: end -->

## Getting started: Installing `R` and RStudio

1.  Background

The use of tables is a very powerful way to summarize and report
information. In any discipline, including transportation geography,
tables can be very effective in describing trends and enabling people to
use empirical data to perform analysis. A table consists of a number of
rows and columns to summarize information. Table 1 represents an example
of simple table with five rows and two columns.

Table 1: Population of selected countries, 2007

| Country       | Population  |
|---------------|-------------|
| Canada        | 33,390,099  |
| United States | 301,141,811 |
| Japan         | 127,433,062 |
| Germany       | 82,400,498  |

With respect to rows, notice that the first row is reserved to provide
heading information. As for columns, the first column provides
information about the country name and the second column provides
information about the country’s population size in 2007. Note that each
block or grid cell in the table has an address that depends on the
location of the row and the column. For instance, the address of the
cell with the size of Canada’s population is column 2, row 2; the one
for Germany is column 2, row 5.

Although tables are primarily used to summarize empirical data, usually
the information provided in a table can be used for further analysis.
For instance, one might want to add up the total population of Table 1,
or rank the countries in descending fashion according to their
population size, or perhaps add an extra column to project population
size in the year 2030.

All of these tasks and more can be handled very easily in a variety of
software packages. For this exercise, you will use the statistical
computing language `R`.

2.  `R`: The open statistical computing project

What is `R`?

`R` is an open-source language for statistical computing. It was created
by Ross Ihaka and Robert Gentleman at the University of Auckland, New
Zealand, as a way to provide their students an accessible, no-cost, tool
for their courses. R is now maintained by R Development Core Team, and
developed by hundreds of contributors around the globe. R is an
attractive alternative to other software packages for data analysis
(e.g., Microsoft Excel) due to its open-source character (i.e., it is
free), its flexibility, and huge user community, which means if there’s
something you want to do (for instance, linear regression), it is very
likely that someone has already developed a package for it.

A good way to think about R is as a core package, to which libraries can
be attached to increase its functionality. `R` can be downloaded for
free at:

<https://cran.rstudio.com/>

`R` comes with a built-in console (a user graphical interface), but
better alternatives to the basic interface, including R Studio, which
can also be downloaded for free here:

<https://www.rstudio.com/products/rstudio/download/>

`R` requires you to work using the command line, which is going to be
unfamiliar to many of you accustomed to user-friendly graphical
interfaces. Do not fear. People worked for a long time using the command
line, or even more cumbersomely, with punched cards in early computers.
Graphical user interfaces are convenient, but they have a major
drawback, namely their inflexibility. A program that functions based on
graphical user interfaces allows you to do only what is hard-coded in
the user interface. Command line, as we will see, is somewhat more
involved, but provides much more flexibility in operation.

Go ahead. Install `R` and RStudio in your computer. If you are working
in the GIS lab, you will find that these have already been installed
there. If you have a previous installation of R, update it to the latest
version of `R`. Note: the teaching resources have been checked for
VERSION!

Before discussing tables further, we will quickly tour RStudio.

3.  RStudio window

The RStudio window provides a complete interface to interact with the
language `R`. It consists of a window with several panes. Some panes
include in addition several tabs. There are the usual drop-down menus
for common operations. See Figure 1 below.

![Figure 1:RStudio Interactive Development
Environment](images\RStudio-Window.png)

The editor pane allows you to open and work with text and other files,
where you can write instructions that can be passed on to the program.
Writing something in the editor does not execute the instructions, it
merely records them for possible future use.

The console pane is where instructions are passed on to the program.
When an instruction is typed (or copied and pasted) there, `R` will
understand that it needs to do something. The instructions must be
written in a way that `R` understands, otherwise errors will occur.

The environment is where all data that is currently in memory is
reported. The History tab acts like a log: it keeps track of all
instructions that have been executed in the console.

The last pane includes a number of useful tabs. The File tab allows you
to navigate your computer, change the working directory, see what files
are where, and so on. The Plot tab is where plots are rendered, when
instructions require `R` to do so. The Packages tab allows you to manage
packages, which as mentioned above, are pieces of code that can augment
the functionality of `R`. The Help tab is where you can consult the
documentation for functions/packages/see examples, and so on. The Viewer
tab is for displaying web content locally. Many `R` functions create
html output and it is in this pane where this kind of content can be
previewed.

Once you have RStudio, download the file “01 Overview of Data Analysis
and Visualization.Rmd”, and use RStudio to open it.
