Course: Introduction to LaTeX
Instructor: Dr. Neeta Nain
Institute: MNIT Jaipur


Introduction to LaTeX
1)Introduction to LaTeX
2)Advantages of LaTeX
3)LaTeX vs MS Word
4)LaTeX Tools and Editors
5)Input Files and Output Formats
6)Compiling LaTeX Documents
7)Basic Document Structure
8)Document Classes and Options
9)Title, Author and Date
10)Abstract
11)Sections and Subsections
12)Spaces and Paragraphs
13)Special Characters
14)LaTeX Commands and Comments
15)Page Styles
16)Hyphenation
17)Font Sizes
18)Text Alignment
19)Lists (Itemize, Enumerate, Description)
20)Mathematical Equations
21)Mathematical Symbols
22)Tables
23)Figures and Images
24)Cross References
25)Bibliography and Citations

Mathematical Notations, Equations, Arrays, Matrices and Lists:
)Inline and Display Mathematics
)Superscripts and Subscripts
)Greek Letters and Special Symbols
)Fractions and Roots
)Sums, Products and Integrals
)Relations and Logic Symbols
)Numbered Equations
)Array Environment
)Piecewise Functions
)Matrices and Matrix Delimiters
)Large and Small Matrices
)Extra Matrix Spacing
)Lists in LaTeX

Exploring Mathematical Display Styles in LaTeX:
)Inline and Display Math Styles
)Mathematical Fonts
)Relations and Logic Symbols
)Superscripts and Subscripts
)Fractions, Roots, Sums, Products and Integrals
)Overbrace and Underbrace
)Array Environment
)Piecewise Functions
)Binomial Coefficients
)Numbered Equations
)Long Equations
)Splitting Equations
)Grouping and Centering Equations
)Matrix Environments
)Matrix Delimiters
)Large and Small Matrices
)Lists in LaTeX

Tools: Overleaf, TeXstudio, MiKTeX, TeX Live

Primary Focus: Document Formatting, Mathematical Typesetting, Equations, Matrices, Arrays and Lists.

Exploring Math Display Styles in LaTeX:
)focuses on writing mathematical expressions and equations in LaTeX. It explains different mathematical environments, symbols, fonts, and formatting techniques.
Topics Covered:
)Inline and Display Math: Inline mathematics uses $...$ or \(...\), while display mathematics uses \[...\] or the displaymath environment.
)Mathematical Fonts: Different font styles can be created using commands such as \mathcal, \mathfrak, \mathbb, \mathrm, and \mathbf.
)Mathematical Symbols: LaTeX supports Greek letters, binary operators, relations, and logical symbols.
)Superscripts and Subscripts: The ^ symbol creates superscripts, while _ creates subscripts.
)Fractions and Roots: Commands such as \frac{a}{b} and \sqrt{x} are used to write fractions and square roots.
)Sums, Products and Integrals: Commands like \sum, \prod, and \int help write advanced mathematical expressions.
)Overbrace and Underbrace: These commands are used to highlight and label parts of mathematical expressions.
)Arrays and Piecewise Functions: The array environment helps organize mathematical expressions into rows and columns.
)Binomial Coefficients: The \binom{n}{k} command represents combinations.
)Numbered Equations: The equation environment automatically numbers equations.
)Long and Split Equations: The multline and align environments help format long equations across multiple lines.
)Matrices: LaTeX provides matrix, pmatrix, bmatrix, Bmatrix, vmatrix, and Vmatrix environments for different matrix styles.
)Lists: The itemize, enumerate, and description environments create unordered, ordered, and descriptive lists.

Colours, Figures and Picture Environment
explains how to make LaTeX documents more attractive by adding colours, images, shapes, and drawings.
Topics Covered:
)Introducing Colours: The xcolor package allows users to add colours to text and mathematical expressions.
)Text Colours: The \textcolor{color}{text} command changes the colour of selected text.
)Predefined Colours: LaTeX supports colours such as red, blue, green, violet, cyan, brown, and teal.
)Custom Colours: The \definecolor command allows users to define colours using RGB, HTML, and named colour models.
)Background Highlights: The \colorbox and \fcolorbox commands create coloured backgrounds and framed text.
)Figures and Images: The graphicx package is used to insert images using \includegraphics.
)Image Resizing: Images can be resized using width, height, and scale options.
)Figure Environment: The figure environment supports image


LaTeX Figures, Picture Environment, and Git & GitHub
1. Introduction
This repository contains study material for Lecture 7, Lecture 8, and Lecture 9. It covers creating figures and graphs using LaTeX, drawing diagrams using the LaTeX Picture Environment, and understanding version control using Git and GitHub.
The main objective is to understand how to create professional technical documents, draw mathematical diagrams, manage project files, and collaborate with other developers.
2. Lecture 7: Creating Figures and Graphs with LaTeX
2.1 Introduction to Figures
LaTeX provides a figure environment to insert figures, diagrams, and graphs into documents. Figures help present information visually and improve document readability.
Basic syntax:
latex
\begin{figure}[h]
    Figure content
    \caption{Figure Title}
    \label{fig:example}
\end{figure}

\begin{figure} starts the figure environment.
[h] suggests placing the figure approximately at the current position.
\caption{} adds a caption below or above the figure.
\label{} assigns a reference name to the figure.
\end{figure} ends the environment.

2.2 Figure Placement Options
LaTeX provides different placement options:

h – Place the figure approximately here.
t – Place the figure at the top of a page.
b – Place the figure at the bottom of a page.
p – Place the figure on a separate page containing floats.
These options help organize figures within a document.

2.3 Creating Figures Using Picture Environment
LaTeX allows users to create simple diagrams using the picture environment.
Important commands include:
\put{x,y}{object} – Places an object at specified coordinates.
\framebox(width,height){text} – Creates a rectangular box containing text.
\line(x,y){length} – Draws a line.
\vector(x,y){length} – Draws an arrow.
\circle{diameter} – Creates a circle.
\caption{} – Adds a figure title.
\label{} – Creates a reference label.
Example:
latex
\begin{figure}[h]
\centering
\setlength{\unitlength}{0.14in}
\begin{picture}(32,15)
\put(3,4){\framebox(6,3){$H_B(q)$}}
\put(13,4){\framebox(6,3){$N[\cdot]$}}
\put(23,4){\framebox(6,3){$H_C(q)$}}
\put(0,5.5){\vector(1,0){3}}
\put(9,5.5){\vector(1,0){4}}
\put(19,5.5){\vector(1,0){4}}
\put(29,5.5){\vector(1,0){3}}
\end{picture}
\caption{Block Oriented Model Structure}
\label{fig:model}
\end{figure}

2.4 Referencing Figures
Figures can be referenced inside the document using \ref{}.
Example:
latex
Figure \ref{fig:model} shows the block model structure.
LaTeX automatically generates the corresponding figure number.

2.5 Importing External Graphics
Instead of drawing figures manually, users can create images using external software and import them into LaTeX.
Common graphics software includes:
MATLAB
Mathematica
Maple
Photoshop
Xfig
LaTeX supports different image formats depending on the compiler.
Common formats include:
EPS
PDF
PNG
JPEG
For modern PDF-based compilation, PDF, PNG, and JPEG are commonly used. EPS is generally associated with traditional PostScript workflows.

2.6 Using the Graphicx Package
The graphicx package is used to insert external images.
Add the following command in the document preamble:
latex
\usepackage{graphicx}
To insert an image:
latex
\begin{figure}[ht]
\centering
\includegraphics[width=0.5\textwidth]{matlab.png}
\caption{MATLAB Graph}
\label{fig:matlab}
\end{figure}
Important commands:
\includegraphics{} – Inserts an external image.
width – Specifies the image width.
height – Specifies the image height.
\scalebox{} – Changes the image scale.
angle – Rotates an image by a specified angle.
Example:
latex
\includegraphics[angle=30,width=0.5\textwidth]{matlab.png}

2.7 Landscape Figures
Large figures can be displayed in landscape orientation using the rotating package.
latex
\usepackage{rotating}
Example:
latex
\begin{sidewaysfigure}
\centering
\includegraphics[width=0.7\textwidth]{matlab.png}
\caption{Landscape Figure}
\label{fig:landscape}
\end{sidewaysfigure}

2.8 Creating Subfigures
Subfigures allow multiple images to be displayed inside one figure environment.
They are useful for comparing different graphs or experimental results.
Example using the modern subcaption package:
latex
\usepackage{graphicx}
\usepackage{subcaption}
\begin{figure}[h]
\centering
\begin{subfigure}{0.45\textwidth}
\includegraphics[width=\textwidth]{big.png}
\caption{Big}
\end{subfigure}
\hfill
\begin{subfigure}{0.45\textwidth}
\includegraphics[width=\textwidth]{small.png}
\caption{Small}
\end{subfigure}
\caption{Comparison of Figures}
\label{fig:subfigures}
\end{figure}

3. Lecture 8: LaTeX Picture Environment
3.1 Introduction
The LaTeX Picture Environment is used to create diagrams containing text, lines, arrows, circles, and geometric shapes.
Basic syntax:

latex
\begin{picture}(width,height)(x-offset,y-offset)
    Picture commands
\end{picture}

Width specifies the picture width.
Height specifies the picture height.
X-offset and Y-offset specify the position of the origin.
Coordinates determine where individual objects are placed.
3.2 Unit Length

The \unitlength command defines the measurement unit used by the picture environment.

Example:

latex
\setlength{\unitlength}{1cm}


Common LaTeX units:

in – Inches.
mm – Millimeters.
cm – Centimeters.
pt – Points.
em – Approximately the width of the letter M in the current font.
ex – Approximately the height of the letter x in the current font.
3.3 Important Picture Commands

The following commands are used to create different objects.

\put(x,y){object} – Places an object at a specified coordinate.
\circle{diameter} – Draws a circle.
\line(x,y){length} – Draws a straight line with a specified slope.
\vector(x,y){length} – Draws an arrow.
\frame{object} – Creates a rectangular frame around an object.
\framebox(width,height){text} – Creates a rectangular box with text.
\dashbox{dash}(width,height){text} – Creates a dashed rectangular box.
\oval(width,height) – Draws a rectangle with rounded corners.
\linethickness{dimension} – Changes the thickness of horizontal and vertical lines.
\makebox(width,height)[position]{text} – Creates a box with positioned text.
\multiput(x,y)(dx,dy){number}{object} – Repeats an object at regular intervals.
\shortstack{} – Arranges multiple text elements vertically.
3.4 Creating a Circle and Coordinate Axes

Example:

latex
\setlength{\unitlength}{0.5in}

\begin{picture}(10,10)(-5,5)
\linethickness{1pt}

\put(-2.5,0){\vector(1,0){5}}
\put(0,-2.5){\vector(0,1){5}}
\put(0,0){\circle{2}}

\end{picture}


This example creates horizontal and vertical coordinate axes with a circle at the origin.

3.5 Creating a Right Triangle

Example:

latex
\setlength{\unitlength}{0.4in}

\begin{picture}(7,5)
\linethickness{1pt}

\put(0,0){\line(1,0){4}}
\put(4,0){\line(0,1){3}}
\put(0,0){\line(4,3){4}}

\put(2,-0.25){\makebox(0,0){$\alpha$}}
\put(4.25,1.5){\makebox(0,0){$\beta$}}
\put(2,2){\makebox(0,0){$\gamma$}}

\end{picture}


This example demonstrates how to create geometric shapes and place mathematical symbols using coordinates.

3.6 Creating a Discontinuous Function

The picture environment can also be used to draw mathematical graphs.

Example:

latex
\setlength{\unitlength}{0.01in}

\begin{picture}(200,75)

\put(0,25){\vector(1,0){200}}
\put(25,0){\vector(0,1){75}}

\put(25,25){\line(1,0){50}}
\put(75,50){\line(1,0){50}}
\put(125,25){\line(1,0){72}}

\put(195,13){\makebox(0,0){$t$}}
\put(175,60){\makebox(0,0){$g(t)$}}

\end{picture}


This demonstrates the use of coordinate positions, horizontal lines, and arrows to represent mathematical functions.

4. Lecture 9: Version Control Tools – Git and GitHub
4.1 Introduction to Version Control

Version control is a system that records changes made to files over time.

It allows developers to track modifications, recover previous versions, and collaborate on projects.

Main benefits:

Tracks changes in files.
Maintains project history.
Identifies who made changes.
Helps recover previous versions.
Supports teamwork and collaboration.
Makes debugging and maintenance easier.
4.2 Types of Version Control Systems

There are three main types:

Local Version Control System – Maintains versions on a single computer.
Centralized Version Control System – Stores project history on a central server. Example: SVN.
Distributed Version Control System – Every clone contains repository history. Example: Git.
4.3 What Is Git?

Git is a distributed version control system used to manage source code and track project changes.

Important features:

Maintains project history through commits.
Supports multiple branches.
Allows offline development.
Supports merging changes.
Helps developers collaborate.
4.4 Git vs GitHub
Git	GitHub
Version control system	Hosting platform
Works locally	Works online
Tracks file changes	Hosts repositories
Maintains commits	Supports collaboration
Supports branches	Supports pull requests

Git manages version history, while GitHub provides online hosting and collaboration features.

4.5 Installing Git

Git can be installed on Windows, Linux, and macOS.

Windows: Download Git from https://git-scm.com/downloads

Ubuntu/Linux:

bash
sudo apt update
sudo apt install git


macOS:

bash
brew install git


Verify installation:

bash
git --version

4.6 Configuring Git

Set the username and email:

bash
git config --global user.name "Student Name"

git config --global user.email "student@example.com"


Verify configuration:

bash
git config --global --list

4.7 Creating a Git Repository

A Git repository stores project files and their version history.

Commands:

bash
mkdir my-project
cd my-project
git init

mkdir creates a directory.
cd enters the directory.
git init initializes a Git repository.
Git creates a hidden .git directory.
4.8 Three Main Areas of Git

Git works using three main areas:

Working Directory – Contains files being edited.
Staging Area – Contains selected changes prepared for committing.
Repository – Stores committed project history.

Basic workflow:

bash
git add .
git commit -m "Initial commit"

4.9 Essential Git Commands
git status – Checks repository status.
git add file.py – Stages a file.
git add . – Stages changes in the current directory.
git commit -m "message" – Records staged changes.
git log – Displays commit history.
git log --oneline – Displays compact commit history.
git diff – Shows unstaged changes.
git diff --staged – Shows staged changes.
git branch – Lists branches.
git switch branch-name – Switches branches.
git merge branch-name – Merges another branch.
git clone URL – Copies a remote repository locally.
git push – Uploads commits to a remote repository.
git pull – Fetches and integrates remote changes.
git fetch – Downloads remote updates without integrating them.
4.10 Git Ignore File

The .gitignore file specifies files and folders that Git should ignore.

Example:

text
__pycache__/
*.pyc
.env
*.log
data/


It is commonly used for temporary files, environment configurations, logs, and generated files.

4.11 Understanding GitHub

GitHub is an online platform used to host Git repositories.

Main features:

Repository hosting.
Code sharing.
Pull requests.
Issue tracking.
Code reviews.
Project management.
Team collaboration.

Website: https://github.com/

4.12 Creating a GitHub Repository

Steps:

Create or sign in to a GitHub account.
Select the New Repository option.
Enter a repository name.
Choose public or private visibility.
Add a README if required.
Click Create Repository.

A public repository can be viewed by anyone, whereas a private repository is accessible only to authorized users.

4.13 README File

A README file introduces a project and explains its purpose, installation, features, and usage.

Common sections include:

Project title.
Project description.
Features.
Installation instructions.
Usage instructions.
Technologies used.
Contributors.
License.

README files are generally written in Markdown and saved as README.md.

4.14 Connecting Git with GitHub

Add a remote repository:

bash
git remote add origin REPOSITORY_URL


Check remote connections:

bash
git remote -v


Push code to GitHub:

bash
git branch -M main
git push -u origin main


This uploads local commits to the configured GitHub repository.

4.15 Cloning a Repository

Cloning downloads a repository to the local computer.

bash
git clone REPOSITORY_URL


It downloads project files, commit history, and repository information.

4.16 Branching and Merging

A branch is an independent line of development.

Branches allow developers to work on different features without directly changing the main branch.

Important commands:

bash
git branch
git branch feature-login
git switch feature-login
git switch -c feature-new


To merge a branch:

bash
git switch main
git merge feature-login

4.17 Merge Conflicts

A merge conflict occurs when Git cannot automatically combine changes made in different branches.

Steps to resolve conflicts:

Open the conflicting file.
Identify the conflicting sections.
Choose or combine the required changes.
Remove conflict markers.
Stage the resolved file.
Complete the merge commit if required.
bash
git add main.py
git commit

4.18 Pull Requests and Forking

A pull request is a proposal to merge changes from one branch into another.

Typical process:

Create a feature branch.
Make changes.
Commit the changes.
Push the branch to GitHub.
Create a pull request.
Request code review.
Merge approved changes.
A fork creates a separate hosted copy of another repository, allowing contributors to work independently and propose changes.

4.19 Git Best Practices
Commit changes regularly.
Use meaningful commit messages.
Create separate branches for new features.
Review changes before committing.
Test code before merging.
Keep sensitive information out of repositories.
Use .gitignore appropriately.
Maintain clear README documentation.
Pull or fetch remote changes regularly.
Review pull requests before merging.
5. Practical Mini Project: Calculator Using Git and GitHub
The objective is to create a simple calculator and manage its development using Git and GitHub.

Step 1: Create a Project
bash
mkdir calculator
cd calculator
git init

Step 2: Create a Python File

Create main.py:
python
print("Calculator")
a = 10
b = 5
print("Sum:", a + b)
print("Difference:", a - b)

Step 3: Stage and Commit
bash
git status
git add main.py
git commit -m "Add initial calculator"
git log --oneline

Step 4: Connect to GitHub
Create an empty repository named calculator on GitHub.
bash
git branch -M main
git remote add origin REPOSITORY_URL
git push -u origin main

Step 5: Create a Feature Branch
bash
git switch -c feature-subtraction
Make the required changes and commit them:
bash
git add main.py
git commit -m "Add subtraction feature"
git push -u origin feature-subtraction

Step 6: Create a Pull Request
Open the repository on GitHub.
Select the option to create a pull request.
Select main as the base branch.
Select feature-subtraction as the compare branch.
Review the changes.
Merge the pull request after approval.
Step 7: Update the Local Repository
bash
git switch main
git pull origin main
The calculator project is now maintained using Git and GitHub.

6. Learning Outcomes
After completing these three lectures, students should be able to:
Create figures and graphs using LaTeX.
Import external images into LaTeX documents.
Use captions and labels to reference figures.
Draw diagrams using the Picture Environment.
Understand coordinates, dimensions, and units.
Use different picture commands to create shapes and graphs.
Explain version control and its importance.
Install and configure Git.
Create and manage Git repositories.
Perform staging, committing, pushing, and pulling.
Create branches and merge changes.
Use GitHub for project hosting and collaboration.
Create pull requests and resolve merge conflicts.
Maintain projects using proper documentation.
7. Conclusion
 introduce important tools used in technical documentation and software development. LaTeX provides powerful facilities for creating professional figures, graphs, and mathematical diagrams. The Picture Environment allows users to draw shapes and illustrations using coordinates and commands. Git and GitHub help developers track project changes, maintain version history, collaborate with teams, and publish their work.
Together, these topics provide a foundation for technical writing, documentation, programming, and collaborative software development.