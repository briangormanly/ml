Marist's Letter LaTeX Template
=====
[![Latest Github release](https://img.shields.io/badge/version-0.1-blue.svg)](https://img.shields.io/badge/version-0.1-blue.svg)
[![Build status of the master branch](https://img.shields.io/badge/build%20status-pass-green.svg)](https://img.shields.io/badge/build%20status-pass-green.svg)

This is an attempt at having a LaTeX template for letter using what Marist College considers our [master guidelines](http://www.marist.edu/publicaffairs/imc/pdfs/styleguide.pdf) for such type of official communication. It uses the [official institutional logo](http://www.marist.edu/publicaffairs/imc/graphics/For_Print/Nameplate2/LargeLogoRed.pdf).

This was developed on MacOS and tested on Linux. I have no intentions of testing this on Windows for personal reasons.


## Features in v0.1
* Separate files for **setup** of personal information and letter main body.
* Sample letters that include a **Short and Long Letters** and a **Recommendation Letter**. 
* If you have a digital signature you can use it! But make sure it is in `.eps` format. I provided a sample `PabloSignature.eps`, check it out.

## Dependencies and Assumptions
* This assumes that you know basic LaTeX to the point of being able to write in
  this typesetting language.
* We assume that you have the most recent versions of `latex`, `tex-live`,  `dvips`, and `ps2pdf` with all its dependencies.
* We require the following LaTeX packages: `xcolor`, `graphicx`, `geometry`, `textpos`, `ifthen`, `soul`, `gfsbodoni`, `tikz`, `scrextend`, and `fancyhdr`. But fear not, these are usually installed with `tex-live`.
* Make sure you never remove the `MaristLogo.eps` file from the directory where your letter is, or update the path to it if you move it.

## Usage
* Edit the file MaristLetterDefs.tex and fill in your personal faculty information, follow the comments in the file.
* Edit the file Letter.tex which will contain the recipient information and your main body of text.
* If you are a command line freak like me, just run the `make` command and my `MakeFile` file contains the sequence to produce a `.dvi`, `.ps`, and `.pdf` versions of your letter as well as a clean-up command for the LaTeX left-over log files.
* If you are not well versed in how to run LaTeX from the command line, you will need to try and run LaTeX the way you usually do it. If you give me feedback, I can include such instructions here for other people.

