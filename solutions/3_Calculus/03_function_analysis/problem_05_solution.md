# Exercise 5 — An Exponential Function with a Maximum

## 1. Problem Statement
Analyze monotonicity and extrema of $f(x)=xe^{-x}$. Determine the behavior as $x\to+\infty$ and explain the shape of the right-hand graph.

## 2. Theoretical Background and Concepts
The product rule gives $(uv)'=u'v+uv'$, and $(e^{-x})'=-e^{-x}$. The exponential factor is always positive, so derivative sign is controlled by the remaining factor. For large positive $x$, the exponential $e^x$ eventually dominates the linear factor $x$.

## 3. Detailed Step-by-Step Solution
The domain is all real numbers. Differentiate:

$$
\begin{aligned}
f'(x)&=1\cdot e^{-x}+x(-e^{-x})\\
&=e^{-x}(1-x).
\end{aligned}
$$

Since $e^{-x}>0$, $f'>0$ for $x<1$, $f'(1)=0$ and $f'<0$ for $x>1$. Thus the function increases on $(-\infty,1)$ and decreases on $(1,\infty)$. The sign switches from positive to negative at $x=1$, giving a maximum

$$
f(1)=e^{-1}=\frac1e.
$$

The limit at the right end of the domain is

$$
\lim_{x\to+\infty}xe^{-x}
=\lim_{x\to+\infty}\frac{x}{e^x}=0.
$$

For justification, l'Hôpital's rule applies to the $\infty/\infty$ quotient and yields $\lim 1/e^x=0$. Thus the graph descends after its maximum but remains positive, approaching the horizontal asymptote $y=0$ from above.

For completeness, if $x=-t$ and $t\to+\infty$, then $xe^{-x}=-te^t\to-\infty$. Also $f(0)=0$, so the graph crosses the origin, rises to $(1,1/e)$, then gently decreases toward $0^+$.

## 4. Verification and Consistency Checks
Test $f'(0)=1>0$ and $f'(2)=e^{-2}(1-2)=-e^{-2}<0$. Both confirm the claimed monotonicity. The function tends to $-\infty$ on the far left and to $0^+$ on the right, so the maximum at $(1,1/e)$ is global, not merely local.

## 5. Final Answer
Increasing on $(-\infty,1)$, decreasing on $(1,\infty)$; unique global maximum $(1,1/e)$. As $x\to+\infty$, $f(x)\to0^+$, so $y=0$ is a right-hand horizontal asymptote.
