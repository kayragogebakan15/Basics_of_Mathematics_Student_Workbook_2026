# Exercise 7 — Limit at a Point and Canceling a Factor

## 1. Problem Statement
Find the limit of $(x^2-4x+3)/(x-3)$ as $x\to3$. Explain why the expression's value at $x=3$ is unnecessary.

## 2. Theoretical Background and Concepts
A limit depends on function values arbitrarily close to the point, not necessarily at the point itself. When substitution produces the indeterminate pattern $0/0$, factorization may cancel a common factor for every nearby point where the original expression is defined.

## 3. Detailed Step-by-Step Solution
Factor the quadratic by finding two numbers whose sum is $-4$ and product is $3$:

$$
x^2-4x+3=(x-1)(x-3).
$$

For $x\ne3$, cancel the common factor:

$$
\frac{x^2-4x+3}{x-3}
=\frac{(x-1)(x-3)}{x-3}=x-1.
$$

The simplified function is continuous at $x=3$, hence

$$
\lim_{x\to3}\frac{x^2-4x+3}{x-3}
=\lim_{x\to3}(x-1)=3-1=2.
$$

## 4. Verification and Consistency Checks
From the left, $x=2.9$ gives $x-1=1.9$; from the right, $x=3.1$ gives $2.1$. Both approach $2$. Although the original quotient is undefined exactly at $x=3$ because its denominator is zero, it agrees with $x-1$ on the punctured neighborhood of $3$; that agreement suffices to determine the limit.

## 5. Final Answer
The two-sided limit equals $2$, even though the original function is not defined at $x=3$.
