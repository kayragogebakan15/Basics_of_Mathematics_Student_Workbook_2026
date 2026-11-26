# Exercise 15 — The Difference Quotient as a Check of the Derivative

## 1. Problem Statement
Choose a function from the set and a point $x_0$ where its derivative exists. Compute $f'(x_0)$ exactly, evaluate $(f(x_0+h)-f(x_0))/h$ at $h=1$, $0.1$, and $0.01$, compare the values with the derivative, and explain why numerical observations alone are not a proof.

## 2. Theoretical Background and Concepts
The derivative is the limit

$$
f'(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}h
$$

provided it exists. Computing finitely many difference quotients can illustrate the approach to a tangent slope but cannot establish the limit for every sufficiently small nonzero $h$. An exact simplification followed by a limit supplies the missing mathematical justification.

## 3. Detailed Step-by-Step Solution
Choose the polynomial $f(x)=x^2$ from Exercise 11, at the point $x_0=2$. Its derivative is $f'(x)=2x$, so

$$
f'(2)=2(2)=4.
$$

Now calculate the difference quotient for arbitrary $h\ne0$:

$$
\begin{aligned}
\frac{f(2+h)-f(2)}h
&=\frac{(2+h)^2-2^2}h\\
&=\frac{4+4h+h^2-4}{h}\\
&=\frac{4h+h^2}{h}\\
&=4+h.
\end{aligned}
$$

Substitute the three requested positive increments:

| $h$ | Exact quotient $4+h$ | Difference from $f'(2)=4$ |
|---:|---:|---:|
| $1$ | $5$ | $1$ |
| $0.1$ | $4.1$ | $0.1$ |
| $0.01$ | $4.01$ | $0.01$ |

The values approach $4$ as $h$ decreases.

For a proof, use the exact identity for all nonzero increments:

$$
\lim_{h\to0}(4+h)=4.
$$

The same result holds from negative increments: the formula is valid for $h<0$ as well. More precisely, for any $\varepsilon>0$, choosing $\delta=\varepsilon$ gives

$$
0<|h|<\delta
\quad\Longrightarrow\quad
\left|\frac{f(2+h)-f(2)}h-4\right|
=|h|<\varepsilon.
$$

This proves the derivative limit without relying on the table.

## 4. Verification and Consistency Checks
At $h=1$, $(f(3)-f(2))/1=(9-4)/1=5$. At $h=0.1$, $(2.1^2-4)/0.1=(4.41-4)/0.1=4.1$. At $h=0.01$, $(2.01^2-4)/0.01=(4.0401-4)/0.01=4.01$. Each agrees with $4+h$, and the exact error is $|h|$, which tends to zero from either side. A finite table alone could miss unexpected behavior at other increments, but the identity and quantified bound cover all nonzero sufficiently small $h$.

## 5. Final Answer
For $f(x)=x^2$ at $x_0=2$, $f'(2)=4$. The three difference quotients are $5$, $4.1$, and $4.01$; their convergence to $4$ is proved by the identity $Q(h)=4+h$ and the bound $|Q(h)-4|=|h|$.
