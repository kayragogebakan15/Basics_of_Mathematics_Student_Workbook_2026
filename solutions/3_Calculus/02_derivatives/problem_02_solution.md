# Exercise 2 — Powers, Roots, and the Domain

## 1. Problem Statement
For $f(x)=2\sqrt{x}-3/x^2+x^{3/2}$, rewrite it using powers, determine its domain, differentiate, and compare the domains of $f$ and $f'$.

## 2. Theoretical Background and Concepts
The square root requires $x\ge0$, and a denominator $x^2$ must be nonzero. For positive $x$ the power rule $(x^p)'=px^{p-1}$ applies to the fractional and negative powers in this problem. The derivative can only be defined where the original function is defined.

## 3. Detailed Step-by-Step Solution
Rewrite the expression as

$$
f(x)=2x^{1/2}-3x^{-2}+x^{3/2}.
$$

The simultaneous conditions $x\ge0$ and $x\ne0$ give the domain $(0,\infty)$. For every $x>0$, differentiation term by term gives

$$
\begin{aligned}
f'(x)
&=2\cdot\frac12x^{-1/2}-3(-2)x^{-3}+\frac32x^{1/2}\\
&=x^{-1/2}+6x^{-3}+\frac32x^{1/2}\\
&=\frac1{\sqrt x}+\frac6{x^3}+\frac32\sqrt x.
\end{aligned}
$$

Each derivative term exists at all positive $x$, so the derivative has the same domain $(0,\infty)$. The point $0$ is not in either domain; the square-root term alone being defined there cannot override the singular term $-3/x^2$.

## 4. Verification and Consistency Checks
For example, $f'(1)=1+6+3/2=17/2$. All three derivative terms are positive for $x>0$, confirming that the function is increasing on its domain. No singularities arise in the derivative for positive $x$.

## 5. Final Answer
$f(x)=2x^{1/2}-3x^{-2}+x^{3/2}$ and $f'(x)=x^{-1/2}+6x^{-3}+\frac32x^{1/2}$. Both domains are $(0,\infty)$.
