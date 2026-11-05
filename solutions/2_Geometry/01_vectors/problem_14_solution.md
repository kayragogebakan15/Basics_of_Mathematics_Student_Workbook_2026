# Exercise 14 — Closest Point on a Line

## 1. Problem Statement
Given a point $P=(4,1)$ and a line $L$ through the origin with direction $v=(1,2)$, use projection to find the closest point on the line and the distance from $P$ to the line. Verify that the vector from the closest point to $P$ is perpendicular to the direction of the line.

## 2. Method and Key Formula
The line can be written parametrically as
$$L=\{tv:t\in\mathbb R\}.$$
The closest point $Q$ on this line is the projection of $P$ onto the direction vector $v$. Denote this projection by $P_v(P)$:
$$Q=P_v(P)=\frac{P\cdot v}{v\cdot v}v.$$
The residual vector $P-Q$ is perpendicular to $v$. Consequently, the shortest distance from $P$ to the line is
$$d(P,L)=\|P-Q\|.$$

## 3. Detailed Step-by-Step Solution
First calculate the dot products:
$$
\begin{aligned}
P\cdot v&=4\cdot1+1\cdot2=6,\\
v\cdot v&=1\cdot1+2\cdot2=5.
\end{aligned}
$$
Substitute them into the projection formula to find the closest point:
$$
\begin{aligned}
Q
&=\frac{6}{5}(1,2)\\
&=\left(\frac65,\frac{12}{5}\right).
\end{aligned}
$$
The vector from $Q$ to $P$ is
$$
\begin{aligned}
P-Q
&=(4,1)-\left(\frac65,\frac{12}{5}\right)\\
&=\left(4-\frac65,1-\frac{12}{5}\right)\\
&=\left(\frac{20-6}{5},\frac{5-12}{5}\right)\\
&=\left(\frac{14}{5},-\frac75\right).
\end{aligned}
$$
Its length gives the distance from the point to the line:
$$
\begin{aligned}
d(P,L)
&=\|P-Q\|\\
&=\sqrt{\left(\frac{14}{5}\right)^2+\left(-\frac75\right)^2}\\
&=\sqrt{\frac{196}{25}+\frac{49}{25}}\\
&=\sqrt{\frac{245}{25}}\\
&=\frac{\sqrt{245}}5=\frac{7\sqrt5}{5}.
\end{aligned}
$$

## 4. Verification and Consistency Checks
Verify perpendicularity using the dot product:
$$
\begin{aligned}
(P-Q)\cdot v
&=\frac{14}{5}\cdot1-\frac75\cdot2\\
&=\frac{14}{5}-\frac{14}{5}\\
&=0.
\end{aligned}
$$
Therefore, $PQ$ is perpendicular to the line's direction. Since $Q$ lies on $L$ and the residual vector is perpendicular to $L$, $Q$ is the perpendicular foot and hence the closest point. Any other point on the line differs from $Q$ by a vector parallel to $v$; by the Pythagorean theorem, its distance from $P$ cannot be smaller than $\|P-Q\|$.

## 5. Final Answer
$$
\boxed{
Q=\left(\frac65,\frac{12}{5}\right),\qquad
d(P,L)=\frac{7\sqrt5}{5}.
}
$$
The perpendicularity check is $(P-Q)\cdot v=0$.
