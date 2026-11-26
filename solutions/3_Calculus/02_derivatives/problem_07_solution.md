# Exercise 7 — A Trigonometric Composition

## 1. Problem Statement
For $f(x)=\sin(x^2+1)$, compute $f'(x)$, identify the inner and outer functions and the derivative of the inner one, and determine the sign of $f'(0)$.

## 2. Theoretical Background and Concepts
A composition is differentiated with $(g\circ u)'(x)=g'(u(x))u'(x)$. For the outer sine function, $g'(u)=\cos u$. A zero derivative has sign zero, which is distinct from a positive or negative derivative.

## 3. Detailed Step-by-Step Solution
Choose

$$
u(x)=x^2+1,\qquad g(u)=\sin u.
$$

Then

$$
u'(x)=2x,\qquad g'(u)=\cos u.
$$

By the chain rule,

$$
\begin{aligned}
f'(x)&=g'(u(x))u'(x)\\
&=\cos(x^2+1)\cdot2x\\
&=2x\cos(x^2+1).
\end{aligned}
$$

At $x=0$,

$$
f'(0)=2(0)\cos(1)=0.
$$

Its sign is **zero**, neither positive nor negative, and the tangent is horizontal there.

## 4. Verification and Consistency Checks
The sine function is even around an inner argument depending on $x^2$: $f(-x)=\sin((-x)^2+1)=f(x)$. Any differentiable even function has derivative zero at the origin; indeed the difference quotients from opposite sides have opposite signs and a common limit only if it is zero. This agrees with the chain-rule result. The point is $(0,\sin1)$.

## 5. Final Answer
$f'(x)=2x\cos(x^2+1)$ and $f'(0)=0$.
