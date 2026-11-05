# Exercise 12 — A Normal Vector to a Plane

## 1. Problem Statement
Given $A=(1,0,2)$, $B=(2,1,0)$, and $C=(0,3,1)$. Construct two vectors lying in the plane, find a vector perpendicular to both, and check the perpendicularity using dot products.

## 2. Method and Key Formula
Two vectors in the plane can be formed from differences of points, using the same starting point. Their cross product is perpendicular to both:
$$n=\overrightarrow{AB}\times\overrightarrow{AC}.$$
A dot product of zero verifies perpendicularity.

## 3. Detailed Step-by-Step Solution
Construct the vectors from $A$:
$$\overrightarrow{AB}=B-A=(2-1,1-0,0-2)=(1,1,-2),$$
$$\overrightarrow{AC}=C-A=(0-1,3-0,1-2)=(-1,3,-1).$$
Calculate their cross product:
$$
\begin{aligned}
n
&=(1,1,-2)\times(-1,3,-1)\\
&=(1\cdot(-1)-(-2)\cdot3,\;(-2)\cdot(-1)-1\cdot(-1),\;1\cdot3-1\cdot(-1))\\
&=(5,3,4).
\end{aligned}
$$

## 4. Verification and Consistency Checks
Check against the first plane vector:
$$n\cdot\overrightarrow{AB}=(5,3,4)\cdot(1,1,-2)=5+3-8=0.$$
Check against the second:
$$n\cdot\overrightarrow{AC}=(5,3,4)\cdot(-1,3,-1)=-5+9-4=0.$$
Both dot products are zero, so $n$ is perpendicular to both vectors. Since the cross product is nonzero, the two direction vectors are not parallel and determine a plane.

## 5. Final Answer
$$\boxed{n=(5,3,4)}$$
Any nonzero scalar multiple of this vector is also a valid normal vector.