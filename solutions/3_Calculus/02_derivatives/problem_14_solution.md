# Exercise 14 — Continuity and Differentiability of a Piecewise Function

## 1. Problem Statement
Investigate the function

$$
f(x)=\begin{cases}
x^2,&x\ge0,\\
ax,&x<0
\end{cases}
$$

at $x=0$. Find every $a$ for which it is continuous, calculate the one-sided derivatives, determine differentiability, and explain why continuity does not suffice.

## 2. Theoretical Background and Concepts
Continuity at $0$ means the left- and right-hand limits both equal $f(0)$. Differentiability at $0$ requires the one-sided difference quotients to have the same finite limit. Differentiability implies continuity, but the converse need not hold: branches may meet at a point with different slopes.

## 3. Detailed Step-by-Step Solution
Because the right branch includes zero,

$$
f(0)=0^2=0.
$$

For any fixed real parameter $a$, the left-hand limit and right-hand limit are

$$
\lim_{x\to0^-}ax=0,\qquad
\lim_{x\to0^+}x^2=0.
$$

Both equal $f(0)=0$, so **the function is continuous at $0$ for every real $a$**.

Next, use one-sided difference quotients, not just formulas valid away from the joining point. For $h<0$,

$$
\frac{f(0+h)-f(0)}h
=\frac{ah-0}{h}=a.
$$

Therefore the left derivative exists and equals $a$:

$$
f'_-(0)=\lim_{h\to0^-}a=a.
$$

For $h>0$,

$$
\frac{f(0+h)-f(0)}h=\frac{h^2}{h}=h,
$$

which gives

$$
f'_+(0)=\lim_{h\to0^+}h=0.
$$

Both one-sided derivatives exist for every real $a$, but they agree exactly when $a=0$. The ordinary two-sided derivative at zero therefore exists if and only if $a=0$, with $f'(0)=0$ in that case.

## 4. Verification and Consistency Checks
For $a=0$, the left branch is identically zero and the right branch is $x^2$; both one-sided slopes are zero, giving a horizontal tangent. For $a=1$, the function still joins continuously at $(0,0)$, but its left slope is $1$ while its right slope is $0$, so there is a corner and no two-sided derivative. This explicit counterexample demonstrates why continuity alone does not guarantee differentiability.

## 5. Final Answer
Continuous at $0$ for **all** real $a$. Both one-sided derivatives exist for every $a$, with $f'_-(0)=a$ and $f'_+(0)=0$; they agree, and $f$ is differentiable at $0$, **only when $a=0$**.
