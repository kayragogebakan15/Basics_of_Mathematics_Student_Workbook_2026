# Exercise 5 — Row Echelon Form and Number of Solutions

## 1. Problem Statement
For the augmented matrix
$$\left[\begin{array}{ccc|c}1&2&-1&3\\0&1&2&1\\0&0&0&0\end{array}\right]$$
determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

## 2. Method and Key Formula
A pivot column identifies a leading variable. A non-pivot column identifies a free variable. A row $[0\ 0\ 0\mid c]$ with $c\ne0$ would indicate inconsistency; no such row appears here.

## 3. Detailed Step-by-Step Solution
The matrix represents
$$\begin{cases}x+2y-z=3,\\y+2z=1.\end{cases}$$
The pivot columns are columns 1 and 2, so $x$ and $y$ are leading variables. Column 3 has no pivot, so $z$ is free. Set $z=t$.

From the second equation,
$$y+2t=1\quad\Longrightarrow\quad y=1-2t.$$
Substitute into the first:
$$x+2(1-2t)-t=3,$$
$$x+2-5t=3\quad\Longrightarrow\quad x=1+5t.$$
Therefore the solution set is parameterized by $t$.

## 4. Verification and Consistency Checks
Substitute $x=1+5t$, $y=1-2t$, $z=t$:
$$x+2y-z=1+5t+2-4t-t=3,$$
$$y+2z=1-2t+2t=1.$$
Both equations hold for every real $t$. There is one free variable, so there are infinitely many solutions.

## 5. Final Answer
$$\boxed{(x,y,z)=(1+5t,1-2t,t),\quad t\in\mathbb R.}$$