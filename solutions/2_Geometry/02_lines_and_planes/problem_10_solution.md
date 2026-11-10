# Exercise 10 — Projection of a Point onto a Plane

## 1. Problem Statement
Project $P=(2,1,3)$ orthogonally onto $\Pi:x+y+z=3$, find its reflection across the plane, and verify that the midpoint of $P$ and the reflection lies on $\Pi$.

## 2. Theoretical Background and Concepts
For a plane $n\cdot X=d$, the orthogonal projection of a point $P$ is

$$
H=P-\frac{n\cdot P-d}{n\cdot n}n.
$$

The reflection is $R=2H-P$. The vector $P-H$ must be parallel to $n$, and $H$ lies on the plane.

## 3. Detailed Step-by-Step Solution
Here $n=(1,1,1)$, $d=3$, $n\cdot P=2+1+3=6$, and $n\cdot n=3$. Thus the correction factor is $(6-3)/3=1$ and

$$
H=(2,1,3)-1(1,1,1)=(1,0,2).
$$

Reflect by doubling the foot and subtracting the original point:

$$
R=2(1,0,2)-(2,1,3)=(2,0,4)-(2,1,3)=(0,-1,1).
$$

## 4. Verification and Consistency Checks
The foot lies on the plane because $1+0+2=3$. The displacement $P-H=(1,1,1)=n$ is perpendicular to the plane. The midpoint satisfies

$$
\frac{P+R}{2}=\left(\frac{2+0}{2},\frac{1-1}{2},\frac{3+1}{2}\right)=(1,0,2)=H,
$$

and its coordinates sum to $3$. Also $H-R=(1,1,1)$, so $P$ and $R$ are equally far from the plane on opposite sides.

## 5. Final Answer
Orthogonal projection $H=(1,0,2)$; reflection $R=(0,-1,1)$.
