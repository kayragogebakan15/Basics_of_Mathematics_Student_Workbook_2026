# Exercise 5 — The Chain Rule as Working Through Layers

## 1. Problem Statement
For $f(x)=(3x^2-2x+1)^5$, identify inner and outer functions, differentiate them, apply the chain rule and explain the extra factor.

## 2. Theoretical Background and Concepts
For a composition $f(x)=g(u(x))$, the chain rule says $f'(x)=g'(u(x))u'(x)$. The outer expression changes in response to the inner expression, which itself changes with $x$.

## 3. Detailed Step-by-Step Solution
Use the inner function $u(x)=3x^2-2x+1$ and outer function $g(u)=u^5$. Their derivatives are

$$
u'(x)=6x-2,\qquad g'(u)=5u^4.
$$

Apply the chain rule:

$$
\begin{aligned}
f'(x)&=5(u(x))^4u'(x)\\
&=5(3x^2-2x+1)^4(6x-2)\\
&=10(3x-1)(3x^2-2x+1)^4.
\end{aligned}
$$

The extra factor $6x-2$ comes from differentiating the inner quadratic. Omitting it would treat the inner expression as though it increased at the same rate as $x$.

## 4. Verification and Consistency Checks
At $x=0$, the formula gives $5(1)^4(-2)=-10$. Expanding just the linear part near zero, $(1-2x+3x^2)^5=1-10x+\cdots$, confirms the slope $-10$. At $x=1/3$, the inner quadratic has a stationary point because $6x-2=0$, so the composite derivative also vanishes.

## 5. Final Answer
$f'(x)=5(3x^2-2x+1)^4(6x-2)$, equivalently $10(3x-1)(3x^2-2x+1)^4$.
