# Exercise 12 — Exponential Function Limit

## 1. Problem Statement
Compute $\lim_{x\to0}(1+3x)^{1/x}$, relate it to the classical limit producing $e$ from Exercise 5, and show the transformation.

## 2. Theoretical Background and Concepts
The standard real-variable exponential limit is

$$
\lim_{u\to0}(1+u)^{1/u}=e,
$$

where $1+u>0$. It is the continuous-variable counterpart of the sequence limit $(1+1/n)^n\to e$. A change of variable and the power rule let us recognize this pattern. The logarithmic approach gives an independent check through $\ln(1+u)/u\to1$.

## 3. Detailed Step-by-Step Solution
For $x$ sufficiently close to zero, $1+3x>0$, so the real power is defined. Put $u=3x$, which gives $u\to0$ as $x\to0$ and $1/x=3/u$. Thus

$$
(1+3x)^{1/x}=(1+u)^{3/u}
=\left((1+u)^{1/u}\right)^3.
$$

Apply the classical limit and the continuity of cubing:

$$
\lim_{x\to0}(1+3x)^{1/x}
=\left(\lim_{u\to0}(1+u)^{1/u}\right)^3
=e^3.
$$

The coefficient $3$ in $3x$ is essential: it changes the exponent $1/x$ into $3/u$, so the limit is $e^3$, not $e$.

## 4. Verification and Consistency Checks
Taking a natural logarithm of the original positive expression yields

$$
\ln\left((1+3x)^{1/x}\right)
=\frac{\ln(1+3x)}x
=3\frac{\ln(1+3x)}{3x}.
$$

Because $\lim_{u\to0}\ln(1+u)/u=1$, the logarithm tends to $3$. Exponentiating gives the same limit $e^3$. The limit is two-sided: the base is positive on a sufficiently small interval around zero, and the transformed standard limit applies from both sides.

## 5. Final Answer
The limit is $e^3\approx20.085537$.
