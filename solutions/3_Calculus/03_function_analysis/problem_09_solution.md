# Exercise 9 — An Oblique Asymptote

## 1. Problem Statement
Analyze the asymptotes of $f(x)=(x^2+1)/(x-1)$ using polynomial division, and explain why the remainder vanishes when $|x|$ is large.

## 2. Theoretical Background and Concepts
A vertical asymptote occurs at a nonremovable zero of the denominator. A line $y=mx+b$ is an oblique asymptote when $f(x)-(mx+b)\to0$ at infinity. Polynomial division separates a rational function into its polynomial quotient and a remainder fraction.

## 3. Detailed Step-by-Step Solution
The domain excludes $x=1$. Divide the numerator by $x-1$:

$$
(x-1)(x+1)=x^2-1,
$$

so

$$
x^2+1=(x-1)(x+1)+2.
$$

For $x\ne1$,

$$
f(x)=x+1+\frac2{x-1}.
$$

As $x\to1^-$, $2/(x-1)\to-\infty$; as $x\to1^+$ it tends to $+\infty$. Hence $x=1$ is a vertical asymptote. The numerator at $1$ is $2\ne0$, so it cannot cancel the pole.

As $x\to+\infty$ or $x\to-\infty$,

$$
f(x)-(x+1)=\frac2{x-1}\longrightarrow0.
$$

Thus $y=x+1$ is the oblique asymptote at both ends. The remainder tends to zero because the numerator is the fixed constant $2$ while the denominator's absolute value grows without bound. There is no horizontal asymptote because $f(x)$ behaves like the unbounded line $x+1$ at infinity.

## 4. Verification and Consistency Checks
At $x=3$, $f(3)=(9+1)/2=5$ and $x+1+2/(x-1)=4+1=5$. At $x=-1$, $f(-1)=2/(-2)=-1$ and $x+1+2/(x-1)=0-1=-1$. These verify the decomposition on both sides of the pole. Since $2/(x-1)$ is positive for $x>1$ and negative for $x<1$, the graph lies respectively above and below its oblique asymptote.

## 5. Final Answer
Vertical asymptote $x=1$; oblique asymptote $y=x+1$ for $x\to\pm\infty$; no horizontal asymptote.
