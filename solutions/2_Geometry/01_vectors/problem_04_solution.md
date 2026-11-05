# Exercise 4 — Dot Product and Perpendicularity

## 1. Problem Statement
For $u=(1,2,-1)$ and $v=(2,-1,3)$ compute $u\cdot v$ and determine whether the vectors are perpendicular. Then find $a$ so that $w=(2,-1,a)$ is perpendicular to $u$, and check the result.

## 2. Method and Key Formula
For vectors in $\mathbb R^3$,
$$u\cdot v=u_1v_1+u_2v_2+u_3v_3.$$
Two nonzero vectors are perpendicular exactly when their dot product is zero.

## 3. Detailed Step-by-Step Solution
Calculate the dot product:
$$u\cdot v=1\cdot2+2\cdot(-1)+(-1)\cdot3=2-2-3=-3.$$
Since this is not zero, $u$ and $v$ are not perpendicular.

For $w=(2,-1,a)$, impose the perpendicularity condition:
$$
\begin{aligned}
u\cdot w&=1\cdot2+2\cdot(-1)+(-1)\cdot a\\
&=2-2-a=-a.
\end{aligned}
$$
Set this equal to zero:
$$-a=0\quad\Longrightarrow\quad a=0.$$

## 4. Verification and Consistency Checks
With $a=0$, $w=(2,-1,0)$ and
$$u\cdot w=1\cdot2+2\cdot(-1)+(-1)\cdot0=0.$$
Thus the constructed vector is perpendicular to $u$.

## 5. Final Answer
$$\boxed{u\cdot v=-3\text{ (not perpendicular)},\qquad a=0.}$$