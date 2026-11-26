# Exercise 1 — Derivative of a Polynomial and the Slope of a Tangent Line

## 1. Problem Statement
For $f(x)=3x^5-2x^3+7x-4$, find $f'(x)$ and calculate $f'(0)$ and $f'(1)$. Determine their signs and interpret the tangent slopes at these points.

## 2. Theoretical Background and Concepts
Differentiation is linear: the derivative of a sum is the sum of derivatives, and constant coefficients remain as factors. The power rule is $(x^m)'=mx^{m-1}$ for nonnegative integer exponents, while the derivative of a constant is zero. At a point $x=a$, the derivative $f'(a)$ is the slope of the tangent to the graph: positive slope means the tangent rises from left to right, negative slope means it falls, and zero slope means it is horizontal.

## 3. Detailed Step-by-Step Solution
Apply the rules term by term:

$$
\begin{aligned}
f'(x)
&=3(5x^4)-2(3x^2)+7(1)-0\\
&=15x^4-6x^2+7.
\end{aligned}
$$

At $x=0$:

$$
f'(0)=15(0)^4-6(0)^2+7=7>0.
$$

At $x=1$:

$$
f'(1)=15(1)^4-6(1)^2+7=15-6+7=16>0.
$$

Thus both tangents rise as $x$ increases. The tangent is steeper at $x=1$ (slope $16$) than at $x=0$ (slope $7$).

## 4. Verification and Consistency Checks
The function values are $f(0)=-4$ and $f(1)=3-2+7-4=4$. The corresponding tangent lines can be checked with the point-slope formula: at $x=0$, $y+4=7x$; at $x=1$, $y-4=16(x-1)$. Each line passes through the correct graph point and has the slope predicted by its derivative.

## 5. Final Answer
$f'(x)=15x^4-6x^2+7$, $f'(0)=7>0$, and $f'(1)=16>0$. Both tangent lines rise, with the latter steeper.
