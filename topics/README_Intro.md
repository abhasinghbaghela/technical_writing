# LaTeX:Intro

## A LATEX source file is saved with the .tex extension.
## The .tex and .bib files are compiled separately, and their outputs are combined to generate the PDF.
## Every LATEX document must contain the following three components:
    \documentclass{article}
    \begin{document}
    \end{document}
## Every input file starts with the command:
    \documentclass{...}
## After the setup is complete, the document body starts with:
    \begin{document}
## The document content is then written using text and appropriate LATEX commands.
## At the end of the document, use:
    \end{document}
## The first line of a LATEX document specifies the document class and optional settings.
        book
        report
        article
        letter
## In general:
    Required arguments are enclosed in braces {}.
    Optional arguments are enclosed in square brackets [].
    Use \title and \maketitle to add a title.
    \title defines the title, while
    \maketitle displays it in the
    document.
    \maketitle must appear after
    \begin{document}.
    \title must be defined before
    \maketitle.
    Use \author and \date to specify the author and date.
## Abstracts
    To create an abstract, place the text inside the abstract
    environment:
    Syntax
    \begin{abstract}
    Abstract text goes here.
    \end{abstract}
Sections
## LATEX provides commands to organize a document into sections and subsections.
    \section{Section Title}
    \subsection{Subsection Title}
    \subsubsection{Subsubsection Title}
## Page Styles
    plain
    headings
    empty
