# Exercise 14 — Closest Point on a Line

## 1. Problem Statement
Given a point $P=(4,1)$ and a line through the origin with direction $v=(1,2)$. Using projection, find the closest point on the line, the distance from $P$ to the line, and verify that the appropriate vector is perpendicular to the direction of the line.

## 2. Method and Key Formula
The closest point on a line through the origin in direction $v$ is the projection of $P$ onto $v$:
$$Q=\operatorname{proj}_v P=\frac{P\cdot v}{v\cdot v}v.$$
The residual vector $P-Q$ is perpendicular to the line. Its length is the shortest distance.

## 3. Detailed Step-by-Step Solution
Calculate the dot products:
$$P\cdot v=4\cdot1+1\cdot2=6,\qquad v\cdot v=1^2+2^2=5.$$
Therefore, the projection and closest point are
$$
Q=\frac65(1,2)=\left(\frac65,\frac{12}5\right).
$$
The vector from $Q$ to $P$ is
$$
\begin{aligned}
P-Q
&=(4,1)-\left(\frac65,\frac{12}5\right)\\
&=\left(\frac{20-6}5,\frac{5-12}5\right)
=\left(\frac{14}5,-\frac75\right).
\end{aligned}
$$
Its length is
$$
\begin{aligned}
d(P,\text{line})
&=\|P-Q\|\\
&=\sqrt{\left(\frac{14}5\right)^2+\left(-\frac75\right)^2}\\
&=\sqrt{\frac{196+49}{25}}
=\frac{\sqrt{245}}5=\frac{7\sqrt5}{5}.
\end{aligned}
$$

## 4. Verification and Consistency Checks
Check that the residual is perpendicular to the line:
$$
(P-Q)\cdot v=\frac{14}5\cdot1-\frac75\cdot2
=\frac{14}5-\frac{14}5=0.
$$
Thus $Q$ is the perpendicular foot. Any other point on the line has a nonzero component along the line relative to $Q$, so its distance from $P$ is at least $\|P-Q\|$.

## 5. Final Answer
$$\boxed{
Q=\left(\frac65,\frac{12}5\right),\qquad
d(P,\text{line})=\frac{7\sqrt5}{5}.
}$$