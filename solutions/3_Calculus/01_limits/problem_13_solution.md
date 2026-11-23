# Exercise 13 — Fundamental Trigonometric Limit

## 1. Problem Statement
Using the standard limit $\lim_{u\to0}\sin u/u=1$, compute $\lim_{x\to0}\sin(5x)/x$ and $\lim_{x\to0}\sin(2x)/\sin(3x)$. Show the reduction to the fundamental limit in both cases.

## 2. Theoretical Background and Concepts
For angles measured in radians,

$$
\lim_{u\to0}\frac{\sin u}{u}=1.
$$

Replacing $u$ by $kx$ for any nonzero constant $k$ preserves $u\to0$ as $x\to0$. Multiplying and dividing by the matching argument of the sine therefore converts more complex quotients into the standard sine limit. A reciprocal can be taken when the corresponding limit is nonzero.

## 3. Detailed Step-by-Step Solution
**First limit.** For nonzero $x$,

$$
\frac{\sin(5x)}x
=5\frac{\sin(5x)}{5x}.
$$

With $u=5x\to0$,

$$
\lim_{x\to0}\frac{\sin(5x)}x
=5\lim_{u\to0}\frac{\sin u}{u}
=5.
$$

**Second limit.** For nonzero $x$ sufficiently close to zero, $\sin(3x)\ne0$. Multiply and divide by $2x$ and $3x$:

$$
\frac{\sin(2x)}{\sin(3x)}
=\frac{\sin(2x)}{2x}\cdot\frac{3x}{\sin(3x)}\cdot\frac23.
$$

As $x\to0$, the first factor tends to $1$. The ratio $\sin(3x)/(3x)$ tends to $1\ne0$, so its reciprocal $3x/\sin(3x)$ also tends to $1$. Hence

$$
\lim_{x\to0}\frac{\sin(2x)}{\sin(3x)}
=1\cdot1\cdot\frac23=\frac23.
$$

## 4. Verification and Consistency Checks
For the first quotient, dividing it by $5$ leaves exactly $\sin(5x)/(5x)\to1$. For the second, the argument-matched factors show that the only surviving constant is $2/3$. Both are two-sided limits: $\sin(kx)/(kx)$ has the same limit for positive and negative $x$. No step replaces $\sin(kx)$ with $kx$ as an exact equality; only the ratio's limit is used.

## 5. Final Answer
The limits are $5$ and $\frac23$, respectively.
