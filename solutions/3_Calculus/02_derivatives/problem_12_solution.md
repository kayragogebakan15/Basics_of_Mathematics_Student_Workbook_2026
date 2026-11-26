# Exercise 12 — Several Rules at Once

## 1. Problem Statement
Differentiate $f(x)=(x^2+1)^3e^x$. State which rule applies to the whole expression, which applies inside its first factor, and factor the final derivative.

## 2. Theoretical Background and Concepts
The outermost structure is a product $u(x)v(x)$, so $(uv)'=u'v+uv'$. The first factor is a composition, requiring the chain rule $(g\circ w)'(x)=g'(w(x))w'(x)$. After differentiating, factoring common expressions makes the result easier to read and verify.

## 3. Detailed Step-by-Step Solution
Plan: apply the product rule to $u=(x^2+1)^3$ and $v=e^x$. Apply the chain rule to $u$ using the inner polynomial $w=x^2+1$ and outer cube $g(w)=w^3$.

First,

$$
w'(x)=2x,\qquad
u'(x)=3(x^2+1)^2(2x)=6x(x^2+1)^2.
$$

Also $v'(x)=e^x$. Now use the product rule:

$$
\begin{aligned}
f'(x)
&=u'v+uv'\\
&=6x(x^2+1)^2e^x+(x^2+1)^3e^x\\
&=e^x(x^2+1)^2\left(6x+(x^2+1)\right)\\
&=e^x(x^2+1)^2(x^2+6x+1).
\end{aligned}
$$

The factor $6x$ comes from multiplying the cube's outer derivative $3(x^2+1)^2$ by the quadratic's inner derivative $2x$.

## 4. Verification and Consistency Checks
At $x=0$, the factored formula yields $f'(0)=1\cdot1\cdot1=1$. Directly from the product rule, $u(0)=1$, $u'(0)=0$, $v(0)=1$, and $v'(0)=1$, so $f'(0)=0\cdot1+1\cdot1=1$. Expanding the factored bracket restores both product-rule terms, verifying the algebra.

## 5. Final Answer
$f'(x)=e^x(x^2+1)^2(x^2+6x+1)$ for every real $x$.
