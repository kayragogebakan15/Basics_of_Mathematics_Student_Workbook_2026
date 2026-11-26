# Exercise 3 — The Product Rule: Why Is It Needed?

## 1. Problem Statement
Differentiate $f(x)=(x^2+1)e^x$. Compare the correct derivative with the incorrect proposal $f'(x)=(2x)e^x$ and explain which term is missing.

## 2. Theoretical Background and Concepts
For differentiable factors $u$ and $v$, the product rule $(uv)'=u'v+uv'$ includes the contribution from each changing factor. We use $(x^2+1)'=2x$ and $(e^x)'=e^x$.

## 3. Detailed Step-by-Step Solution
Set $u=x^2+1$, $v=e^x$. Then $u'=2x$ and $v'=e^x$. Hence

$$
\begin{aligned}
f'(x)&=u'v+uv'\\
&=2xe^x+(x^2+1)e^x\\
&=e^x(x^2+2x+1)\\
&=e^x(x+1)^2.
\end{aligned}
$$

The incorrect expression keeps only $u'v=2xe^x$ and omits the entire term $uv'=(x^2+1)e^x$.

## 4. Verification and Consistency Checks
At $x=0$ the incorrect derivative predicts $0$ but the correct formula gives $1$. Indeed, using the definition and the standard exponential derivative limit,

$$
\begin{aligned}
f'(0)&=\lim_{h\to0}\frac{(1+h^2)e^h-1}{h}\\
&=\lim_{h\to0}\left(he^h+\frac{e^h-1}{h}\right)=0+1=1.
\end{aligned}
$$

Thus the independently calculated slope agrees with the product rule.

## 5. Final Answer
$f'(x)=e^x(x+1)^2$; the missing term is $(x^2+1)e^x$.
