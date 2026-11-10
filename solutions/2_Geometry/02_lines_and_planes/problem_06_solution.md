# Exercise 6 — Angle Between Planes

## 1. Problem Statement
For $\Pi_1:x+y+z=1$ and $\Pi_2:x-y=2$, determine whether the planes are parallel, calculate their angle if not, and explain the role of their normals.

## 2. Theoretical Background and Concepts
Plane normals are the coefficient vectors in their Cartesian equations. Distinct planes are parallel exactly when their normals are proportional. The smaller (unoriented) angle $\theta$ between planes satisfies

$$
\cos\theta=\frac{|n_1\cdot n_2|}{\|n_1\|\,\|n_2\|},\qquad 0\le\theta\le90^\circ.
$$

The absolute value removes the arbitrary choice of sign for a plane's normal.

## 3. Detailed Step-by-Step Solution
Read off $n_1=(1,1,1)$ and $n_2=(1,-1,0)$. The vectors are not proportional, because their third components are $1$ and $0$. Their dot product is

$$
n_1\cdot n_2=1(1)+1(-1)+1(0)=0.
$$

Their norms are $\sqrt3$ and $\sqrt2$, both nonzero. Hence

$$
\cos\theta=\frac{|0|}{\sqrt3\sqrt2}=0,\qquad\theta=90^\circ.
$$

## 4. Verification and Consistency Checks
The planes' normal vectors are perpendicular; taking planes perpendicular to those normals gives a right dihedral angle. No points on the planes are needed because translating a plane leaves its orientation and normal unchanged.

## 5. Final Answer
The planes are not parallel; they are **perpendicular**, and their smaller angle is $90^\circ$.
