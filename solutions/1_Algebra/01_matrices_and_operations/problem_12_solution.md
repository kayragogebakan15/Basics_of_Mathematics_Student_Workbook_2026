# Exercise 12 — Formula for a Matrix Power

## 1. Problem Statement

Let
\[
A=\begin{pmatrix}1&1\\0&1\end{pmatrix}.
\]
Compute \(A^2,A^3,A^4\), conjecture a formula for \(A^n\), and justify it by induction.

## 2. Theoretical Background and Concepts

A matrix power is repeated multiplication. Mathematical induction proves a general formula by establishing a base case and showing that if it holds for \(n\), then it also holds for \(n+1\).

## 3. Detailed Step-by-Step Solution

\[
A^2=AA=
\begin{pmatrix}1&1\\0&1\end{pmatrix}
\begin{pmatrix}1&1\\0&1\end{pmatrix}
=\begin{pmatrix}
1\cdot1+1\cdot0&1\cdot1+1\cdot1\\
0\cdot1+1\cdot0&0\cdot1+1\cdot1
\end{pmatrix}
=\begin{pmatrix}1&2\\0&1\end{pmatrix}.
\]
The upper-right entry is \(1\cdot1+1\cdot1=2\). Multiplying once more,
\[
A^3=A^2A=
\begin{pmatrix}1&2\\0&1\end{pmatrix}
\begin{pmatrix}1&1\\0&1\end{pmatrix}
=\begin{pmatrix}
1\cdot1+2\cdot0&1\cdot1+2\cdot1\\
0\cdot1+1\cdot0&0\cdot1+1\cdot1
\end{pmatrix}
=\begin{pmatrix}1&3\\0&1\end{pmatrix}.
\]
Its upper-right entry is \(1\cdot1+2\cdot1=3\). Similarly,
\[
A^4=A^3A=
\begin{pmatrix}1&3\\0&1\end{pmatrix}
\begin{pmatrix}1&1\\0&1\end{pmatrix}
=\begin{pmatrix}
1\cdot1+3\cdot0&1\cdot1+3\cdot1\\
0\cdot1+1\cdot0&0\cdot1+1\cdot1
\end{pmatrix}
=\begin{pmatrix}1&4\\0&1\end{pmatrix}.
\]
Its upper-right entry is \(1\cdot1+3\cdot1=4.
\]
The upper-right entry equals the exponent, suggesting
\[
\boxed{A^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}}
\quad\text{for integers }n\geq1.
\]

### Inductive verification

**Base case:** For \(n=1\),
\[
A^1=\begin{pmatrix}1&1\\0&1\end{pmatrix},
\]
so the formula holds.

**Inductive step:** Assume
\[
A^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}.
\]
Multiplying by \(A\) and calculating each entry by the row-by-column rule,
\[
\begin{aligned}
A^{n+1}&=A^nA\\
&=\begin{pmatrix}1&n\\0&1\end{pmatrix}
\begin{pmatrix}1&1\\0&1\end{pmatrix}\\
&=\begin{pmatrix}
1\cdot1+n\cdot0&1\cdot1+n\cdot1\\
0\cdot1+1\cdot0&0\cdot1+1\cdot1
\end{pmatrix}\\
&=\begin{pmatrix}1&n+1\\0&1\end{pmatrix}.
\]
This is exactly the proposed formula with \(n+1\) in place of \(n\).

## 4. Verification and Consistency Checks

The formula reproduces the directly calculated powers for \(n=2,3,4\). The inductive step proves that it continues to hold for every integer \(n\geq1\), not merely for the first few examples.

## Final Answer

\[
\boxed{A^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}\quad(n\geq1)}.
\]
