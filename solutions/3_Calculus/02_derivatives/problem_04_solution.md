# Exercise 4 — A Quotient and Domain Control

## 1. Problem Statement
Determine the domain of $f(x)=(x^2+1)/(x-1)$, compute and simplify $f'(x)$, and explain why $x=1$ is excluded.

## 2. Theoretical Background and Concepts
The quotient rule gives $(u/v)'=(u'v-uv')/v^2$ wherever $v\ne0$. A derivative cannot be defined at a point at which the original function is not defined.

## 3. Detailed Step-by-Step Solution
Because $x-1=0$ at $x=1$, the domain is all real numbers except $1$. Let $u=x^2+1$ and $v=x-1$. Then $u'=2x$, $v'=1$ and

$$
\begin{aligned}
f'(x)
&=\frac{2x(x-1)-(x^2+1)\cdot1}{(x-1)^2}\\
&=\frac{2x^2-2x-x^2-1}{(x-1)^2}\\
&=\frac{x^2-2x-1}{(x-1)^2}.
\end{aligned}
$$

## 4. Verification and Consistency Checks
Divide the original numerator: $x^2+1=(x-1)(x+1)+2$. For $x\ne1$,

$$
f(x)=x+1+\frac2{x-1}.
$$

Differentiating independently,

$$
f'(x)=1-\frac2{(x-1)^2}
=\frac{(x-1)^2-2}{(x-1)^2}
=\frac{x^2-2x-1}{(x-1)^2}.
$$

At $x=1$, the original numerator is $2$ and the denominator $0$; it is a nonremovable singularity, so this point remains excluded.

## 5. Final Answer
The domain is $\mathbb R\setminus\{1\}$ and $f'(x)=(x^2-2x-1)/(x-1)^2$ for $x\ne1$.
