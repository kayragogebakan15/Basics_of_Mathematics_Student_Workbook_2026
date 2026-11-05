# Exercise 6 — Projection and Perpendicular Component

## 1. Problem Statement
Find the projection of $u=(4,2)$ onto the direction $v=(1,1)$. Then compute
$$r=u-P_v(u),$$
where $P_v(u)$ denotes the projection of $u$ onto the direction of $v$. Verify that $r\cdot v=0$ and explain this result geometrically.

## 2. Method and Key Formula
For a nonzero vector $v$, the projection of $u$ onto the direction of $v$ is
$$P_v(u)=\frac{u\cdot v}{v\cdot v}v.$$
The scalar $\frac{u\cdot v}{v\cdot v}$ determines how far along the direction $v$ the projection lies. Subtracting this parallel component from $u$ gives the perpendicular component:
$$r=u-P_v(u).$$

## 3. Detailed Step-by-Step Solution
First calculate the dot products:
$$
\begin{aligned}
u\cdot v&=4\cdot1+2\cdot1=6,\\
v\cdot v&=1\cdot1+1\cdot1=2.
\end{aligned}
$$
Substitute these values into the projection formula:
$$
\begin{aligned}
P_v(u)
&=\frac{6}{2}(1,1)\\
&=3(1,1)\\
&=(3,3).
\end{aligned}
$$
Now subtract the projection from the original vector:
$$
\begin{aligned}
r&=u-P_v(u)\\
&=(4,2)-(3,3)\\
&=(1,-1).
\end{aligned}
$$

## 4. Verification and Consistency Checks
Check that the remaining component is perpendicular to $v$:
$$
r\cdot v=(1,-1)\cdot(1,1)=1\cdot1+(-1)\cdot1=1-1=0.
$$
Also verify that the two components reconstruct the original vector:
$$(3,3)+(1,-1)=(4,2)=u.$$
Thus, $u$ has been decomposed into a component parallel to $v$ and a component perpendicular to $v$. The projection is the parallel component, while $r$ is the perpendicular remainder.

## 5. Final Answer
$$\boxed{P_v(u)=(3,3),\qquad r=(1,-1),\qquad r\cdot v=0.}$$
