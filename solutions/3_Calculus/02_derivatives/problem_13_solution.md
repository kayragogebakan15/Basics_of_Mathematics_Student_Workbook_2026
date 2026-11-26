# Exercise 13 — A Multi-Layer Composition

## 1. Problem Statement
For $f(x)=e^{\sin(x^2)}$, write the layers $x\longrightarrow x^2\longrightarrow\sin(x^2)\longrightarrow e^{\sin(x^2)}$, compute the derivative, and explain the reverse-order chain-rule process.

## 2. Theoretical Background and Concepts
For a composition of three differentiable functions, the chain rule multiplies the derivative of the outer layer by the derivative of the middle layer and then by the derivative of the inner layer, each evaluated at its proper input. This reverses the construction order because an infinitesimal change passes from $x$ through each intermediate variable.

## 3. Detailed Step-by-Step Solution
Define the successive layers

$$
u=x^2,\qquad v=\sin u,\qquad f=e^v.
$$

Their derivatives with respect to their immediate inputs are

$$
\frac{du}{dx}=2x,\qquad
\frac{dv}{du}=\cos u,\qquad
\frac{df}{dv}=e^v.
$$

Multiply in reverse layer order:

$$
\begin{aligned}
\frac{df}{dx}
&=\frac{df}{dv}\cdot\frac{dv}{du}\cdot\frac{du}{dx}\\
&=e^v\cos u\cdot2x\\
&=2xe^{\sin(x^2)}\cos(x^2).
\end{aligned}
$$

The outer exponential's derivative remains the same exponential, the sine contributes cosine, and the inner square contributes $2x$. Leaving out any of the three contributions would ignore a layer of the composition.

## 4. Verification and Consistency Checks
At $x=0$, the formula gives $f'(0)=0$, since $2x=0$. This is consistent with evenness: $f(-x)=e^{\sin((-x)^2)}=f(x)$, so a differentiable even function must have zero derivative at the origin. At $x=1$ the derivative becomes $2e^{\sin1}\cos1$, consistent with substitution into the chain-rule factors.

## 5. Final Answer
$f'(x)=2xe^{\sin(x^2)}\cos(x^2)$ for all real $x$.
