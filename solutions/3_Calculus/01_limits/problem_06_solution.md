# Exercise 6 — From a Sequence to a Function: Limit at Infinity

## 1. Problem Statement
Compute the limit of $(3x^2-x+1)/(5x^2+4x-2)$ as the real variable $x$ tends to positive infinity. Compare the method with Exercise 1 and explain what changes and what remains the same.

## 2. Theoretical Background and Concepts
The quotient limit law applies when numerator and denominator have finite limits and the denominator's limit is nonzero. In rational expressions with equal polynomial degrees, dividing by the highest power identifies the ratio of leading coefficients. The same algebra works for sequences indexed by integers and functions with real inputs.

## 3. Detailed Step-by-Step Solution
For $x\ne0$, divide both polynomials by $x^2$:

$$
\frac{3x^2-x+1}{5x^2+4x-2}
=\frac{3-\frac1x+\frac1{x^2}}{5+\frac4x-\frac2{x^2}}.
$$

As $x\to+\infty$, both $1/x$ and $1/x^2$ approach zero; the denominator approaches $5\ne0$. Therefore

$$
\lim_{x\to+\infty}\frac{3x^2-x+1}{5x^2+4x-2}
=\frac{3-0+0}{5+0-0}=\frac35.
$$

Exercise 1 uses the same operation, dividing by the common highest degree $2$. The only difference is the domain: $n$ takes integer values increasing without bound, while $x$ passes through all sufficiently large real values. The leading-term argument is unchanged.

## 4. Verification and Consistency Checks
Subtract the candidate limit:

$$
\frac{3x^2-x+1}{5x^2+4x-2}-\frac35
=\frac{5(3x^2-x+1)-3(5x^2+4x-2)}{5(5x^2+4x-2)}
=\frac{-17x+11}{25x^2+20x-10}.
$$

The numerator grows linearly while the denominator grows quadratically, so this difference tends to zero. The original denominator is nonzero for sufficiently large $x$, which makes the calculation valid.

## 5. Final Answer
The function limit is $\frac35$; exactly the same dominant-degree technique applies as for the sequence in Exercise 1.
