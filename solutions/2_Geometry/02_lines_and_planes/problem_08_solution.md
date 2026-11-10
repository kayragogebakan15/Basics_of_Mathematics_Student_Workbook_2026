# Exercise 8 — Intersection Point of a Line and a Plane

## 1. Problem Statement
Find and verify the intersection of $(x,y,z)=(1,0,2)+t(1,2,-1)$ with the plane $x+y+z=4$.

## 2. Theoretical Background and Concepts
Substitute the line's coordinate expressions into the plane equation, solve for its parameter, then evaluate the point. A nonzero dot product between the line direction and plane normal ensures the intersection is unique.

## 3. Detailed Step-by-Step Solution
The parametric coordinates are $x=1+t$, $y=2t$, $z=2-t$. Substitute them:

$$
(1+t)+2t+(2-t)=4.
$$

Collect terms and solve:

$$
3+2t=4\quad\Longrightarrow\quad t=\frac12.
$$

Evaluate all three coordinates:

$$
X\left(\frac12\right)=\left(1+\frac12,2\cdot\frac12,2-\frac12\right)=\left(\frac32,1,\frac32\right).
$$

## 4. Verification and Consistency Checks
For the plane, $\frac32+1+\frac32=4$. For the line, subtracting its base point gives $(\frac12,1,-\frac12)=\frac12(1,2,-1)$. Finally $n\cdot v=(1,1,1)\cdot(1,2,-1)=2\ne0$, proving uniqueness.

## 5. Final Answer
The unique intersection point is $(\frac32,1,\frac32)$.
