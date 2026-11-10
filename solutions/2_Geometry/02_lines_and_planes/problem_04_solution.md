# Exercise 4 — Plane Through Three Points

## 1. Problem Statement
Find the plane through $A=(1,0,0)$, $B=(0,1,0)$ and $C=(0,0,1)$ by constructing two in-plane vectors and their cross product. Verify all three points.

## 2. Theoretical Background and Concepts
Two nonparallel vectors $u=B-A$ and $v=C-A$ lie in the required plane. Their cross product $u\times v$ is a nonzero normal, so the plane is $(u\times v)\cdot(X-A)=0$.

## 3. Detailed Step-by-Step Solution
Form the displacements:

$$
u=B-A=(-1,1,0),\qquad v=C-A=(-1,0,1).
$$

Compute the cross product component by component:

$$
\begin{aligned}
u\times v&=(u_2v_3-u_3v_2,\;u_3v_1-u_1v_3,\;u_1v_2-u_2v_1)\\
&=(1\cdot1-0\cdot0,\;0\cdot(-1)-(-1)\cdot1,\;(-1)\cdot0-1\cdot(-1))\\
&=(1,1,1).
\end{aligned}
$$

Since the cross product is nonzero, the points are not collinear. With normal $n=(1,1,1)$ and point $A$:

$$
(x-1)+y+z=0\quad\Longrightarrow\quad x+y+z=1.
$$

## 4. Verification and Consistency Checks
$A$ gives $1+0+0=1$, $B$ gives $0+1+0=1$ and $C$ gives $0+0+1=1$. Also $n\cdot u=-1+1=0$ and $n\cdot v=-1+1=0$.

## 5. Final Answer
The unique plane is $x+y+z=1$.
