# Exercise 13 — A Logarithm and an Asymptote

## 1. Problem Statement
Completely analyze $f(x)=\ln x/x$ for $x>0$: determine its zero, monotonicity, maximum, limits at the ends of its domain, asymptotes and the information needed for a correct sketch.

## 2. Theoretical Background and Concepts
A logarithm requires a positive argument. For a quotient, the sign of the derivative determines monotonicity; the derivative's zero is only a candidate extremum until its sign change is checked. Near a domain boundary, an infinite limit indicates a vertical asymptote. A finite limit at infinity indicates a horizontal asymptote.

## 3. Detailed Step-by-Step Solution
The domain is $(0,\infty)$. The numerator $\ln x$ vanishes at $x=1$, so the only zero is $(1,0)$. The denominator is always positive, so $f(x)<0$ for $0<x<1$ and $f(x)>0$ for $x>1$.

Using the quotient rule,

$$
f'(x)=\frac{x(1/x)-(\ln x)\cdot1}{x^2}
=\frac{1-\ln x}{x^2}.
$$

The denominator is positive. Solve $1-\ln x=0$ to find $\ln x=1$, or $x=e$. Thus $f'>0$ on $(0,e)$ and $f'<0$ on $(e,\infty)$. The function rises to a global maximum at

$$
f(e)=\frac{\ln e}{e}=\frac1e.
$$

At the left endpoint, set $t=1/x$. As $x\to0^+$, $t\to+\infty$ and

$$
\frac{\ln x}{x}=-t\ln t\longrightarrow-\infty.
$$

Therefore $x=0$ is a vertical asymptote approached from the right, and the graph falls to $-\infty$ near that boundary. At the far right,

$$
\lim_{x\to+\infty}\frac{\ln x}{x}=0^+.
$$

This follows, for example, by l'Hôpital's rule on the $\infty/\infty$ form: the derivative quotient is $(1/x)/1=1/x\to0$. Hence $y=0$ is a horizontal asymptote at positive infinity, approached from above after the maximum.

For curvature and a more accurate sketch, differentiate once more:

$$
\begin{aligned}
f''(x)
&=\frac{-1}{x}\cdot x^{-2}+(1-\ln x)(-2)x^{-3}\\
&=\frac{-1-2+2\ln x}{x^3}\\
&=\frac{2\ln x-3}{x^3}.
\end{aligned}
$$

The concavity changes at $\ln x=3/2$, or $x=e^{3/2}$. It is concave down on $(0,e^{3/2})$ and concave up on $(e^{3/2},\infty)$, with inflection point $(e^{3/2},3/(2e^{3/2}))$.

Qualitative sketch (not to scale):

~~~text
    y
    ^         max (e,1/e)
    |           *
    |         /   \____ -> y=0+
  0 +--------*----------------------> x
    |       x=1
    |      /
    |    /
    |  /
    | / 
    :/
   x=0  vertical asymptote
~~~

The plot must distinguish the excluded boundary $x=0$, the crossing at $x=1$, the peak at $x=e$, the later change of concavity, and the approach to zero from above.

## 4. Verification and Consistency Checks
$f'(1)=(1-\ln1)/1=1>0$, so the curve crosses zero while increasing. At $x=e^2>e$, $1-\ln(e^2)=-1<0$, confirming descent after the maximum. As $x\to0^+$, $\ln x<0$ and $1/x>0$ diverges, consistent with negative infinity. The inflection occurs strictly after the maximum because $e^{3/2}>e$, consistent with bending back toward the horizontal asymptote.

## 5. Final Answer
Domain $(0,\infty)$; zero $(1,0)$; increasing on $(0,e)$, decreasing on $(e,\infty)$; global maximum $(e,1/e)$. Vertical asymptote $x=0$ and horizontal asymptote $y=0$ as $x\to+\infty$. Inflection point $(e^{3/2},3/(2e^{3/2}))$.
