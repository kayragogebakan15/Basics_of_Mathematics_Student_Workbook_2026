# Exercise 13 — Undoing a Composite Transformation

## 1. Problem Statement
The matrices
$$S=\begin{pmatrix}2&0\\0&1\end{pmatrix},\qquad H=\begin{pmatrix}1&1\\0&1\end{pmatrix}$$
describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways: (1) first compute $T$, then its inverse; (2) use $(HS)^{-1}=S^{-1}H^{-1}$. Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain the rule: “when undoing a composition of operations, we undo them from the end.”

## 2. Method and Key Formula
For invertible matrices, $(AB)^{-1}=B^{-1}A^{-1}$. The order reverses because the last transformation applied must be undone first.

## 3. Detailed Step-by-Step Solution
**Method 1: calculate $T$ first.** Use row-by-column multiplication:
$
\begin{aligned}
T=HS
&=\begin{pmatrix}1&1\\0&1\end{pmatrix}
\begin{pmatrix}2&0\\0&1\end{pmatrix}\\
&=\begin{pmatrix}
1\cdot2+1\cdot0&1\cdot0+1\cdot1\\
0\cdot2+1\cdot0&0\cdot0+1\cdot1
\end{pmatrix}\\
&=\begin{pmatrix}2&1\\0&1\end{pmatrix}.
\end{aligned}
$
Its determinant is $2$, so
$$
T^{-1}=\frac12\begin{pmatrix}1&-1\\0&2\end{pmatrix}
=\begin{pmatrix}\frac12&-\frac12\\0&1\end{pmatrix}.
$$
**Method 2: reverse the factors.**
Since $S$ is diagonal, its inverse is obtained by taking reciprocals:
$S^{-1}=\begin{pmatrix}\frac12&0\\0&1\end{pmatrix}.$
For $H$, $\det H=1\cdot1-1\cdot0=1$. The $2\times2$ inverse formula gives
$H^{-1}=\frac11\begin{pmatrix}1&-1\\0&1\end{pmatrix}
=\begin{pmatrix}1&-1\\0&1\end{pmatrix}.$
Calculate the correct order:
$
\begin{aligned}
S^{-1}H^{-1}
&=\begin{pmatrix}\frac12&0\\0&1\end{pmatrix}
\begin{pmatrix}1&-1\\0&1\end{pmatrix}\\
&=\begin{pmatrix}
\frac12\cdot1+0\cdot0&\frac12\cdot(-1)+0\cdot1\\
0\cdot1+1\cdot0&0\cdot(-1)+1\cdot1
\end{pmatrix}
=\begin{pmatrix}\frac12&-\frac12\\0&1\end{pmatrix}.
\end{aligned}
$
The incorrect order gives
$
\begin{aligned}
H^{-1}S^{-1}
&=\begin{pmatrix}1&-1\\0&1\end{pmatrix}
\begin{pmatrix}\frac12&0\\0&1\end{pmatrix}\\
&=\begin{pmatrix}
1\cdot\frac12+(-1)\cdot0&1\cdot0+(-1)\cdot1\\
0\cdot\frac12+1\cdot0&0\cdot0+1\cdot1
\end{pmatrix}
=\begin{pmatrix}\frac12&-1\\0&1\end{pmatrix}.
\end{aligned}
$
The order reverses because $HS$ applies $S$ first and $H$ second. To undo it, undo $H$ first, then $S$, giving $S^{-1}H^{-1}$. Indeed,
$S^{-1}H^{-1}HS=S^{-1}(H^{-1}H)S=S^{-1}IS=I.$

## 4. Verification and Consistency Checks
Multiplying $T$ by the proposed inverse:
$$
\begin{pmatrix}2&1\\0&1\end{pmatrix}
\begin{pmatrix}\frac12&-\frac12\\0&1\end{pmatrix}
=\begin{pmatrix}1&0\\0&1\end{pmatrix}.
$$
The two correct methods agree, while reversing the factors incorrectly does not produce the inverse.

## 5. Final Answer
$$\boxed{T^{-1}=S^{-1}H^{-1}=\begin{pmatrix}\frac12&-\frac12\\0&1\end{pmatrix}.}$$