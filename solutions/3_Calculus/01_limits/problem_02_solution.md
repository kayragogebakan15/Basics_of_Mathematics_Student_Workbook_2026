# Exercise 2 — Different Growth Rates

## 1. Problem Statement
Compute the limits of $(3n+1)/(n^2+4)$ and $(2n^3-n)/(5n^2+1)$ as $n\to\infty$. Compare the results and explain what the polynomial degrees imply.

## 2. Theoretical Background and Concepts
For polynomial quotients at positive infinity, divide by the denominator's highest power or factor out leading powers. When numerator degree is lower, the quotient tends to zero; when degrees match, it tends to the ratio of leading coefficients. When the numerator degree is higher, the magnitude grows without bound, with the sign determined by the leading terms.

## 3. Detailed Step-by-Step Solution
**First sequence.** Divide by $n^2$:

$$
\frac{3n+1}{n^2+4}
=\frac{\frac3n+\frac1{n^2}}{1+\frac4{n^2}}
\longrightarrow\frac{0}{1}=0.
$$

**Second sequence.** Factor out the excess power of $n$:

$$
\frac{2n^3-n}{5n^2+1}
=n\frac{2-\frac1{n^2}}{5+\frac1{n^2}}.
$$

The fraction on the right tends to $2/5>0$. Because $n\to+\infty$, the whole product tends to $+\infty$ (it has no finite real limit).

The first numerator has degree $1<2$, so its denominator grows faster. The second numerator has degree $3>2$, so its numerator dominates by one power of $n$.

## 4. Verification and Consistency Checks
For the first expression, the rewritten numerator tends to $0$ and its denominator to $1$, giving a valid quotient limit. For the second, the factor $(2-1/n^2)/(5+1/n^2)$ is eventually larger than, for instance, $1/5>0$; consequently the original expression eventually exceeds $n/5$, which grows without bound. This justifies the infinite limit, not merely the intuition about polynomial degrees.

## 5. Final Answer
The first limit is $0$. The second expression diverges to $+\infty$. Lower numerator degree yields $0$; equal degrees give a leading-coefficient ratio; a higher numerator degree produces unbounded magnitude in the nondegenerate polynomial case.
