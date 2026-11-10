# Exercise 12 — Intersection Line of Two Planes

## 1. Problem Statement
Find a parametric equation for the common line of $x+y+z=3$ and $x-y+z=1$. Derive its direction from the system and from a cross product; compare them.

## 2. Theoretical Background and Concepts
The intersection of two nonparallel planes is a line. Solving both plane equations gives a point and a free direction. Independently, the cross product of their nonparallel normals is perpendicular to both normals and hence lies along the intersection.

## 3. Detailed Step-by-Step Solution
Subtract the second plane equation from the first:

$$
(x+y+z)-(x-y+z)=3-1\quad\Longrightarrow\quad 2y=2\quad\Longrightarrow\quad y=1.
$$

Substitute $y=1$ into $x+y+z=3$:

$$
x+z=2.
$$

Set $z=t$, so $x=2-t$. The intersection line is

$$
(x,y,z)=(2-t,1,t)=(2,1,0)+t(-1,0,1).
$$

Its direction from the system is $v=(-1,0,1)$. For the geometric method, the normals are $n_1=(1,1,1)$ and $n_2=(1,-1,1)$; compute

$$
\begin{aligned}
n_1\times n_2&=(1\cdot1-1(-1),\;1\cdot1-1\cdot1,\;1(-1)-1\cdot1)\\
&=(2,0,-2)=-2(-1,0,1)=-2v.
\end{aligned}
$$

## 4. Verification and Consistency Checks
Substitute the parametric point into both original planes:

$$
(2-t)+1+t=3,\qquad (2-t)-1+t=1.
$$

Both identities hold for all $t$. The cross product is nonzero and proportional to the algebraic direction, so the two constructions agree despite opposite orientations.

## 5. Final Answer
The intersection is $(x,y,z)=(2,1,0)+t(-1,0,1)$, with equivalent direction $(2,0,-2)$ from the cross product.
