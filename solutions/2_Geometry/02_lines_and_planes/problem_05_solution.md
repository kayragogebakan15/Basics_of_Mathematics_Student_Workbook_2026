# Exercise 5 — Relative Position of Two Lines

## 1. Problem Statement
Classify $L_1:(x,y,z)=(1,1,0)+t(1,2,1)$ and $L_2:(x,y,z)=(2,0,1)+s(0,1,-1)$ as intersecting, parallel or skew. Give an intersection point if one exists.

## 2. Theoretical Background and Concepts
Two lines in three dimensions are parallel only if their direction vectors are scalar multiples. If they are not parallel, they intersect exactly when one pair of parameter values satisfies all three coordinate equations. Otherwise they are skew.

## 3. Detailed Step-by-Step Solution
The direction vectors are $v_1=(1,2,1)$ and $v_2=(0,1,-1)$. They are not scalar multiples: any multiple of $v_2$ has first component zero, while $v_1$ does not.

Equating the parametric coordinates gives

$$
\begin{cases}
1+t=2,\\
1+2t=s,\\
t=1-s.
\end{cases}
$$

The first equation gives $t=1$. The second gives $s=1+2(1)=3$. But the third would require $1=1-3=-2$, a contradiction. In fact, the first two equations produce $(2,3,1)$ on $L_1$ and $(2,3,-2)$ on $L_2$; their $z$ coordinates differ.

## 4. Verification and Consistency Checks
The first-coordinate equation fixes $t$ uniquely and then the second fixes $s$ uniquely, so no other pair can resolve the failed third equation. Since the directions are not proportional, parallelism is also excluded.

## 5. Final Answer
The lines are **skew**: they are neither parallel nor intersecting.
