# Exercise 11 — Plane Containing a Line and a Point

## 1. Problem Statement
Find the plane containing $(x,y,z)=(1,0,2)+t(1,1,-1)$ and $P=(0,2,1)$. Verify the whole line and the point.

## 2. Theoretical Background and Concepts
A plane containing a line must contain its direction $v$. If $p$ is a point on the line, the vector $w=P-p$ is a second direction within the plane. If $v\times w\ne0$, the cross product is a normal and the plane is $(v\times w)\cdot(X-p)=0$.

## 3. Detailed Step-by-Step Solution
Choose the line's base point $p=(1,0,2)$ and its direction $v=(1,1,-1)$. The vector connecting it to the additional point is

$$
w=P-p=(0-1,2-0,1-2)=(-1,2,-1).
$$

Compute a normal:

$$
\begin{aligned}
v\times w&=(1(-1)-(-1)2,\;(-1)(-1)-1(-1),\;1(2)-1(-1))\\
&=(1,2,3).
\end{aligned}
$$

The cross product is nonzero, so the plane is uniquely determined. Using $p$:

$$
(x-1)+2(y-0)+3(z-2)=0\quad\Longrightarrow\quad x+2y+3z=7.
$$

## 4. Verification and Consistency Checks
At $P$, $0+2(2)+3(1)=7$. For an arbitrary point of the line, $(x,y,z)=(1+t,t,2-t)$:

$$
(1+t)+2t+3(2-t)=1+t+2t+6-3t=7
$$

for every $t$. The normal also satisfies $n\cdot v=1+2-3=0$ and $n\cdot w=-1+4-3=0$.

## 5. Final Answer
The required plane is $x+2y+3z=7$.
