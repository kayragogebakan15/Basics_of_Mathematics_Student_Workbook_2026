# Exercise 5 — The Classical Limit Leading to the Number e

## 1. Problem Statement
Evaluate $\lim_{n\to\infty}(1+1/n)^n$, calculate several values for increasing $n$, compare them with the limit, and explain why numerical data alone are not proof.

## 2. Theoretical Background and Concepts
The number $e$ is characterized by the classical sequence limit

$$
e=\lim_{n\to\infty}\left(1+\frac1n\right)^n.
$$

The expression is a standard exponential limit and may also be related to the natural logarithm by $\ln((1+1/n)^n)=n\ln(1+1/n)$. Numerical evaluations can suggest the limiting value but do not establish behavior for arbitrarily large $n$.

## 3. Detailed Step-by-Step Solution
Let $a_n=(1+1/n)^n$. Direct calculations give:

| $n$ | $a_n$ (approximately) |
|---|---:|
| $1$ | $2.000000$ |
| $2$ | $2.250000$ |
| $5$ | $2.488320$ |
| $10$ | $2.593742$ |
| $100$ | $2.704814$ |
| $1000$ | $2.716924$ |

The observed values move toward $e\approx2.718282$.

To connect this with an analytical argument, use the standard logarithm bounds, valid for all $u>0$:

$$
\frac{u}{1+u}\le\ln(1+u)\le u.
$$

Set $u=1/n$ and multiply by $n>0$:

$$
\frac{n}{n+1}\le n\ln\left(1+\frac1n\right)\le1.
$$

Both bounds tend to $1$, so the squeeze theorem yields

$$
\lim_{n\to\infty}n\ln\left(1+\frac1n\right)=1.
$$

Continuity of the exponential function then gives

$$
\lim_{n\to\infty}a_n
=\lim_{n\to\infty}\exp\left(n\ln\left(1+\frac1n\right)\right)
=\exp(1)=e.
$$

## 4. Verification and Consistency Checks
For example, $a_2=(1+1/2)^2=9/4=2.25$ and $a_5=(6/5)^5=7776/3125=2.48832$. The numerical values are consistent with convergence but finitely many samples cannot rule out unexpected behavior at larger indices; the logarithmic bounds apply to every positive integer and close this logical gap.

## 5. Final Answer
The limit is $e\approx2.718282$. The table illustrates convergence; the squeeze argument establishes it.
