# Exercise 11 — A Parameter and the Number of Extrema

## 1. Problem Statement
For the family $f_a(x)=x^3-3ax$, determine the number of critical points and their nature depending on the real parameter $a$. Separate all cases and explain the changes in graph shape.

## 2. Theoretical Background and Concepts
Critical points of a differentiable function occur where its derivative vanishes. A zero of the derivative does not automatically represent an extremum; the derivative must change sign in the appropriate direction. Parameter values can change the number of real critical points by altering whether an equation has real roots.

## 3. Detailed Step-by-Step Solution
For every real $a$, the function is a polynomial defined on $\mathbb R$. Differentiate:

$$
f_a'(x)=3x^2-3a=3(x^2-a),\qquad f_a''(x)=6x.
$$

**Case 1: $a<0$.** Since $x^2\ge0>a$, we have $x^2-a>0$ for all $x$. Therefore $f_a'(x)>0$ everywhere. There are no critical points, the function is strictly increasing on $\mathbb R$, and there are no local extrema.

**Case 2: $a=0$.** Then $f_0(x)=x^3$ and $f_0'(x)=3x^2$. The derivative vanishes only at $x=0$, but is positive on both sides; it does not change sign. The origin is a stationary inflection point, not an extremum. Indeed $f_0''(x)=6x$ changes sign at zero, so the graph changes concavity there while remaining strictly increasing.

**Case 3: $a>0$.** The critical equation $x^2=a$ gives two distinct roots $x=-\sqrt a$ and $x=\sqrt a$. Factor:

$$
f_a'(x)=3(x-\sqrt a)(x+\sqrt a).
$$

The sign pattern is positive on $(-\infty,-\sqrt a)$, negative on $(-\sqrt a,\sqrt a)$, and positive on $(\sqrt a,\infty)$. Thus the graph increases, decreases, then increases. The point at $x=-\sqrt a$ is a local maximum and the point at $x=\sqrt a$ a local minimum.

Calculate their heights using $(\sqrt a)^3=a^{3/2}$:

$$
\begin{aligned}
f_a(-\sqrt a)&=-a^{3/2}+3a\sqrt a=2a^{3/2},\\
f_a(\sqrt a)&=a^{3/2}-3a\sqrt a=-2a^{3/2}.
\end{aligned}
$$

Consequently the local maximum is $(-\sqrt a,2a^{3/2})$ and local minimum $(\sqrt a,-2a^{3/2})$. Neither is an absolute extremum because every $f_a$ tends to $-\infty$ as $x\to-\infty$ and $+\infty$ as $x\to+\infty$.

## 4. Verification and Consistency Checks
For $a=1$, $f_1'(x)=3(x-1)(x+1)$ has signs $+,-,+$; the predicted extrema are $(-1,2)$ and $(1,-2)$. For $a=-1$, $f_{-1}'(x)=3(x^2+1)>0$, so no roots or extrema exist. For $a=0$, the derivative $3x^2$ remains nonnegative on both sides of the stationary point, verifying why it is not a maximum or minimum. The second derivative values for $a>0$ are $f_a''(-\sqrt a)=-6\sqrt a<0$ and $f_a''(\sqrt a)=6\sqrt a>0$, independently confirming their types.

## 5. Final Answer
For $a<0$, there are no critical points and no extrema. For $a=0$, there is one critical point $(0,0)$, a stationary inflection, but no extremum. For $a>0$, there are two critical points: local maximum $(-\sqrt a,2a^{3/2})$ and local minimum $(\sqrt a,-2a^{3/2})$.
