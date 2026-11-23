# Exercise 8 — A Square Root in a Function Limit

## 1. Problem Statement
Compute $\lim_{x\to4}(\sqrt{x}-2)/(x-4)$ by rationalizing the numerator, and compare the method with the sequence limit of Exercise 3.

## 2. Theoretical Background and Concepts
Direct substitution gives $0/0$, an indeterminate form. Multiplication by the conjugate $\sqrt{x}+2$ uses $(a-b)(a+b)=a^2-b^2$ to expose a cancelable factor. An algebraically equivalent expression for $x\ne4$ has the same limit at $4$.

## 3. Detailed Step-by-Step Solution
For $x\ge0$ and $x\ne4$, multiply by the conjugate divided by itself:

$$
\frac{\sqrt{x}-2}{x-4}
=\frac{(\sqrt{x}-2)(\sqrt{x}+2)}{(x-4)(\sqrt{x}+2)}.
$$

Simplify the numerator:

$$
=\frac{x-4}{(x-4)(\sqrt{x}+2)}
=\frac1{\sqrt{x}+2}.
$$

Now continuity of the square root and the quotient law give

$$
\lim_{x\to4}\frac{\sqrt{x}-2}{x-4}
=\frac1{\sqrt4+2}=\frac14.
$$

In Exercise 3 the conjugate changed an $\infty-\infty$ difference into a quotient. Here it cancels a $0/0$ factor. Both transformations use the difference-of-squares identity.

## 4. Verification and Consistency Checks
At $x=9$, the original quotient is $(3-2)/(9-4)=1/5$, and the transformed expression gives $1/(3+2)=1/5$. More importantly, the expressions coincide for every $x\ge0$, $x\ne4$, so the limit is unchanged. The new denominator tends to $4\ne0$, legitimizing direct substitution.

## 5. Final Answer
The limit is $\frac14$.
