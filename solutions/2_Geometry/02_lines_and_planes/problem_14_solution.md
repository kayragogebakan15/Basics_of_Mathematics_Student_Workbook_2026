# Exercise 14 — Contrast: Intersection and Parallelism

## 1. Problem Statement
Through $P=(0,0,1)$ draw two lines with directions $v_1=(2,1,-1)$ and $v_2=(2,1,0)$. Classify each relative to $z=0$; find the intersection for the intersecting line and explain how to recognize parallelism for the other.

## 2. Theoretical Background and Concepts
The plane $z=0$ has normal $n=(0,0,1)$. For $L=P+tv$, the dot product $n\cdot v$ is the rate of change of the plane's left-hand side along the line. A nonzero value yields one crossing; zero means the line is parallel to the plane, and the line is contained only if its starting point also lies on the plane.

## 3. Detailed Step-by-Step Solution
For $v_1$, the line is

$$
L_1:(x,y,z)=(2t,t,1-t).
$$

Since $n\cdot v_1=-1\ne0$, it crosses once. Set $z=0$:

$$
1-t=0\quad\Longrightarrow\quad t=1,
$$

so the intersection point is $(2,1,0)$.

For $v_2$, the line is

$$
L_2:(x,y,z)=(2t,t,1).
$$

The dot product is $n\cdot v_2=0$. Its starting point has $z=1\ne0$, so the line is parallel to the plane and is not contained in it. In particular, its zero vertical direction component makes $z$ remain $1$ for all $t$, which identifies parallelism without solving an intersection equation.

## 4. Verification and Consistency Checks
For $L_1$ at $t=1$, $(2,1,0)$ has $z=0$; uniqueness follows from $n\cdot v_1\ne0$. For $L_2$, every point has $z=1$, which excludes both intersection and containment.

## 5. Final Answer
$L_1$ intersects the plane exactly at $(2,1,0)$; $L_2$ is strictly parallel to the plane and has no point in common with it.
