# Exercise 11 — When Do Matrices Commute?

## 1. Problem Statement

Given
\[
A=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad
B=\begin{pmatrix}a&b\\c&d\end{pmatrix},
\]
find the conditions on \(a,b,c,d\) for which \(AB=BA\), and describe all such matrices \(B\).

## 2. Theoretical Background and Concepts

Two square matrices commute when their products in both orders are equal. To find the conditions, compute both products and equate corresponding entries.

## 3. Detailed Step-by-Step Solution

Compute
\[
AB=\begin{pmatrix}1&1\\0&1\end{pmatrix}
\begin{pmatrix}a&b\\c&d\end{pmatrix}
=\begin{pmatrix}a+c&b+d\\c&d\end{pmatrix}.
\]
In the opposite order,
\[
BA=\begin{pmatrix}a&b\\c&d\end{pmatrix}
\begin{pmatrix}1&1\\0&1\end{pmatrix}
=\begin{pmatrix}a&a+b\\c&c+d\end{pmatrix}.
\]
Set the corresponding entries equal:
\[
a+c=a\Rightarrow c=0,
\]
\[
b+d=a+b\Rightarrow d=a,
\]
and the bottom-right equality \(d=c+d\) again gives \(c=0\). The remaining equality is then automatically satisfied.

Thus \(c=0\), \(d=a\), while \(a\) and \(b\) may be arbitrary.

## 4. Verification and Consistency Checks

Substituting \(c=0\) and \(d=a\) gives
\[
AB=\begin{pmatrix}a&b+a\\0&a\end{pmatrix}
=BA.
\]
Therefore, every matrix of the stated form commutes with \(A\).

## Final Answer

\[
\boxed{B=\begin{pmatrix}a&b\\0&a\end{pmatrix},\quad a,b\text{ arbitrary}.}
\]
