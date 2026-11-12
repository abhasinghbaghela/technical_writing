
# LaTeX: Document Styling and Advanced Features

## 1. Introduction
LaTeX is a document preparation system used to create professional and well-structured documents. It provides advanced features for page layout, formatting, numbering, indexing, and bibliographies.

## 2. Document Classes and Page Styles
The `\documentclass` command determines the overall structure, font size, and paper size of a document.

Common document classes:
- `article`: Papers and short documents.
- `report`: Longer reports with chapters.
- `book`: Books and theses.
- `beamer`: Slide presentations.
- `letter`: Formal correspondence.
- `exam`: Tests and quizzes.

Page styles control headers and footers:
- `plain`: Page number at the bottom.
- `empty`: No headers, footers, or page numbers.
- `headings`: Section or chapter titles in the header.

The `geometry` package customizes page margins, while `fancyhdr` provides control over headers and footers.

## 3. Title Pages and Abstracts
LaTeX uses the following commands to create a title:

```latex
\title{My Document}
\author{Author Name}
\date{\today}
\begin{document}
\maketitle
```

Formatting commands such as `\Huge`, `\Large`, and `\bfseries` can customize the title.

The `abstract` environment creates a summary of the document.

```latex
\begin{abstract}
This document explains advanced LaTeX features.
\end{abstract}
```

## 4. Customizing Document Appearance
Important packages for document styling:

- `sectsty`: Changes section heading styles.
- `fontspec`: Selects system fonts (requires XeLaTeX or LuaLaTeX).
- `xcolor`: Adds text and page colors.
- `fancyhdr`: Customizes headers and footers.
- `enumitem`: Controls list labels, indentation, and spacing.

Example:

```latex
\usepackage{xcolor}
\pagecolor{yellow!10}
```

## 5. Lines, Paragraphs, and Page Breaks
LaTeX provides commands to control text layout.

- `\\`: Creates a manual line break.
- Blank line: Starts a new paragraph.
- `\par`: Ends a paragraph.
- `\newpage`: Starts a new page.
- `\pagebreak`: Suggests a page break.
- `\clearpage`: Places pending figures and tables before a page break.

Other useful commands:

- `\mbox{}`: Keeps text together on one line.
- `\hspace{}`: Adds horizontal space.
- `\vspace{}`: Adds vertical space.
- `\parindent`: Controls paragraph indentation.
- `\parskip`: Controls space between paragraphs.

## 6. Section and Equation Numbering
LaTeX automatically numbers sections and subsections.

```latex
\section{Introduction}
\subsection{Background}
```

Useful commands:

- `\setcounter{section}{3}`: Changes the section counter.
- `\section*{Acknowledgments}`: Creates an unnumbered section.
- `\renewcommand{\thesection}{\Roman{section}}`: Uses Roman numerals for section numbering.

Equation numbering:

```latex
\begin{equation}
E = mc^2
\end{equation}
```

To suppress equation numbering, use `equation*` from the `amsmath` package.

## 7. Boxes and Custom Layouts
LaTeX provides different box commands for positioning and formatting content.

- `\makebox`: Creates an unframed box.
- `\framebox`: Creates a framed box.
- `\parbox`: Creates a fixed-width paragraph box.
- `\raisebox`: Moves content vertically.
- `\rule`: Draws horizontal or vertical lines.
- `\newsavebox`: Declares a box for storing content.
- `\savebox`: Saves content.
- `\usebox`: Reuses saved content.

Boxes can be combined to create complex layouts.

The `trivlist` environment creates a vertical list without visible labels and can be used to build custom environments.

## 8. Indexing with MakeIndex
MakeIndex is used to create an index for a LaTeX document.

Basic commands:

```latex
\usepackage{makeidx}
\makeindex

\index{LaTeX}
\printindex
```

Compilation sequence:

1. Run LaTeX.
2. Run MakeIndex.
3. Run LaTeX again.

Index entries can include subentries, page ranges, and cross-references.

## 9. Bibliographies with BibTeX
BibTeX manages references stored in a `.bib` file and formats them according to a bibliography style.

Example:

```latex
\bibliographystyle{plain}
\bibliography{refs}
```

To cite a reference:

```latex
\cite{reference_key}
```

Common BibTeX entry types:

- `article`: Journal articles.
- `book`: Books.
- `inproceedings`: Conference papers.
- `techreport`: Technical reports.
- `misc`: Other reference types.

Compilation sequence:

1. Run LaTeX.
2. Run BibTeX.
3. Run LaTeX twice.

## 10. Finding and Fixing Errors
LaTeX provides error messages in the compilation log, often with line numbers and file information.

Common errors include:

- Undefined control sequence.
- Missing file.
- Undefined environment.
- Missing `\begin{document}`.
- Mismatched `\begin` and `\end`.
- Incorrect mathematical delimiters.
- Too many columns in a table.

### Error-Fixing Strategies
1. Check the compilation log and error location.
2. Review recent code changes.
3. Comment out suspicious code.
4. Recompile regularly.
5. Create a minimal document to isolate difficult errors.

Overfull and underfull box warnings indicate layout problems. A "TeX capacity exceeded" message indicates that a resource limit has been reached.

## 11. Learning Outcomes
After studying these topics, learners should be able to:

- Select suitable LaTeX document classes.
- Customize page styles, margins, headers, and footers.
- Create title pages and abstracts.
- Format sections, equations, and paragraphs.
- Use boxes for custom layouts.
- Generate indexes using MakeIndex.
- Manage references using BibTeX.
- Identify and fix common LaTeX errors.
