# Exercise 9 — One-Sided Limits and an Asymptote

## 1. Problem Statement
Analyze the left-hand and right-hand limits of $f(x)=1/(x-2)$ at $x=2$, decide whether its two-sided limit exists, and explain the vertical asymptote with a qualitative sketch.

## 2. Theoretical Background and Concepts
A one-sided limit studies the function as $x$ approaches a point from only one direction. If the numerator remains positive and the denominator tends to zero through negative or positive values, the quotient diverges to negative or positive infinity, respectively. A finite two-sided limit requires both one-sided limits to agree. A line $x=a$ is a vertical asymptote if at least one one-sided function limit is infinite as $x\to a$.

## 3. Detailed Step-by-Step Solution
For $x<2$, the denominator $x-2$ is negative. As $x$ approaches $2$ from below, it approaches $0$ through negative values, so

$$
\lim_{x\to2^-}\frac1{x-2}=-\infty.
$$

For $x>2$, the denominator is positive and approaches zero through positive values, so

$$
\lim_{x\to2^+}\frac1{x-2}=+\infty.
$$

The left-hand and right-hand behaviors disagree. Thus no two-sided limit exists, even as a common infinite limit. Both sides become unbounded near $2$, so $x=2$ is a vertical asymptote.

Qualitative sketches of the two branches (not to scale). The dotted vertical line represents the asymptote $x=2$. Each branch slopes **downward as $x$ increases**.

~~~text
       Left of x=2                 Right of x=2

     y                                  y
     ^                                  ^
-----+--------:----> x                 |   : *-------- 
     |   ____ :                     ---+---:--\--------> x
     |  /     :                        |   :   \
     | /      :                        |   :    \___
     |/       :                        |
     |     \  :                        |
     |      \ :                        |
     |       \:                        |
             x=2                           x=2

As x increases toward 2 from the left, f(x) falls toward -infinity.
As x increases away from 2 on the right, f(x) falls from +infinity toward 0.
~~~

To make the direction of each branch unambiguous, compare representative values in order of increasing $x$:

| Left branch ($x<2$) | $f(x)$ | Right branch ($x>2$) | $f(x)$ |
|---:|---:|---:|---:|
| $1$ | $-1$ | $2.01$ | $100$ |
| $1.5$ | $-2$ | $2.1$ | $10$ |
| $1.9$ | $-10$ | $2.5$ | $2$ |
| $1.99$ | $-100$ | $3$ | $1$ |

For any two numbers $x_1<x_2$ on the same side of $2$, the difference satisfies

$$
f(x_2)-f(x_1)
=\frac1{x_2-2}-\frac1{x_1-2}
=\frac{x_1-x_2}{(x_2-2)(x_1-2)}<0.
$$

The numerator is negative, while the denominator is positive because both factors have the same sign on either side of $2$. Thus **both branches are strictly decreasing**. The right branch approaches $+\infty$ when traced *toward* $x=2$ from the right (that is, while $x$ decreases), which does not contradict its decreasing behavior when $x$ increases.

## 4. Verification and Consistency Checks
For $x=1.9$, $f(x)=1/(-0.1)=-10$; for $x=1.99$, $f(x)=-100$. From the right, $f(2.1)=10$ and $f(2.01)=100$. These values agree with the proven signs and unbounded behavior. The function is undefined at $2$, which is consistent with, but is not by itself proof of, the asymptote.

## 5. Final Answer
The left-hand limit is $-\infty$, the right-hand limit is $+\infty$, the two-sided limit does not exist, and the vertical asymptote is $x=2$.
