# Exercise 9 — Distances

## 1. Problem Statement
Calculate the distance from $P=(2,3)$ to $3x+4y-10=0$ and from $Q=(2,-1,3)$ to $2x-2y+z-4=0$. Compare the formulas geometrically.

## 2. Theoretical Background and Concepts
For a line $ax+by+c=0$ and point $(x_0,y_0)$, distance is

$$
d=\frac{|ax_0+by_0+c|}{\sqrt{a^2+b^2}}.
$$

For a plane $ax+by+cz+d_0=0$ and point $(x_0,y_0,z_0)$, distance is

$$
d=\frac{|ax_0+by_0+cz_0+d_0|}{\sqrt{a^2+b^2+c^2}}.
$$

Both formulas divide the magnitude of the signed equation residual by the length of the normal vector. This produces the perpendicular distance.

## 3. Detailed Step-by-Step Solution
For the line, $n=(3,4)$ and $\|n\|=\sqrt{3^2+4^2}=5$. Evaluate its left-hand side at $P$:

$$
3(2)+4(3)-10=6+12-10=8.
$$

Therefore

$$
d(P,L)=\frac{|8|}{5}=\frac85.
$$

For the plane, $n=(2,-2,1)$ and $\|n\|=\sqrt{4+4+1}=3$. Evaluate at $Q$:

$$
2(2)-2(-1)+3-4=4+2+3-4=5.
$$

Therefore

$$
d(Q,\Pi)=\frac{|5|}{3}=\frac53.
$$

## 4. Verification and Consistency Checks
Both distances are nonnegative and both normals are nonzero. The identical structure is expected: only the length of the normal changes from a two-component to a three-component norm. Each distance measures displacement along the unit normal rather than along an arbitrary path.

## 5. Final Answer
The distances are $\frac85$ to the line and $\frac53$ to the plane.
