
# LaTeX: Mathematical Expressions and Display Styles

## 1. Introduction
LaTeX provides powerful tools for writing mathematical expressions, equations, symbols, matrices, and formulas. It is widely used in mathematics, science, engineering, and academic documents.

## 2. Inline Math vs Display Math
LaTeX supports two main ways to write mathematical expressions.

**Inline Math:** Displays equations within a line of text.

```latex
\( x+y=10 \)
```

You can also use `$ ... $`.

**Display Math:** Displays equations separately in the center of the page.

```latex
\[
x+y=10
\]
```

Other display environments include `displaymath` and `equation`.

Load the mathematical packages using:

```latex
\usepackage{amsmath, amssymb}
```

## 3. Mathematical Fonts
LaTeX provides different mathematical font styles.

Important commands:

- `\mathcal{}`: Calligraphic font.
- `\mathfrak{}`: Fraktur font.
- `\mathbb{}`: Blackboard bold font.
- `\mathrm{}`: Roman font.
- `\mathbf{}`: Bold font.
- `\mathit{}`: Italic font.
- `\mathsf{}`: Sans-serif font.
- `\mathtt{}`: Typewriter font.

Example:

```latex
\[
\mathbb{R}, \mathcal{A}, \mathfrak{B}
\]
```

## 4. Relations and Logic Symbols
LaTeX supports Greek letters, mathematical operators, and relation symbols.

**Greek Letters:**

```latex
\alpha, \beta, \gamma, \delta, \lambda, \pi
```

**Binary Operators:**

```latex
\times, \otimes, \oplus, \cup, \cap
```

**Relation Operators:**

```latex
<, >, \subset, \supset, \subseteq, \supseteq
```

**Other Symbols:**

```latex
\int, \oint, \sum, \prod
```

## 5. Superscripts, Subscripts and Greek Letters
Superscripts are created using `^`, while subscripts use `_`.

Example:

```latex
$a_i^2 + b_j^3$
```

Greek letters are written using a backslash followed by their names.

```latex
$\alpha, \beta, \gamma, \delta, \lambda, \pi$
```

## 6. Fractions, Roots, Sums, Products and Integrals
LaTeX provides commands for common mathematical expressions.

**Fractions:**

```latex
\frac{a+b}{c}
```

**Square Roots:**

```latex
\sqrt{x}
```

**Cube Roots:**

```latex
\sqrt[3]{y}
```

**Summation:**

```latex
\sum_{i=1}^{n} i
```

**Product:**

```latex
\prod_{k=1}^{m} k
```

**Integration:**

```latex
\int_0^\infty e^{-x}\,dx
```

## 7. Overbrace and Underbrace
These commands are used to place explanatory labels above or below mathematical expressions.

```latex
\[
\overbrace{a+b+c}^{d}
\]

\[
\underbrace{a+b+c}_{d}
\]
```

- `\overbrace{}`: Places a brace above an expression.
- `\underbrace{}`: Places a brace below an expression.

## 8. Arrays and Piecewise Functions
The `array` environment creates aligned rows and columns inside mathematical expressions.

Example:

```latex
\[
\begin{array}{lcr}
\text{Left} & \text{Center} & \text{Right} \\
a & b & c \\
1 & 2 & 3
\end{array}
\]
```

Alignment options:
- `l`: Left alignment.
- `c`: Center alignment.
- `r`: Right alignment.

Arrays can also represent piecewise functions.

```latex
\[
f(x)=\left\{
\begin{array}{ll}
-x, & x<0 \\
0, & x=0 \\
x^2, & x>0
\end{array}
\right.
\]
```

## 9. Binomial Coefficients
The `\binom{n}{k}` command creates a binomial coefficient.

Example:

```latex
\[
\binom{n}{k} = \frac{n!}{k!(n-k)!}
\]
```

It is commonly used in combinatorics and probability.

## 10. Numbered and Long Equations
The `equation` environment automatically numbers equations.

```latex
\begin{equation}
\int_0^1 x^2\,dx = \frac{1}{3}
\end{equation}
```

For long equations, use the `multline` environment.

```latex
\begin{multline*}
p(x)=3x^6+14x^5y+590x^4y^2\\
-12x^2y^4-12xy^5+2y^6-a^3b^3
\end{multline*}
```

Use `align` to align multiple equations at a particular symbol.

```latex
\begin{align*}
2x-5y &= 8 \\
3x+9y &= -12
\end{align*}
```

Use `gather` to group and center multiple equations.

## 11. Matrices in LaTeX
The `amsmath` package provides several matrix environments.

**Basic Matrix:**

```latex
\[
\begin{matrix}
1 & 2 \\
3 & 4
\end{matrix}
\]
```

Different matrix environments:

- `matrix`: No surrounding delimiters.
- `pmatrix`: Parentheses.
- `bmatrix`: Square brackets.
- `Bmatrix`: Curly braces.
- `vmatrix`: Single vertical bars.
- `Vmatrix`: Double vertical bars.

Example:

```latex
\[
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
\]
```

For compact matrices inside text, use `smallmatrix`.

Extra row spacing can be added using:

```latex
\\[6pt]
```

## 12. Lists in LaTeX
LaTeX provides three common list environments.

**Itemize:** Creates unordered bullet lists.

```latex
\begin{itemize}
\item Apples
\item Oranges
\item Bananas
\end{itemize}
```

**Enumerate:** Creates numbered lists.

```latex
\begin{enumerate}
\item First step
\item Second step
\item Third step
\end{enumerate}
```

**Description:** Creates labeled lists.

```latex
\begin{description}
\item[HTML] HyperText Markup Language
\item[CSS] Cascading Style Sheets
\item[JS] JavaScript
\end{description}
```

## 13. Learning Outcomes
After studying these topics, learners should be able to:

- Write inline and display mathematical expressions.
- Use mathematical fonts and symbols.
- Create fractions, roots, sums, products, and integrals.
- Format arrays and piecewise functions.
- Write numbered and multiline equations.
- Create matrices with different delimiters.
- Use mathematical alignment environments.
- Create itemized, numbered, and description lists.
