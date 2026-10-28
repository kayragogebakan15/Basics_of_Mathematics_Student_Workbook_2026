# Exercise 9 — Composing Transformations

## 1. Problem Statement

Let
\[
S=\begin{pmatrix}2&0\\0&1\end{pmatrix},\qquad
R=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
x=\begin{pmatrix}1\\2\end{pmatrix}.
\]
Compute \(RSx\) and \(SRx\), compare them, and explain geometrically why the order matters.

## 2. Theoretical Background and Concepts

Matrix multiplication represents composition of linear transformations. In \(RSx\), the rightmost transformation \(S\) acts first, followed by \(R\). In \(SRx\), rotation \(R\) acts first, followed by scaling \(S\).

## 3. Detailed Step-by-Step Solution

### A. Compute \(RSx\)

First apply the scaling:
\[
Sx=\begin{pmatrix}2&0\\0&1\end{pmatrix}\begin{pmatrix}1\\2\end{pmatrix}
=\begin{pmatrix}2\\2\end{pmatrix}.
\]
Then rotate:
\[
RSx=R\begin{pmatrix}2\\2\end{pmatrix}
=\begin{pmatrix}-2\\2\end{pmatrix}.
\]

### B. Compute \(SRx\)

First rotate:
\[
Rx=\begin{pmatrix}0&-1\\1&0\end{pmatrix}\begin{pmatrix}1\\2\end{pmatrix}
=\begin{pmatrix}-2\\1\end{pmatrix}.
\]
Then scale the horizontal coordinate by 2:
\[
SRx=S\begin{pmatrix}-2\\1\end{pmatrix}
=\begin{pmatrix}-4\\1\end{pmatrix}.
\]

## 4. Verification and Consistency Checks

The results differ:
\[
RSx=\begin{pmatrix}-2\\2\end{pmatrix}
\ne
\begin{pmatrix}-4\\1\end{pmatrix}=SRx.
\]
Geometrically, scaling the horizontal coordinate before rotation affects both resulting coordinates after the rotation; rotating first changes which coordinate is then enlarged by the nonuniform scaling.

## Final Answer

\[
\boxed{RSx=\begin{pmatrix}-2\\2\end{pmatrix}},\qquad
\boxed{SRx=\begin{pmatrix}-4\\1\end{pmatrix}}.
\]
The transformations do not commute because the scaling is nonuniform.
