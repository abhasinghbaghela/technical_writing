LaTeX
##1. Introduction to LaTeX
LaTeX is a document preparation system used to create professional documents, mathematical equations, and technical reports.
Key Topics
1. Advantages of LaTeX
2. LaTeX vs MS Word
3. LaTeX Editors: Overleaf, TeXstudio
4. Basic Document Structure
5. Document Classes and Sections
6. Text Formatting and Alignment
7. Lists and Special Characters
8. Page Styles and Font Sizes


##2. Mathematical Typesetting
LaTeX provides powerful tools for writing mathematical expressions.
Important Commands
1. Inline Math: $...$
2. Display Math: \\[...\\]
3. Superscripts: x^2
4. Subscripts: x_1
5. Fractions: \\frac{a}{b}
6. Square Roots: \\sqrt{x}
7. Summation: \\sum
8. Integrals: \\int
9. Matrices: matrix, pmatrix, bmatrix
10. Equations: equation, align
11. Piecewise Functions: cases
12. Lists: itemize, enumerate


##3. Colours, Figures and Images
1. xcolor – Add colours to documents.
2. \\textcolor{red}{text} – Change text colour.
3. graphicx – Insert external images.
4. \\includegraphics{} – Add images.
5. figure – Create figure environments.
6. \\caption{} – Add captions.
7. \\label{} and \\ref{} – Reference figures.
8. subcaption – Add multiple subfigures.


##4. LaTeX Picture Environment
Used to draw diagrams, shapes, graphs, and coordinate-based illustrations.
Important Commands
1. \\put(x,y){object} – Place objects.
2. \\line(x,y){length} – Draw lines.
3. \\vector(x,y){length} – Draw arrows.
4. \\circle{diameter} – Draw circles.
5. \\framebox{} – Create boxes.
6. \\oval{} – Create oval shapes.
7. \\multiput{} – Repeat objects.
8. \\setlength{\\unitlength}{} – Set drawing units.


##5. Git and GitHub
Introduction
- Git: Distributed version control system used to track code changes.
- GitHub: Online platform for hosting repositories and collaborating.
Types of Version Control
1. Local Version Control
2. Centralized Version Control
3. Distributed Version Control
Essential Git Commands
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
Important Concepts
1. Working Directory – Files being edited.
2. Staging Area – Changes prepared for commit.
3. Repository – Stores committed history.
4. Branching – Independent development.
5. Merging – Combining branches.
6. Merge Conflicts – Conflicting changes requiring manual resolution.
7. Pull Requests – Proposals to merge code.
8. Forking – Creating a separate copy of a repository.
9. .gitignore – Specifies files Git should ignore.
10. README.md – Documents a project.


##6. Git Best Practices
1. Commit changes regularly.
2. Use meaningful commit messages.
3. Create branches for new features.
4. Review and test code before merging.
5. Never upload passwords or API keys.
6. Maintain proper README documentation.


##7. Introduction to Doxygen
Doxygen is an open-source documentation generator for programming languages such as C, C++, Python, and Java. It extracts information from specially formatted comments in source code and generates reference manuals in formats such as HTML, LaTeX, and PDF.
Key Features of Doxygen
1. Parses source code and extracts function, class, and module documentation from comments.
2. Generates cross-referenced code, call graphs, and inheritance diagrams.
3. Supports Markdown, LaTeX formulas, Graphviz diagrams, and code examples.
4. Can be integrated into CI/CD workflows.
5. Is widely used for library and API documentation.
Installing Doxygen
1. Windows: Download the installer from Doxygen Downloads.
2. macOS: Install using brew install doxygen.
3. Linux (Debian/Ubuntu): Install using sudo apt-get install doxygen.
4. Check the installation using:
doxygen --version
Basic Doxygen Workflow
1. Write specially formatted documentation comments in your source code.
2. Create a configuration file using doxygen -g Doxyfile.
3. Edit the Doxyfile configuration as needed.
4. Generate the documentation using doxygen Doxyfile.
5. Browse the generated HTML documentation at html/index.html, or use the generated LaTeX/PDF output.
Doxygen Comment Syntax (C/C++/Java)
/**
 * \\brief Brief description of the function.
 *
 * Longer detailed explanation.
 * \\param x A parameter description.
 * \\return Description of the return value.
 */
int myFunction(int x);
Doxygen for Python
def foo(bar):
    """
    Brief description.
    More details here.

    :param bar: Bar parameter
    :type bar: int
    :return: Computed value
    :rtype: int
    """
    return bar + 1
Common Doxygen Tags
1. \\brief – Short summary of a function, class, or module.
2. \\param – Describes a function parameter.
3. \\return – Describes the return value.
4. \\author – Specifies author information.
5. \\version – Specifies the version.
6. \\see – References related items.
7. \\note – Adds an additional note.
Documenting Classes
/**
 * \\class Car
 * \\brief Represents a car object.
 *
 * Details about the class.
 */
class Car {
public:
    /**
     * \\brief Start the engine.
     * \\return True if successful.
     */
    bool startEngine();
};
Advanced Features: Grouping and Diagrams
1. Use Doxygen grouping commands to organize related code elements.
2. Create call graphs and include dependency diagrams by enabling Graphviz support with HAVE_DOT = YES in the Doxyfile.
3. Embed diagrams using @dot or PlantUML directives.
4. Use Markdown or HTML tables and images to make documentation more informative.
Doxygen Output Formats
1. HTML: Default format and useful for browsing documentation.
2. LaTeX/PDF: Suitable for printable reference manuals.
3. Other formats: RTF, XML, DocBook, and man pages.
Common Doxyfile settings include:
GENERATE_HTML = YES
GENERATE_LATEX = YES
GENERATE_RTF = NO
GENERATE_XML = NO
Doxygen Best Practices
1. Explain the purpose and expected behavior of functions, not just their parameters.
2. Keep brief and detailed descriptions distinct.
3. Document all public APIs and modules.
4. Use a consistent set of tags and documentation layout.
5. Generate documentation as part of continuous integration.
6. Store the Doxyfile configuration in the source repository.
7. Update documentation alongside code changes and review it during code reviews.
8. Publish generated documentation to GitHub Pages or an internal wiki when appropriate.
Learning Outcomes
1. Understand the purpose of automated code documentation.
2. Install Doxygen and check its version.
3. Write Doxygen comments for C/C++/Java and Python code.
4. Use common Doxygen tags to document functions, parameters, return values, and classes.
5. Generate HTML and LaTeX/PDF documentation.
6. Explore diagrams, call graphs, and cross-references.
7. Integrate documentation generation with version control and development workflows.
Doxygen Mini-Project
1. Download and install Doxygen.
2. Add Doxygen comments to a small C++ or Python codebase.
3. Generate the documentation and open html/index.html.
4. Explore the generated diagrams and cross-references.
Further Resources
- Doxygen Manual
- Doxygen Downloads