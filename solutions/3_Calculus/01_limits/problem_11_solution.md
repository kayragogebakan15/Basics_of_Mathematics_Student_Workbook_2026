# Exercise 11 — An n-th Root

## 1. Problem Statement
Compute the limit of the sequence $\sqrt[n]{5^n+2^n}$ as $n\to\infty$. Explain why the larger exponential term dominates and why the transformation differs from a quotient of polynomials.

## 2. Theoretical Background and Concepts
For positive numbers $a>b$, the exponential ratio $(b/a)^n$ tends to zero. Factoring out the larger exponential $a^n$ yields an expression with an $n$-th root. If $1\le b_n\le M$ for some fixed $M>0$, then $1\le b_n^{1/n}\le M^{1/n}\to1$, so the squeeze theorem applies.

## 3. Detailed Step-by-Step Solution
The term $5^n$ grows faster than $2^n$, because their ratio is

$$
\frac{2^n}{5^n}=\left(\frac25\right)^n\longrightarrow0.
$$

Factor $5^n$ from the radicand:

$$
\begin{aligned}
\sqrt[n]{5^n+2^n}
&=\sqrt[n]{5^n\left(1+\left(\frac25\right)^n\right)}\\
&=5\left(1+\left(\frac25\right)^n\right)^{1/n}.
\end{aligned}
$$

Since $0<(2/5)^n\le1$ for every positive integer $n$,

$$
1\le\left(1+\left(\frac25\right)^n\right)^{1/n}\le2^{1/n}.
$$

The outer expressions both tend to $1$, because $2^{1/n}=\exp((\ln2)/n)\to1$. By the squeeze theorem the middle factor also tends to $1$. Therefore

$$
\lim_{n\to\infty}\sqrt[n]{5^n+2^n}=5\cdot1=5.
$$

Unlike a polynomial quotient, the natural operation here is to factor the dominant exponential and then control the variable exponent $1/n$; dividing by a polynomial power would not isolate the dominant terms.

## 4. Verification and Consistency Checks
The original terms satisfy the direct bounds

$$
5^n\le5^n+2^n\le2\cdot5^n.
$$

Taking positive $n$-th roots gives $5\le\sqrt[n]{5^n+2^n}\le5\cdot2^{1/n}$, another immediate squeeze to $5$. For $n=1$ the term is $7$, and for $n=2$ it is $\sqrt{29}\approx5.385$, both above the limit, consistent with the bound.

## 5. Final Answer
The sequence converges to $5$, determined by the faster-growing exponential $5^n$.
