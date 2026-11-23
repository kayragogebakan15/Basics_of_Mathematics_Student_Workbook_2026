# Exercise 3 — A Square Root and Removing an Indeterminate Form

## 1. Problem Statement
Compute the limit of $\sqrt{n^2+5n}-n$ as $n\to\infty$, using a conjugate, and explain why this avoids the indeterminate form.

## 2. Theoretical Background and Concepts
Subtracting two positive expressions that both grow without bound gives the indeterminate pattern $\infty-\infty$. Multiplying by the conjugate uses the identity $(a-b)(a+b)=a^2-b^2$, converting the difference into a quotient where the dominant terms can be compared safely.

## 3. Detailed Step-by-Step Solution
Multiply the expression by its positive conjugate divided by itself:

$$
\sqrt{n^2+5n}-n
=\frac{(\sqrt{n^2+5n}-n)(\sqrt{n^2+5n}+n)}
{\sqrt{n^2+5n}+n}.
$$

Use the difference of squares in the numerator:

$$
=\frac{(n^2+5n)-n^2}{\sqrt{n^2+5n}+n}
=\frac{5n}{\sqrt{n^2+5n}+n}.
$$

For $n>0$, factor $n$ from the square root: $\sqrt{n^2+5n}=n\sqrt{1+5/n}$. Cancel $n$:

$$
=\frac5{\sqrt{1+\frac5n}+1}
\longrightarrow\frac5{1+1}=\frac52.
$$

## 4. Verification and Consistency Checks
Every transformation is an exact equality for positive integers $n$; the conjugate denominator is strictly positive. The transformed expression has a denominator tending to $2$, not zero, so the quotient-limit rule applies. It is positive and less than $5/2$ for finite positive $n$, consistent with approaching $5/2$ from below.

## 5. Final Answer
The limit is $\frac52$.
