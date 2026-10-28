# Exercise 13 — A Recurrence Written in Matrix Form

## 1. Problem Statement

Let
\[
F=\begin{pmatrix}1&1\\1&0\end{pmatrix}.
\]
Compute \(F^2,F^3,F^4,F^5\), compare the entries with the Fibonacci sequence \(0,1,1,2,3,5,8,\ldots\), and explain how \(F(a,b)^T\) performs a recurrence step.

## 2. Theoretical Background and Concepts

The Fibonacci sequence is defined by \(f_0=0\), \(f_1=1\), and \(f_{n+1}=f_n+f_{n-1}\). Matrix multiplication can update a pair of consecutive terms at once.

## 3. Detailed Step-by-Step Solution

\[
F^2=\begin{pmatrix}2&1\\1&1\end{pmatrix},\quad
F^3=\begin{pmatrix}3&2\\2&1\end{pmatrix},\quad
F^4=\begin{pmatrix}5&3\\3&2\end{pmatrix},\quad
F^5=\begin{pmatrix}8&5\\5&3\end{pmatrix}.
\]
The Fibonacci numbers appear in these matrices. More precisely, for \(n\geq1\),
\[
F^n=\begin{pmatrix}f_{n+1}&f_n\\f_n&f_{n-1}\end{pmatrix}.
\]
For example, \(F^5=\begin{pmatrix}f_6&f_5\\f_5&f_4\end{pmatrix}=\begin{pmatrix}8&5\\5&3\end{pmatrix}\).

For a general column vector,
\[
F\begin{pmatrix}a\\b\end{pmatrix}
=\begin{pmatrix}1&1\\1&0\end{pmatrix}
\begin{pmatrix}a\\b\end{pmatrix}
=\begin{pmatrix}a+b\\a\end{pmatrix}.
\]
The new first component is the sum of the old two components; the new second component keeps the old first component. Thus, if the state is \((f_n,f_{n-1})^T\), the new state is \((f_{n+1},f_n)^T\).

## 4. Verification and Consistency Checks

The first powers confirm the pattern:
\[
F^2=\begin{pmatrix}f_3&f_2\\f_2&f_1\end{pmatrix}
=\begin{pmatrix}2&1\\1&1\end{pmatrix},
\]
and the same indexing gives the displayed values for \(F^3,F^4,F^5\). Direct multiplication of a general vector also confirms the recurrence step.

## Final Answer

\[
\boxed{F^2=\begin{pmatrix}2&1\\1&1\end{pmatrix},F^3=\begin{pmatrix}3&2\\2&1\end{pmatrix},F^4=\begin{pmatrix}5&3\\3&2\end{pmatrix},F^5=\begin{pmatrix}8&5\\5&3\end{pmatrix}}
\]
and \(\boxed{F(a,b)^T=(a+b,a)^T}\).
