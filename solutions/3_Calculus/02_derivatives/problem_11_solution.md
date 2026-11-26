# Exercise 11 — Derivative from the Definition

## 1. Problem Statement
Using only the definition $f'(x)=\lim_{h\to0}(f(x+h)-f(x))/h$, find the derivative of $f(x)=x^2$. Compare it with the power rule and identify where the limit is used.

## 2. Theoretical Background and Concepts
The derivative at a point is the limit of the difference quotient as the increment $h$ tends to zero. For $h\ne0$, a common factor of $h$ may be canceled before taking the limit. Direct substitution into the original quotient at $h=0$ would be invalid because its denominator would vanish.

## 3. Detailed Step-by-Step Solution
Fix an arbitrary real number $x$. Evaluate the shifted function:

$$
f(x+h)=(x+h)^2=x^2+2xh+h^2.
$$

Subtract $f(x)=x^2$:

$$
f(x+h)-f(x)=x^2+2xh+h^2-x^2=2xh+h^2.
$$

For $h\ne0$, factor and cancel $h$:

$$
\frac{f(x+h)-f(x)}h=\frac{2xh+h^2}h=2x+h.
$$

Only now take the limit as $h$ approaches zero:

$$
f'(x)=\lim_{h\to0}(2x+h)=2x.
$$

This is the point where the limit is essential: the slopes of nearby secant lines approach the single tangent slope $2x$.

## 4. Verification and Consistency Checks
The power rule independently predicts $(x^2)'=2x^{2-1}=2x$, in agreement with the definition. At $x=3$, the difference quotient is $6+h$ and tends to $6$ from both positive and negative $h$. The cancellation is restricted to $h\ne0$, exactly as required by the deleted-neighborhood definition of the derivative.

## 5. Final Answer
$f'(x)=2x$ for every real $x$, derived directly from the difference-quotient limit.
