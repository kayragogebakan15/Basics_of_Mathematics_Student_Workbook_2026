# Exercise 3 — When Does the Inverse Not Exist?

## 1. Problem Statement
For
$$A=\begin{pmatrix}2&4\\1&2\end{pmatrix}$$
explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

## 2. Method and Key Formula
A square matrix is invertible if and only if its determinant is nonzero. Also, if the rows of a matrix are linearly dependent, its determinant is zero and it cannot have an inverse.

## 3. Detailed Step-by-Step Solution
**Method 1: determinant.** For this matrix,
$$\det(A)=2\cdot2-4\cdot1=4-4=0.$$
Because the determinant is zero, the inverse does not exist.

**Method 2: row dependence.** The first row is twice the second row:
$$(2,4)=2(1,2).$$
Thus the two rows are linearly dependent. They do not provide two independent row directions, so the matrix cannot be inverted.

## 4. Verification and Consistency Checks
Both tests give the same conclusion: the determinant is zero and the rows are dependent. In particular, no matrix $C$ can satisfy $AC=I$, because the two rows of $AC$ would remain dependent, whereas the two rows of $I$ are independent.

## 5. Final Answer
$$\boxed{A^{-1}\text{ does not exist because }\det(A)=0\text{ and the rows are dependent.}}$$