# Exercise 13 — Do Four Points Lie in One Plane?

## 1. Problem Statement
Given
$$A=(0,0,0),\quad B=(1,2,0),\quad C=(0,1,1),\quad D=(2,5,1).$$
1. Construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$.
2. Find $n=\overrightarrow{AB}\times\overrightarrow{AC}$.
3. Construct $\overrightarrow{AD}$ and check whether $\overrightarrow{AD}\cdot n=0$.
4. Based on this, decide whether $D$ lies in the plane determined by $A,B,C$, and justify the criterion.

## 2. Method and Key Formula
The cross product of two non-parallel direction vectors in a plane gives a normal vector $n$. A displacement from a point in that plane lies in the plane exactly when it is perpendicular to the normal:
$$\overrightarrow{AD}\cdot n=0.$$

## 3. Detailed Step-by-Step Solution
Since $A$ is the origin,
$$\overrightarrow{AB}=B-A=(1,2,0),\qquad
\overrightarrow{AC}=C-A=(0,1,1).$$
Find the normal:
$$
\begin{aligned}
n
&=(1,2,0)\times(0,1,1)\\
&=(2\cdot1-0\cdot1,\;0\cdot0-1\cdot1,\;1\cdot1-2\cdot0)\\
&=(2,-1,1).
\end{aligned}
$$
Construct the final displacement:
$$\overrightarrow{AD}=D-A=(2,5,1).$$
Now calculate the dot product:
$$\overrightarrow{AD}\cdot n=2\cdot2+5\cdot(-1)+1\cdot1=4-5+1=0.$$

## 4. Verification and Consistency Checks
The zero dot product means $\overrightarrow{AD}$ is perpendicular to the normal and therefore lies parallel to the plane through $A$. Since it starts at $A$, point $D$ lies in the plane. As an additional check, $n$ is perpendicular to the two defining directions:
$$n\cdot\overrightarrow{AB}=2-2+0=0,\qquad
n\cdot\overrightarrow{AC}=0-1+1=0.$$

## 5. Final Answer
$$\boxed{D\text{ lies in the plane determined by }A,B,C.}$$