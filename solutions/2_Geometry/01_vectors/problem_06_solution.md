# Exercise 6 — Projection and Perpendicular Component

## 1. Problem Statement
Find the projection of $u=(4,2)$ onto the direction $v=(1,1)$. Then compute
$$r=u-\operatorname{proj}_v u$$
and verify that $r\cdot v=0$. Explain this result geometrically.

## 2. Method and Key Formula
The vector projection of $u$ onto a nonzero vector $v$ is
$$\operatorname{proj}_v u=\frac{u\cdot v}{v\cdot v}v.$$
Subtracting the projection from $u$ leaves the component perpendicular to $v$.

## 3. Detailed Step-by-Step Solution
Calculate the required dot products:
$$u\cdot v=4\cdot1+2\cdot1=6,\qquad v\cdot v=1^2+1^2=2.$$
Substitute into the projection formula:
$$\operatorname{proj}_v u=\frac62(1,1)=3(1,1)=(3,3).$$
Now subtract this parallel component:
$$r=u-\operatorname{proj}_v u=(4,2)-(3,3)=(1,-1).$$

## 4. Verification and Consistency Checks
Check perpendicularity:
$$r\cdot v=(1,-1)\cdot(1,1)=1-1=0.$$
Also, the decomposition is exact:
$$(3,3)+(1,-1)=(4,2)=u.$$
Geometrically, $(3,3)$ is the component of $u$ along the line in direction $v$, while $(1,-1)$ is the perpendicular remainder.

## 5. Final Answer
$$\boxed{\operatorname{proj}_v u=(3,3),\qquad r=(1,-1),\qquad r\cdot v=0.}$$