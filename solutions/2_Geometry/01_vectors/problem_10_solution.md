# Exercise 10 — Triangle Area from Vectors

## 1. Problem Statement
The points $A=(0,0,0)$, $B=(2,1,0)$, and $C=(1,3,2)$ form a triangle. Construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$, compute the area of the parallelogram using the cross product, and then find the area of the triangle. Explain the factor $\frac12$.

## 2. Method and Key Formula
The area of the parallelogram spanned by vectors $p$ and $q$ is $\|p\times q\|$. A diagonal divides a parallelogram into two congruent triangles, so the triangle area is half the parallelogram area.

## 3. Detailed Step-by-Step Solution
Construct the two side vectors from the common point $A$:
$$\overrightarrow{AB}=B-A=(2,1,0),$$
$$\overrightarrow{AC}=C-A=(1,3,2).$$
Calculate their cross product:
$$
\begin{aligned}
\overrightarrow{AB}\times\overrightarrow{AC}
&=(1\cdot2-0\cdot3,\;0\cdot1-2\cdot2,\;2\cdot3-1\cdot1)\\
&=(2,-4,5).
\end{aligned}
$$
Its magnitude is
$$
\begin{aligned}
\|\overrightarrow{AB}\times\overrightarrow{AC}\|
&=\sqrt{2^2+(-4)^2+5^2}\\
&=\sqrt{4+16+25}=\sqrt{45}=3\sqrt5.
\end{aligned}
$$
Therefore, the parallelogram area is $3\sqrt5$, and the triangle area is
$$A_{\triangle ABC}=\frac12(3\sqrt5)=\frac{3\sqrt5}{2}.$$

## 4. Verification and Consistency Checks
The cross product is nonzero, so the two side vectors are not parallel and the triangle has positive area. The factor $1/2$ is required because the triangle occupies exactly one half of the parallelogram formed by the same two side vectors.

## 5. Final Answer
$$\boxed{A_{\text{parallelogram}}=3\sqrt5,\qquad A_{\triangle ABC}=\frac{3\sqrt5}{2}.}$$