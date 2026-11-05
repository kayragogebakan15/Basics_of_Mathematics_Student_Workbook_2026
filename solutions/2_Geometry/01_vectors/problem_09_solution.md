# Exercise 9 — Cross Product as a Perpendicular Direction

## 1. Problem Statement
For $u=(1,2,0)$ and $v=(0,1,3)$ compute $u\times v$. Use dot products to check perpendicularity to both vectors, compute $v\times u$, and compare the results.

## 2. Method and Key Formula
For vectors in $\mathbb R^3$,
$$
u\times v=
\begin{pmatrix}
u_2v_3-u_3v_2\\
u_3v_1-u_1v_3\\
u_1v_2-u_2v_1
\end{pmatrix}.
$$
The cross product is perpendicular to both input vectors and is anti-commutative: $v\times u=-(u\times v)$.

## 3. Detailed Step-by-Step Solution
Substitute the components:
$$
\begin{aligned}
u\times v
&=(2\cdot3-0\cdot1,\;0\cdot0-1\cdot3,\;1\cdot1-2\cdot0)\\
&=(6,-3,1).
\end{aligned}
$$
Reverse the order:
$$
\begin{aligned}
v\times u
&=(1\cdot0-3\cdot2,\;3\cdot1-0\cdot0,\;0\cdot2-1\cdot1)\\
&=(-6,3,-1).
\end{aligned}
$$

## 4. Verification and Consistency Checks
Check perpendicularity to $u$:
$$(u\times v)\cdot u=(6,-3,1)\cdot(1,2,0)=6-6+0=0.$$
Check perpendicularity to $v$:
$$(u\times v)\cdot v=(6,-3,1)\cdot(0,1,3)=0-3+3=0.$$
Finally, $v\times u=(-6,3,-1)=-(6,-3,1)$, confirming the sign reversal when the order is swapped.

## 5. Final Answer
$$\boxed{u\times v=(6,-3,1),\qquad v\times u=(-6,3,-1)=-(u\times v).}$$