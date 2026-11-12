# LaTeX, Git & GitHub

## 1. Introduction to LaTeX
LaTeX is a document preparation system used to create professional documents, mathematical equations, and technical reports.

### Key Topics
1. Advantages of LaTeX
2. LaTeX vs MS Word
3. LaTeX Editors: Overleaf, TeXstudio
4. Basic Document Structure
5. Document Classes and Sections
6. Text Formatting and Alignment
7. Lists and Special Characters
8. Page Styles and Font Sizes

## 2. Mathematical Typesetting
LaTeX provides powerful tools for writing mathematical expressions.

### Important Commands
1. Inline Math: `$...$`
2. Display Math: `\[...\]`
3. Superscripts: `x^2`
4. Subscripts: `x_1`
5. Fractions: `\frac{a}{b}`
6. Square Roots: `\sqrt{x}`
7. Summation: `\sum`
8. Integrals: `\int`
9. Matrices: `matrix`, `pmatrix`, `bmatrix`
10. Equations: `equation`, `align`
11. Piecewise Functions: `cases`
12. Lists: `itemize`, `enumerate`

## 3. Colours, Figures and Images
1. `xcolor` – Add colours to documents.
2. `\textcolor{red}{text}` – Change text colour.
3. `graphicx` – Insert external images.
4. `\includegraphics{}` – Add images.
5. `figure` – Create figure environments.
6. `\caption{}` – Add captions.
7. `\label{}` and `\ref{}` – Reference figures.
8. `subcaption` – Add multiple subfigures.

## 4. LaTeX Picture Environment
Used to draw diagrams, shapes, graphs, and coordinate-based illustrations.

### Important Commands
1. `\put(x,y){object}` – Place objects.
2. `\line(x,y){length}` – Draw lines.
3. `\vector(x,y){length}` – Draw arrows.
4. `\circle{diameter}` – Draw circles.
5. `\framebox{}` – Create boxes.
6. `\oval{}` – Create oval shapes.
7. `\multiput{}` – Repeat objects.
8. `\setlength{\unitlength}{}` – Set drawing units.

## 5. Git and GitHub

### Introduction
- **Git:** Distributed version control system used to track code changes.
- **GitHub:** Online platform for hosting repositories and collaborating.

### Types of Version Control
1. Local Version Control
2. Centralized Version Control
3. Distributed Version Control

### Essential Git Commands

```bash
git --version
git config --global user.name "Name"
git config --global user.email "email@example.com"

git init
git status
git add .
git commit -m "Initial commit"
git log --oneline
git diff

git branch
git switch -c feature
git merge feature

git clone REPOSITORY_URL
git remote add origin REPOSITORY_URL
git push -u origin main
git pull
git fetch
```

### Important Concepts
1. Working Directory – Files being edited.
2. Staging Area – Changes prepared for commit.
3. Repository – Stores committed history.
4. Branching – Independent development.
5. Merging – Combining branches.
6. Merge Conflicts – Conflicting changes requiring manual resolution.
7. Pull Requests – Proposals to merge code.
8. Forking – Creating a separate copy of a repository.
9. `.gitignore` – Specifies files Git should ignore.
10. README.md – Documents a project.

## 6. Git Best Practices
1. Commit changes regularly.
2. Use meaningful commit messages.
3. Create branches for new features.
4. Review and test code before merging.
5. Never upload passwords or API keys.
6. Maintain proper README documentation.

## 7. Learning Outcomes
1. Create professional documents using LaTeX.
2. Write mathematical equations and matrices.
3. Insert images and create diagrams.
4. Use the Picture Environment.
5. Understand version control.
6. Manage repositories using Git.
7. Collaborate using GitHub.
8. Create branches and resolve merge conflicts.