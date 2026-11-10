# Exercise 13 — Closest Point on a Plane

## 1. Problem Statement
Find the point of $x+2y+2z=4$ closest to $P=(3,0,0)$, its distance from $P$, and prove the connecting segment is perpendicular to the plane.

## 2. Theoretical Background and Concepts
The nearest point on a plane is the orthogonal projection. For a plane $n\cdot X=d$, the foot is $H=P-\frac{n\cdot P-d}{n\cdot n}n$, and the distance is $\frac{|n\cdot P-d|}{\|n\|}$. Orthogonality guarantees minimality by the Pythagorean theorem: every other plane point adds a perpendicular in-plane displacement to the shortest segment.

## 3. Detailed Step-by-Step Solution
Here $n=(1,2,2)$, $n\cdot P=3$, $d=4$ and $n\cdot n=1+4+4=9$. Therefore

$$
\frac{n\cdot P-d}{n\cdot n}=\frac{3-4}{9}=-\frac19.
$$

Compute the foot:

$$
\begin{aligned}
H&=(3,0,0)-\left(-\frac19\right)(1,2,2)\\
&=\left(3+\frac19,\frac29,\frac29\right)\\
&=\left(\frac{28}{9},\frac29,\frac29\right).
\end{aligned}
$$

The shortest distance is

$$
d(P,\Pi)=\frac{|3-4|}{\sqrt9}=\frac13.
$$

## 4. Verification and Consistency Checks
Plane membership is exact:

$$
\frac{28}{9}+2\frac29+2\frac29=\frac{28+4+4}{9}=4.
$$

The connecting vector is $H-P=(1/9,2/9,2/9)=n/9$, so it is perpendicular to every in-plane direction. Its length is $\sqrt{1+4+4}/9=3/9=1/3$, matching the distance formula. For any other point $Y$ of the plane, $(Y-H)\cdot(P-H)=0$ and thus $\|P-Y\|^2=\|P-H\|^2+\|H-Y\|^2\ge\|P-H\|^2$.

## 5. Final Answer
Closest point $H=(28/9,2/9,2/9)$; minimum distance $1/3$.
