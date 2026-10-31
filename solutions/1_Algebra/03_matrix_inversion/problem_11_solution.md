# Exercise 11 — Parameter and Invertibility

## 1. Problem Statement
For
$$A(t)=\begin{pmatrix}1&t\\t&1\end{pmatrix}$$
find all $t$ for which the matrix is invertible, and then give a formula for $A(t)^{-1}$. Explain what happens to this formula at the excluded values.

## 2. Method and Key Formula
A $2\times2$ matrix is invertible exactly when its determinant is nonzero. For $\begin{pmatrix}a&b\\c&d\end{pmatrix}$, its inverse is $\frac1{ad-bc}\begin{pmatrix}d&-b\\-c&a\end{pmatrix}$ when $ad-bc\ne0$.

## 3. Detailed Step-by-Step Solution
Calculate the determinant as a function of $t$:
$$\det(A(t))=1\cdot1-t\cdot t=1-t^2=(1-t)(1+t).$$
It is zero at $t=1$ and $t=-1$. Thus the matrix is invertible for every real $t$ except these two values. Applying the inverse formula,
$$
A(t)^{-1}=\frac{1}{1-t^2}
\begin{pmatrix}1&-t\\-t&1\end{pmatrix},\qquad t\ne\pm1.
$$
At $t=1$, the two rows are equal. At $t=-1$, the second row is the negative of the first. In either case the rows are dependent and the denominator in the inverse formula is zero.

## 4. Verification and Consistency Checks
For $t\ne\pm1$,
$$
A(t)A(t)^{-1}
=\frac1{1-t^2}
\begin{pmatrix}1-t^2&-t+t\\t-t&1-t^2\end{pmatrix}
=I_2.
$$
The formula is therefore valid exactly on the stated domain.

## 5. Final Answer
$$\boxed{t\in\mathbb R\setminus\{-1,1\},\qquad
A(t)^{-1}=\frac1{1-t^2}\begin{pmatrix}1&-t\\-t&1\end{pmatrix}.}$$