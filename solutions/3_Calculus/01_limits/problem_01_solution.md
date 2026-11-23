# Exercise 1 — Dominant Terms in a Sequence

## 1. Problem Statement
Compute the limit of the sequence

$$
a_n=\frac{4n^2-3n+1}{2n^2+5n-7},\qquad n\to\infty.
$$

Explain why its highest-degree terms determine the limit.

## 2. Theoretical Background and Concepts
For a ratio of polynomials with the same highest degree, dividing the numerator and denominator by that highest power isolates the leading coefficients. Every term containing a positive power of $1/n$ tends to zero as $n$ grows. Limits of quotients may then be used when the denominator has a nonzero limit.

## 3. Detailed Step-by-Step Solution
Divide numerator and denominator by $n^2$ (valid for positive integers $n$):

$$
\frac{4n^2-3n+1}{2n^2+5n-7}
=\frac{4-\frac3n+\frac1{n^2}}{2+\frac5n-\frac7{n^2}}.
$$

As $n\to\infty$, both $1/n$ and $1/n^2$ approach zero. The denominator tends to $2\ne0$, so the quotient limit is

$$
\lim_{n\to\infty}a_n=\frac{4-0+0}{2+0-0}=\frac42=2.
$$

Equivalently, the leading terms $4n^2$ and $2n^2$ grow at the same quadratic rate, while all lower-degree terms become negligible relative to $n^2$.

## 4. Verification and Consistency Checks
Subtract the proposed limit algebraically:

$$
a_n-2=\frac{4n^2-3n+1-2(2n^2+5n-7)}{2n^2+5n-7}
=\frac{-13n+15}{2n^2+5n-7}.
$$

Dividing this difference by $n^2$ gives a numerator tending to zero and a denominator tending to $2$, independently confirming $a_n-2\to0$. The denominator vanishes at $n=1$, but the sequence is defined for all integers $n\ge2$; omitting a finite initial index does not affect its limit.

## 5. Final Answer
The sequence converges to $2$, the ratio of the leading coefficients $4/2$.
