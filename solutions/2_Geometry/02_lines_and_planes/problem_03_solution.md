# Exercise 3 — Plane Through a Point with a Given Normal Vector

## 1. Problem Statement
Find the plane through $P=(1,-2,3)$ with normal vector $n=(2,1,-1)$. Verify the point and explain what the normal does.

## 2. Theoretical Background and Concepts
A plane with nonzero normal $n=(a,b,c)$ through $P=(x_0,y_0,z_0)$ has equation $n\cdot(X-P)=0$, or $a(x-x_0)+b(y-y_0)+c(z-z_0)=0$. Its direction vectors are exactly the vectors orthogonal to $n$.

## 3. Detailed Step-by-Step Solution
Substitute the given point and normal:

$$
2(x-1)+(y+2)-(z-3)=0.
$$

Expand each term and combine constants:

$$
2x-2+y+2-z+3=0\quad\Longrightarrow\quad 2x+y-z+3=0.
$$

Equivalently, $2x+y-z=-3$.

## 4. Verification and Consistency Checks
At $P$, the left-hand side is $2(1)+(-2)-3+3=0$. If $X$ and $Y$ lie on the plane, subtracting their equations gives $n\cdot(X-Y)=0$, so every displacement along the plane is perpendicular to $n$.

## 5. Final Answer
The plane is $2x+y-z+3=0$, with normal $n=(2,1,-1)$.
