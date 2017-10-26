# Skill Share: Pandoc

Tahir H. Butt <tahir.butt@gmail.com>

October 26, 2017

This skill share covers:

0. [Motivation](#motivation) :open_mouth: :thumbsup:
1. [Installation](#installation) :nut_and_bolt: :hammer: 
2. [Pandoc Markdown](#pandoc_markdown)
3. [Citations](#citations)
4. [Bonus: Filters](#bonus_filters)

## Motivation

This is far from either an exhaustive or objective list, but here are some
of the reasons I think you might want to use Pandoc:

- You want to use [plain text](http://plain-text.co/) for your academic
  writing
- You are sympathetic to the ["Write Once, Run
  Everywhere"](https://en.wikipedia.org/wiki/Write_once,_run_anywhere)
  principle 
- You want to avoid having to use Microsoft Word but must share your
  documents with those who do
- You are jealous of all those mathematic and scientific articles produced
  using LaTeX but don't want to learn another arcane markup language
- All the cool kids seem to be using it

## Installation

The simplest installation method is to download and install the [current
release binary packages](https://github.com/jgm/pandoc/releases/latest) for
your operating system.

Because of the scope of this tutorial, I ask that you also instead work inside
a Docker container with optional dependencies installed, namely the LaTeX tools
for producing PDFs.

- Install [Docker Community Edition
  (CE)](https://www.docker.com/community-edition#/download) for your OS
- Upon restart, configure Docker to share folders
- Run [pandoc](https://github.com/jagregory/pandoc-docker) Docker container to
  download image: `docker run jagregory/pandoc`

## Pandoc Markdown

The [User Guide](https://pandoc.org/MANUAL.html#pandocs-markdown) covers the
specification of the Pandoc markdown syntax.

## Citations

Pandoc comes with a [Citation filter](https://pandoc.org/MANUAL.html#citations)
which adds support for bibliographies with
[pandoc-citeproc](https://github.com/jgm/pandoc-citeproc). If you already use
Zotero, I recommend installing the [Better
Bib(La)TeX](https://github.com/retorquere/zotero-better-bibtex) to export your
library for use with with the Pandoc citeproc filter.

## Bonus: Filters

- [Pandoc Filters](https://github.com/jgm/pandoc/wiki/Pandoc-Filters) with
example of CSV-to-table filter
- [R Markdown](http://rmarkdown.rstudio.com/) for producing documents from R and
Python data analysis
