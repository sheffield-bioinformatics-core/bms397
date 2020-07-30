---
title: "BMSXXX Bioinformatics and Data Analysis Primer"
author: "Mark Dunning - Sheffield Bioinformatics Core"
output: 
  html_document: 
    toc: yes
    toc_float: yes
    css: stylesheets/styles.css
editor_options: 
  chunk_output_type: inline
---

<img src="images/logo-sm.png" style="position:absolute;top:40px;right:10px;" width="200" />

# About 

This primer was developed to enable BMS students to undertake data analysis project work in light of Covid-19 restricting access to labs. Others are free to use the materials on this page for their own learning.

## Contact

web : [sbc.shef.ac.uk](https://sbc.shef.ac.uk)  
twitter: [SheffBioinfCore](https://twitter.com/SheffBioinfCore)  
email: [bioinformatics-core@sheffield.ac.uk](bioinformatics-core@sheffield.ac.uk)

# Week 1 - Introduction to Data Manipulation and Visualisation using R

## Overview

As the data generated from high-throughput biological experiments increase in volume and become more complex, the ability to manipulate and visualise data is a highly-desirable skill in academia and industry. Whilst familiar tools such as Excel allow basic manipulations, they are often not scalable to larger datasets and are not ameanable to reproducible analysis. 

R is a highly-regarded, free, software environment for statistical analysis, with many useful features that promote and facilitate reproducible research.

In this course, we give an introduction to the R environment and explain how it can be used to import, manipulate and visualise tabular data. 

After the course you should feel confident to start exploring your own dataset using the materials and references provided. 


## Setup

1) To follow the course on your own computer, install both R **and** RStudio for your operating system. Instructions are availableon youtube to explain the process
  + [Installation for Mac](https://www.youtube.com/watch?v=1PsPfMaLWSk)
  + [Installation for Windows](https://www.youtube.com/watch?v=GAGUDL-4aVw)
  
2) Please download and extract (un-zip) [this zip file](http://sbc.shef.ac.uk/r-online/CourseData.zip) into the directory on your computer that you wish to work in

3) Create an RStudio project using the menu **File -> New Project -> Existing Directory** and browse to the directory that you extraced the zip file to.

4) Type the following into the R console to install some extra R packages required for the workshop

```
install.packages("dplyr")
install.packages("ggplot2")
install.packages("readr")
```

These instructions are also described in a video:- [https://youtu.be/vzLclNVuGoI](https://youtu.be/vzLclNVuGoI)

**Mac Users may get the following error message when trying to install these packages**

```
xcrun error: inactive developer path (/Library/Developer/CommandLineTools), missing xcrun at:.....

```

If this is the case, you will need to follow the instructions from this link to install "Xcode"

[https://apple.stackexchange.com/questions/254380/why-am-i-getting-an-invalid-active-developer-path-when-attempting-to-use-git-a](https://apple.stackexchange.com/questions/254380/why-am-i-getting-an-invalid-active-developer-path-when-attempting-to-use-git-a)

**Window users might get a message that Rtools is required. This shouldn't be neccesary, but you might need it for other packages. It can be installed here:-**

[https://cran.r-project.org/bin/windows/Rtools/](https://cran.r-project.org/bin/windows/Rtools/)


5) Check your installation. You can check everything is installed by copying and pasting this into the R console

```
source("https://raw.githubusercontent.com/sheffield-bioinformatics-core/r-online/master/check_packages.R")

```

## Course Notes

+ [Introduction Slides](http://sbc.shef.ac.uk/r-online/intro_slides.html)
+ [Part 1](http://sbc.shef.ac.uk/r-online/part1.nb.html)
+ [Part 2](http://sbc.shef.ac.uk/r-online/part2.nb.html)
+ [Part 3](http://sbc.shef.ac.uk/r-online/part3.nb.html)
  
## Video Recordings

Videos of the instructor going through the course materials will be available on youtube

- [Course Introduction](https://www.youtube.com/watch?v=bb-qyh3c9vE)
- [Part 1](https://youtu.be/nGiMyIRTDj0)
- [Part 2](https://youtu.be/o2lb87tPfjM)
- [Part 3](https://youtu.be/5H84lzgBang)


# Week 2 - Introduction to RNA-seq analysis


## Overview

High-throughput RNA-sequencing is now the standard technique for quantifying transcript abundance in a biological sample of interest. In this course we will describe the processes that take place once you submit a library for RNA sequencing, and what data you should expect to receive from the Bioinformatics Core.

We will describe the steps involved to go from sequencing library to a list of genes that show statistically significant differences between your biological conditions of interest. Practical sessions will use the user-friendly Galaxy interface (https://usegalaxy.org/) to demonstrate tasks such as *alignment*, *quality control* and *assessing differential expression*. We will also showcase some web sites you can use for enrichment and pathways analysis.

*Please note that the course will not cover the analysis of RNA-seq data using the  R programming langugage*

## Setup

- Please register for an account at [usegalaxy.eu](https://usegalaxy.eu).**Make sure to check your email to activate your account**
- Please download the GSEA app from 
[http://software.broadinstitute.org/gsea/downloads.jsp](http://software.broadinstitute.org/gsea/downloads.jsp) for your operating system (GSEA_Win_4.0.3-installer.exe or GSEA_4.0.3.app.zip)
- Please watch these pre-recorded lectures

  + [Introduction and Experimental Design](https://youtu.be/YtOG-77FfIg)
  + [RNA-seq workflow overview](https://youtu.be/m1x4CaLg90A)
  + [Functional Gene Analysis](https://youtu.be/clb0bh3zFSM)

## Course Notes

+ [RNA-seq Pre-processing](http://sbc.shef.ac.uk/rnaseq-introduction-online/01-pre-processing.nb.html)
+ [Differential Expression](http://sbc.shef.ac.uk/rnaseq-introduction-online/02-differential-expression.nb.html)
+ [Gene Set Enrichment](http://sbc.shef.ac.uk/rnaseq-introduction-online/03-enrichment.nb.html)
  
## Video Recordings

- [RNA-seq Pre-processing](https://youtu.be/WHeLvBWt6bg)
- [Differential Expression and Pathways](https://youtu.be/l_vw1loyDJ0)

