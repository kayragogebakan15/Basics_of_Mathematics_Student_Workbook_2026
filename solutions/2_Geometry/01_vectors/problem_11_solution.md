# Exercise 11 — Decomposition into Parallel and Perpendicular Components

## 1. Problem Statement
Decompose $u=(3,4)$ into components parallel and perpendicular to $v=(1,2)$. Check
$$u=u_{\parallel}+u_{\perp},\qquad u_{\perp}\cdot v=0.$$
Explain why these are two independent checks of correctness.

## 2. Method and Key Formula
The parallel component is the projection:
$$u_{\parallel}=\operatorname{proj}_v u=\frac{u\cdot v}{v\cdot v}v.$$
The perpendicular component is the remainder:
$$u_{\perp}=u-u_{\parallel}.$$

## 3. Detailed Step-by-Step Solution
Calculate
$$u\cdot v=3\cdot1+4\cdot2=11,\qquad v\cdot v=1^2+2^2=5.$$
Therefore,
$$
u_{\parallel}=\frac{11}{5}(1,2)=\left(\frac{11}{5},\frac{22}{5}\right).
$$
Subtract from $u$:
$$
\begin{aligned}
u_{\perp}
&=(3,4)-\left(\frac{11}{5},\frac{22}{5}\right)\\
&=\left(\frac{15-11}{5},\frac{20-22}{5}\right)
=\left(\frac45,-\frac25\right).
\end{aligned}
$$

## 4. Verification and Consistency Checks
First check reconstruction:
$$
u_{\parallel}+u_{\perp}
=\left(\frac{11+4}{5},\frac{22-2}{5}\right)
=(3,4)=u.
$$
Then check perpendicularity:
$$
u_{\perp}\cdot v
=\frac45\cdot1+\left(-\frac25\right)\cdot2
=\frac45-\frac45=0.
$$
These checks are independent: reconstruction confirms that the two components add to the original vector, while the dot product confirms that the remainder is perpendicular to the specified direction. One condition alone does not guarantee the other.

## 5. Final Answer
$$\boxed{
u_{\parallel}=\left(\frac{11}{5},\frac{22}{5}\right),\qquad
u_{\perp}=\left(\frac45,-\frac25\right).
}$$