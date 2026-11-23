# Exercise 4 — Powers and Oscillation

## 1. Problem Statement
Analyze the behavior as $n\to\infty$ of $(2/3)^n$, $(3/2)^n$, $(-1)^n$, and $(-1)^n/n$. Justify convergence or divergence in each case.

## 2. Theoretical Background and Concepts
A geometric sequence $q^n$ approaches zero for $|q|<1$, grows without bound for $q>1$, and oscillates for $q=-1$. A sequence may oscillate in sign yet still converge when the absolute values approach zero. The squeeze theorem says that if $-b_n\le a_n\le b_n$ and $b_n\to0$, then $a_n\to0$.

## 3. Detailed Step-by-Step Solution
**First sequence.** Because $0<2/3<1$, each multiplication reduces the positive term:

$$
\lim_{n\to\infty}\left(\frac23\right)^n=0.
$$

**Second sequence.** Since $3/2>1$, powers increase without any finite upper bound:

$$
\left(\frac32\right)^n\longrightarrow+\infty.
$$

**Third sequence.** Even and odd subsequences give different values:

$$
(-1)^{2k}=1,\qquad (-1)^{2k+1}=-1.
$$

Since their limits differ, the full sequence has no limit.

**Fourth sequence.** Its sign alternates, but its size decreases:

$$
-\frac1n\le\frac{(-1)^n}{n}\le\frac1n.
$$

Both outer sequences tend to $0$, so by the squeeze theorem

$$
\lim_{n\to\infty}\frac{(-1)^n}{n}=0.
$$

## 4. Verification and Consistency Checks
The third sequence cannot converge because a convergent sequence and all its subsequences must share the same limit, contradicted by $1$ and $-1$. For the fourth, $|(-1)^n/n|=1/n\to0$, which independently proves convergence in absolute difference from zero.

## 5. Final Answer
The behaviors are, respectively, convergence to $0$, divergence to $+\infty$, nonconvergent oscillation, and oscillatory convergence to $0$.
