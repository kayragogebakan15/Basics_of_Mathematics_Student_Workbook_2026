# Exercise 14 — A 0/0 Limit with Trigonometry

## 1. Problem Statement
Compute the limit of $(1-\cos x)/x^2$ as $x\to0$ without using l'Hôpital's rule. Justify the result with a trigonometric identity and the fundamental limit $\lim_{u\to0}\sin u/u=1$.

## 2. Theoretical Background and Concepts
The half-angle identity follows from the double-angle identity for cosine:

$$
1-\cos x=2\sin^2\left(\frac x2\right).
$$

For angles measured in radians, the fundamental trigonometric limit states that $\sin u/u\to1$ as $u\to0$. The square of an expression converging to $1$ also converges to $1$.

## 3. Detailed Step-by-Step Solution
Direct substitution yields $0/0$, so rewrite the numerator. For every nonzero $x$,

$$
\frac{1-\cos x}{x^2}
=\frac{2\sin^2(x/2)}{x^2}.
$$

Because $x=2(x/2)$, we have $x^2=4(x/2)^2$. Therefore

$$
\frac{2\sin^2(x/2)}{x^2}
=\frac{2\sin^2(x/2)}{4(x/2)^2}
=\frac12\left(\frac{\sin(x/2)}{x/2}\right)^2.
$$

Let $u=x/2$. Since $u\to0$ as $x\to0$, apply the fundamental limit:

$$
\lim_{x\to0}\frac{1-\cos x}{x^2}
=\frac12\left(\lim_{u\to0}\frac{\sin u}{u}\right)^2
=\frac12\cdot1^2=\frac12.
$$

The factor $1/2$ arises from the factor $4$ in the squared denominator; it is not $2$.

## 4. Verification and Consistency Checks
An independent check rationalizes the numerator, using $(1-\cos x)(1+\cos x)=\sin^2x$:

$$
\frac{1-\cos x}{x^2}
=\frac{\sin^2x}{x^2(1+\cos x)}
=\frac1{1+\cos x}\left(\frac{\sin x}{x}\right)^2.
$$

For nonzero $x$ sufficiently near $0$, $1+\cos x\ne0$. Its limit is $2$, while the squared sine quotient tends to $1$, so the independent expression tends to $1/2$. Both the original quotient and its transformed versions are even in $x$, consistent with the same limit from either side.

## 5. Final Answer
The two-sided limit is $\frac12$, established without derivatives.
