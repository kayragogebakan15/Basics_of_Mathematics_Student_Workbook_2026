# Exercise 2 — Distance as the Length of a Vector

## 1. Problem Statement
The points are $A=(1,2,3)$ and $B=(4,-2,6)$.
1. Construct $\overrightarrow{AB}$.
2. Compute its length.
3. Compute the distance between the points using the coordinate formula.
4. Explain why both calculations give the same result.

## 2. Method and Key Formula
The displacement from $A$ to $B$ is $\overrightarrow{AB}=B-A$. The Euclidean length of a vector $w=(w_1,w_2,w_3)$ is
$$\|w\|=\sqrt{w_1^2+w_2^2+w_3^2}.$$
The distance formula between two points is the length of their difference vector.

## 3. Detailed Step-by-Step Solution
Subtract the coordinates of $A$ from those of $B$:
$$\overrightarrow{AB}=(4-1,-2-2,6-3)=(3,-4,3).$$
Its length is
$$
\begin{aligned}
\|\overrightarrow{AB}\|
&=\sqrt{3^2+(-4)^2+3^2}\\
&=\sqrt{9+16+9}=\sqrt{34}.
\end{aligned}
$$
Using the point-distance formula directly,
$$
\begin{aligned}
d(A,B)
&=\sqrt{(4-1)^2+(-2-2)^2+(6-3)^2}\\
&=\sqrt{3^2+(-4)^2+3^2}=\sqrt{34}.
\end{aligned}
$$

## 4. Verification and Consistency Checks
Both methods give $\sqrt{34}$. This is not a coincidence: the coordinate differences in the distance formula are exactly the components of $B-A$. Therefore, $d(A,B)=\|B-A\|$.

## 5. Final Answer
$$\boxed{\overrightarrow{AB}=(3,-4,3),\qquad d(A,B)=\sqrt{34}.}$$