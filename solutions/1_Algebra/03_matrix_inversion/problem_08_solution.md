# Exercise 8 — Inverse of a Transformation

## 1. Problem Statement
The matrix
$$S=\begin{pmatrix}2&0\\0&\frac12\end{pmatrix}$$
describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S,S^{-1}$ on one simple vector.

## 2. Method and Key Formula
A diagonal matrix with nonzero diagonal entries is inverted by taking the reciprocal of each diagonal entry:
$$\operatorname{diag}(a,b)^{-1}=\operatorname{diag}\left(\frac1a,\frac1b\right).$$
Geometrically, an inverse transformation undoes the original transformation.

## 3. Detailed Step-by-Step Solution
The matrix doubles the horizontal coordinate and halves the vertical coordinate. Therefore,
$$S^{-1}=\begin{pmatrix}\frac12&0\\0&2\end{pmatrix}.$$
Choose $v=\begin{pmatrix}2\\4\end{pmatrix}$. Applying $S$ gives
$$Sv=\begin{pmatrix}2&0\\0&\frac12\end{pmatrix}
\begin{pmatrix}2\\4\end{pmatrix}
=\begin{pmatrix}4\\2\end{pmatrix}.$$
Now apply the inverse:
$$S^{-1}(Sv)=\begin{pmatrix}\frac12&0\\0&2\end{pmatrix}
\begin{pmatrix}4\\2\end{pmatrix}
=\begin{pmatrix}2\\4\end{pmatrix}=v.$$

## 4. Verification and Consistency Checks
The matrix products are
$$SS^{-1}=S^{-1}S=\begin{pmatrix}1&0\\0&1\end{pmatrix}.$$
Thus the inverse restores every vector, not only the chosen example.

## 5. Final Answer
$$\boxed{S^{-1}=\begin{pmatrix}\frac12&0\\0&2\end{pmatrix}.}$$
It halves the horizontal coordinate and doubles the vertical coordinate, undoing the original scaling.