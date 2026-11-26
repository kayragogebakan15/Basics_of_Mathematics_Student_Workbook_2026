# Exercise 6 — Product Rule and Trigonometry

## 1. Problem Statement
For $f(x)=x\sin x+\cos x$, compute and simplify $f'(x)$, evaluate $f'(0)$, and interpret the tangent direction at $x=0$.

## 2. Theoretical Background and Concepts
For differentiable $u,v$, $(uv)'=u'v+uv'$. In radians, $(\sin x)'=\cos x$ and $(\cos x)'=-\sin x$. A derivative of zero at a point indicates a horizontal tangent, not necessarily a constant function.

## 3. Detailed Step-by-Step Solution
Use $u=x$ and $v=\sin x$. The product rule yields

$$
(x\sin x)'=1\cdot\sin x+x\cos x.
$$

The second term has derivative $(\cos x)'=-\sin x$. Adding contributions cancels the sine terms:

$$
\begin{aligned}
f'(x)&=\sin x+x\cos x-\sin x\\
&=x\cos x.
\end{aligned}
$$

At the origin,

$$
f'(0)=0\cdot\cos0=0.
$$

The tangent is horizontal at $x=0$. Since $f(0)=0\cdot0+\cos0=1$, its tangent equation is $y=1$.

## 4. Verification and Consistency Checks
Check directly by the difference quotient:

$$
\frac{f(h)-f(0)}h
=\sin h+\frac{\cos h-1}{h}.
$$

Here $\sin h\to0$ and $(\cos h-1)/h=-2\sin^2(h/2)/h=-\sin(h/2)\bigl(\sin(h/2)/(h/2)\bigr)\to0$. Thus the quotient tends to zero, confirming $f'(0)=0$ independently of the differentiation rules.

## 5. Final Answer
$f'(x)=x\cos x$; $f'(0)=0$, so the tangent at $(0,1)$ is the horizontal line $y=1$.
