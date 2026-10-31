# Exercise 6 — A Parameter and Invertibility

## 1. Problem Statement

For
$
A(t)=\begin{pmatrix}t&1\\2&t\end{pmatrix},
$
find all values of $t$ for which $A(t)$ is not invertible. Explain the connection with the determinant.

## 2. Method and Key Formula

A square matrix is invertible exactly when its determinant is nonzero. For a $2\times2$ matrix,
$
\det\begin{pmatrix}a&b\\c&d\end{pmatrix}=ad-bc.
$
Thus, find the determinant as a function of $t$, then solve $\det A(t)=0$.

## 3. Detailed Step-by-Step Solution

Calculate the determinant:
$\det A(t)=t\cdot t-1\cdot2$  
$=t^2-2.$
The matrix is not invertible when
$
t^2-2=0.
$
Solving,
$
t^2=2
\quad\Longrightarrow\quad
t=\pm\sqrt{2}.
$
For all other real values of $t$, $t^2-2\neq0$, so the matrix is invertible.

## 4. Verification and Consistency Checks

Substituting either exceptional value gives
$
(\pm\sqrt2)^2-2=2-2=0.
$
Hence both values make the determinant zero, as required.

## 5. Final Answer

$
\boxed{t=\sqrt2\ \text{or}\ t=-\sqrt2}
$
These are exactly the values for which $A(t)$ is not invertible.