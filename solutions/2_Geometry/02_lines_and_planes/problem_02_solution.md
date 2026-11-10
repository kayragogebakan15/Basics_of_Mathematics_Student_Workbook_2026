# Exercise 2 — A Line in Space

## 1. Problem Statement
For $L:(x,y,z)=(2,-1,3)+t(1,2,-2)$, identify a point and a direction vector, determine whether $P=(4,3,-1)$ lies on $L$, and find the point at $t=-1$.

## 2. Theoretical Background and Concepts
A parametric line $X=p+tv$ consists of all points obtained by adding multiples of its nonzero direction $v$ to a fixed point $p$. A candidate point belongs to the line only when the same parameter satisfies all three coordinate equations.

## 3. Detailed Step-by-Step Solution
The base point is $p=(2,-1,3)$ and the direction is $v=(1,2,-2)$. Write the coordinate equations:

$$
x=2+t,\qquad y=-1+2t,\qquad z=3-2t.
$$

For $P=(4,3,-1)$, the first coordinate forces $4=2+t$, hence $t=2$. Check the other coordinates using this same value:

$$
-1+2(2)=3,\qquad 3-2(2)=-1.
$$

Therefore $P$ lies on $L$. For $t=-1$:

$$
X(-1)=(2-1,-1-2,3+2)=(1,-3,5).
$$

## 4. Verification and Consistency Checks
The displacement from $p$ to $P$ is $P-p=(2,4,-4)=2(1,2,-2)$, independently confirming membership. Also $(1,-3,5)-(2,-1,3)=(-1,-2,2)=-v$.

## 5. Final Answer
Point $(2,-1,3)$; direction $(1,2,-2)$; $P$ belongs to $L$ at $t=2$; $X(-1)=(1,-3,5)$.
