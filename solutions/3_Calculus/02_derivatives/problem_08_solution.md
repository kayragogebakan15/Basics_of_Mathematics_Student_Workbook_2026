# Exercise 8 — Two Exponential Functions

## 1. Problem Statement
For $f(x)=e^{2x-3}+5^x$, calculate $f'(x)$ and explain the appearance of the factors $2$ and $\ln5$.

## 2. Theoretical Background and Concepts
The exponential derivative rules are $(e^{u(x)})'=e^{u(x)}u'(x)$ and $(a^x)'=a^x\ln a$ for a constant base $a>0$. The first follows from the chain rule; the second follows by rewriting $a^x=e^{x\ln a}$ and differentiating this composition.

## 3. Detailed Step-by-Step Solution
Set $u(x)=2x-3$, so $u'(x)=2$. Differentiating the first summand gives

$$
\frac{d}{dx}e^{2x-3}=e^{2x-3}(2)=2e^{2x-3}.
$$

For the second summand use $5^x=e^{x\ln5}$, with inner derivative $\ln5$:

$$
\frac{d}{dx}5^x=e^{x\ln5}\ln5=5^x\ln5.
$$

By the sum rule,

$$
f'(x)=2e^{2x-3}+5^x\ln5.
$$

## 4. Verification and Consistency Checks
At $x=0$ the derivative formula gives $f'(0)=2e^{-3}+\ln5$. The chain-factor check is immediate from $d(2x-3)/dx=2$ and $d(x\ln5)/dx=\ln5$. Because $e^{2x-3}>0$, $5^x>0$, and $\ln5>0$, the derivative is positive for every real $x$; the function is increasing, consistent with both exponential terms.

## 5. Final Answer
$f'(x)=2e^{2x-3}+5^x\ln5$ for all real $x$.
