# Exercise 9 — A Logarithm and the Chain Rule

## 1. Problem Statement
For $f(x)=\ln(x^2+1)$, differentiate, determine the sign of $f'(x)$ on the negative and positive half-lines and at zero, and describe the qualitative behavior near zero.

## 2. Theoretical Background and Concepts
The logarithm derivative is $(\ln u(x))'=u'(x)/u(x)$ wherever $u(x)>0$. A positive derivative indicates increasing behavior and a negative derivative indicates decreasing behavior on an interval. The denominator's sign determines whether the derivative has the same sign as its numerator.

## 3. Detailed Step-by-Step Solution
The inner argument is $u(x)=x^2+1$, which is at least $1$ for all real $x$; the function is defined on $\mathbb R$. Differentiate the inner expression:

$$
u'(x)=2x.
$$

The chain rule gives

$$
f'(x)=\frac{u'(x)}{u(x)}=\frac{2x}{x^2+1}.
$$

Since $x^2+1>0$ for every $x$, the sign of $f'(x)$ is exactly the sign of $2x$:

| Interval or point | Sign of $f'(x)$ | Behavior |
|---|---|---|
| $x<0$ | Negative | Decreasing |
| $x=0$ | Zero | Horizontal tangent |
| $x>0$ | Positive | Increasing |

Therefore the graph falls toward the origin from the left and rises away from it on the right. The minimum is $f(0)=\ln1=0$.

## 4. Verification and Consistency Checks
The function is even: $f(-x)=\ln((-x)^2+1)=f(x)$. Its graph is symmetric about the $y$-axis, consistent with an odd derivative $2x/(x^2+1)$ and a stationary minimum at zero. Moreover, $x^2+1\ge1$ implies $\ln(x^2+1)\ge0$, with equality only at $x=0$, independently verifying the global minimum.

## 5. Final Answer
$f'(x)=2x/(x^2+1)$, negative for $x<0$, zero at $0$, and positive for $x>0$. The function has its minimum $0$ at the origin.
