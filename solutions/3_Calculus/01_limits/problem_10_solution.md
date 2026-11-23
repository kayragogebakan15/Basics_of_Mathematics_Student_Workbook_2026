# Exercise 10 — Continuity of a Piecewise Function

## 1. Problem Statement
Determine $a$ so that the function with $f(x)=ax+1$ for $x<2$ and $f(x)=x^2-1$ for $x\ge2$ is continuous at $x=2$. Explicitly compare the left-hand limit, right-hand limit and function value.

## 2. Theoretical Background and Concepts
A function is continuous at $x=2$ exactly when its two one-sided limits exist, agree, and equal $f(2)$. The left-hand branch determines the limit from below; the right-hand branch determines the value at $2$ and the limit from above.

## 3. Detailed Step-by-Step Solution
From the branch for $x<2$:

$$
\lim_{x\to2^-}f(x)=\lim_{x\to2^-}(ax+1)=2a+1.
$$

From the branch for $x\ge2$:

$$
\lim_{x\to2^+}f(x)=\lim_{x\to2^+}(x^2-1)=2^2-1=3.
$$

Since the second branch includes $x=2$, it also gives

$$
f(2)=2^2-1=3.
$$

Set the left-hand limit equal to $3$:

$$
2a+1=3\quad\Longrightarrow\quad 2a=2\quad\Longrightarrow\quad a=1.
$$

## 4. Verification and Consistency Checks
With $a=1$, the left-hand expression is $x+1$, so its limit as $x\to2^-$ is $3$. The right-hand expression tends to $3$, and the value at $2$ is $3$. Therefore

$$
\lim_{x\to2^-}f(x)=\lim_{x\to2^+}f(x)=f(2)=3.
$$

If $a\ne1$, the left-hand limit differs from $3$, producing a jump or mismatch at the joining point.

## 5. Final Answer
The unique parameter making $f$ continuous at $x=2$ is $a=1$.
