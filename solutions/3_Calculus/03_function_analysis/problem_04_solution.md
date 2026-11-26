# Exercise 4 — A Function with Two Vertical Asymptotes

## 1. Problem Statement
Analyze $f(x)=1/(x^2-1)$: determine its domain, asymptotes, sign and monotonicity on each domain interval, and explain why the intervals must be separated.

## 2. Theoretical Background and Concepts
A rational expression excludes roots of its denominator. Sign changes across excluded points can alter both the sign of the function and its limiting behavior. Derivative sign can be used to infer monotonicity only on intervals contained in the domain; it cannot be carried across a pole.

## 3. Detailed Step-by-Step Solution
Factor the denominator:

$$
x^2-1=(x-1)(x+1).
$$

The domain is $\mathbb R\setminus\{-1,1\}$. Since the numerator stays $1$, both excluded points are genuine vertical asymptotes. Signs of the factors give

$$
\begin{aligned}
\lim_{x\to-1^-}f(x)&=+\infty,&
\lim_{x\to-1^+}f(x)&=-\infty,\\
\lim_{x\to1^-}f(x)&=-\infty,&
\lim_{x\to1^+}f(x)&=+\infty.
\end{aligned}
$$

As $x\to\pm\infty$, $1/(x^2-1)\to0^+$, so $y=0$ is a horizontal asymptote. Because $x^2-1>0$ for $|x|>1$ and $x^2-1<0$ for $|x|<1$, the function is positive outside $[-1,1]$ and negative between the poles. There are no zeros.

Differentiate:

$$
f'(x)=-(x^2-1)^{-2}(2x)
=-\frac{2x}{(x^2-1)^2}.
$$

The denominator is positive wherever the function is defined. Hence $f'>0$ for $x<0$, $f'(0)=0$, and $f'<0$ for $x>0$. Combine this with domain breaks:

| Interval | Sign of $f$ | Sign of $f'$ | Behavior |
|---|---|---|---|
| $(-\infty,-1)$ | Positive | Positive | Increasing |
| $(-1,0)$ | Negative | Positive | Increasing |
| $(0,1)$ | Negative | Negative | Decreasing |
| $(1,\infty)$ | Positive | Negative | Decreasing |

The central branch reaches a local maximum $f(0)=1/(-1)=-1$ and goes to $-\infty$ at both of its vertical boundaries. The exterior branches are positive and approach zero as $|x|\to\infty$, while rising to $+\infty$ near their respective poles.

## 4. Verification and Consistency Checks
Representative values are $f(-2)=1/3>0$, $f(0)=-1$, and $f(2)=1/3>0$. Derivative values $f'(-2)=4/9>0$ and $f'(2)=-4/9<0$ confirm exterior branch directions. Because $f(-x)=f(x)$, the graph is symmetric about the $y$-axis, consistent with the symmetric poles and the derivative's odd sign pattern. Monotonicity is not asserted across $x=-1$ or $x=1$, where the function is undefined.

## 5. Final Answer
Domain $\mathbb R\setminus\{-1,1\}$; vertical asymptotes $x=-1$ and $x=1$; horizontal asymptote $y=0$; positive for $|x|>1$, negative for $|x|<1$. Increasing on $(-\infty,-1)$ and $(-1,0)$, decreasing on $(0,1)$ and $(1,\infty)$; local maximum $(0,-1)$.
