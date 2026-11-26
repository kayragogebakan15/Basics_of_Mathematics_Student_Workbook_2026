# Exercise 6 — A Logarithmic Function

## 1. Problem Statement
Analyze the domain, zero, and monotonicity of $f(x)=\ln x-x+1$. Explain why the domain must be established before differentiation and sign analysis.

## 2. Theoretical Background and Concepts
The real logarithm $\ln x$ is defined only for $x>0$, so a calculus analysis must stay within this domain. The derivative of $\ln x$ is $1/x$ for positive $x$. A change of sign of $f'$ from positive to negative marks a maximum; a function that rises to a unique maximum of zero and then falls has no other roots.

## 3. Detailed Step-by-Step Solution
The domain is $(0,\infty)$. For $x>0$,

$$
f'(x)=\frac1x-1=\frac{1-x}{x}.
$$

Since $x>0$, the denominator is always positive. Thus the derivative has the same sign as $1-x$: it is positive for $0<x<1$, zero at $x=1$, and negative for $x>1$. The function increases on $(0,1)$ and decreases on $(1,\infty)$.

At the only critical point,

$$
f(1)=\ln1-1+1=0.
$$

Hence the graph has its unique global maximum $0$ at $x=1$. In particular, the only zero is $x=1$: the increasing and decreasing branches have strictly smaller values away from their common maximum. At the left endpoint, $\ln x\to-\infty$ as $x\to0^+$ while $-x+1\to1$, so $f(x)\to-\infty$. At the right, $\ln x-x\to-\infty$ as $x\to+\infty$ (for instance, $\ln x/x\to0$, so $x(\ln x/x-1)\to-\infty$).

## 4. Verification and Consistency Checks
Evaluate the derivative at $x=1/2$: $f'(1/2)=2-1=1>0$. At $x=2$, $f'(2)=1/2-1=-1/2<0$. These confirm the rise and fall. The inequality $\ln x\le x-1$ for all $x>0$, with equality only at $x=1$, independently proves $f(x)\le0$ and its unique zero. The vertical asymptote $x=0$ is approached only from the right because nonpositive inputs are not in the domain.

## 5. Final Answer
Domain $(0,\infty)$; unique zero and global maximum at $(1,0)$; increasing on $(0,1)$ and decreasing on $(1,\infty)$. The domain restriction is essential because $\ln x$ is not real-valued for $x\le0$.
