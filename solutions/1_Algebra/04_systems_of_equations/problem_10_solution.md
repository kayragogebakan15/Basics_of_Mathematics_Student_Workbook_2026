# Exercise 10 — A Polynomial Through Three Points

## 1. Problem Statement
Find a polynomial $p(x)=ax^2+bx+c$ whose graph passes through $(0,1)$, $(1,3)$, and $(2,9)$. Reduce the problem to a system of equations and check the result by substituting all three points.

## 2. Method and Key Formula
A point $(x_0,y_0)$ lies on the graph exactly when $p(x_0)=y_0$. Substituting the three given points gives three linear equations for the unknown coefficients $a,b,c$.

## 3. Detailed Step-by-Step Solution
From $(0,1)$:
$$a(0)^2+b(0)+c=1\quad\Longrightarrow\quad c=1.$$
From $(1,3)$:
$$a+b+c=3\quad\Longrightarrow\quad a+b=2.$$
From $(2,9)$:
$$4a+2b+c=9\quad\Longrightarrow\quad 4a+2b=8,$$
or $2a+b=4$.
Subtract $a+b=2$ from $2a+b=4$ to obtain $a=2$. Then $b=0$, and $c=1$.

The coefficient system can be written as
$$
\begin{pmatrix}0&0&1\\1&1&1\\4&2&1\end{pmatrix}
\begin{pmatrix}a\\b\\c\end{pmatrix}
=\begin{pmatrix}1\\3\\9\end{pmatrix}.
$$

## 4. Verification and Consistency Checks
The resulting polynomial is $p(x)=2x^2+1$. Evaluate it at the three $x$-coordinates:
$$p(0)=1,\qquad p(1)=2+1=3,\qquad p(2)=2(4)+1=9.$$
All three points lie on the graph.

## 5. Final Answer
$$\boxed{p(x)=2x^2+1.}$$