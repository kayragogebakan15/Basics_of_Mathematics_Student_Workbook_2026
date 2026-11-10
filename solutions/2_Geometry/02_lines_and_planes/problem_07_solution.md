# Exercise 7 — A Line Relative to a Plane

## 1. Problem Statement
Determine whether $L:(x,y,z)=(1,1,0)+t(1,-1,0)$ intersects $\Pi:x+y+z=2$ once, lies in it, or is parallel without meeting it. Explain the dot-product test.

## 2. Theoretical Background and Concepts
For a line $p+tv$ and a plane $n\cdot X=d$, substitution gives $n\cdot p+t(n\cdot v)=d$. If $n\cdot v\ne0$, there is exactly one intersection. If $n\cdot v=0$, either the whole line is in the plane (when $n\cdot p=d$) or the two objects have no common points.

## 3. Detailed Step-by-Step Solution
The plane normal is $n=(1,1,1)$, the line direction is $v=(1,-1,0)$, and its base point is $p=(1,1,0)$. Compute

$$
n\cdot v=1-1+0=0,\qquad n\cdot p=1+1+0=2.
$$

Thus the line travels in a direction parallel to the plane and starts at a point of the plane. Substitution also gives

$$
(1+t)+(1-t)+0=2
$$

for every real $t$.

## 4. Verification and Consistency Checks
Both requirements are met: zero normal-direction component and an initial point satisfying the plane equation. Since every point of the line has the same value of $n\cdot X$, the complete line is contained in the plane.

## 5. Final Answer
$L$ **lies entirely in** $\Pi$; there are infinitely many common points.
