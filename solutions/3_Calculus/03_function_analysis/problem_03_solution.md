# Exercise 3 — A Rational Function

## 1. Problem Statement
Analyze the domain, zeros, asymptotes, and monotonicity of $f(x)=(x+1)/(x-2)$. Sketch its graph consistently with these features.

## 2. Theoretical Background and Concepts
A rational function is undefined at a zero of its denominator. A zero of its numerator gives a function zero only where the denominator is nonzero. A vertical asymptote occurs at a noncancelable pole; a horizontal asymptote $y=L$ follows when $f(x)\to L$ as $x\to\pm\infty$. Derivative signs establish the direction of each graph branch.

## 3. Detailed Step-by-Step Solution
The denominator requires $x\ne2$, so the domain is $\mathbb R\setminus\{2\}$. The numerator vanishes at $x=-1$, giving zero $(-1,0)$. The $y$-intercept is $f(0)=1/(-2)=-1/2$.

Rewrite the expression:

$$
f(x)=\frac{x-2+3}{x-2}=1+\frac3{x-2}.
$$

Since $3/(x-2)\to0$ as $x\to\pm\infty$, $y=1$ is the horizontal asymptote. Near $x=2$, the numerator is close to $3>0$ and the denominator changes sign:

$$
\lim_{x\to2^-}f(x)=-\infty,\qquad
\lim_{x\to2^+}f(x)=+\infty.
$$

Thus $x=2$ is the vertical asymptote.

The derivative is

$$
f'(x)=\frac{(x-2)-(x+1)}{(x-2)^2}
=-\frac3{(x-2)^2}<0,\qquad x\ne2.
$$

Therefore **both branches decrease as $x$ increases**, separately on $(-\infty,2)$ and $(2,\infty)$. On the left, the graph approaches $y=1$ from below at $-\infty$, passes through $(-1,0)$ and $(0,-1/2)$, then falls to $-\infty$ near $2$. On the right, it descends from $+\infty$ near $2$ toward $y=1$ from above.

Schematic sketches (not to scale; vertical dotted guides represent $x=2$):

~~~text
Left branch: x<2              Right branch: x>2
   y                              y
   ^  y=1                         ^ :\
 1 +.........                  1 +.:.\........ y=1
   |  \                           | :  \____
 0 +---\------:---> x           0 +.:----------> x
   |    \     :                   | :
   |     \    :                   | :
   |       \  :                   | :
   |        \ :                   | :
             x=2                    x=2
~~~

## 4. Verification and Consistency Checks
At $x=-1$, $(-1+1)/(-1-2)=0$. At $x=0$, $f(0)=-1/2$, as above. Test slope signs: $f'(0)=-3/4<0$ and $f'(3)=-3<0$. These confirm the same decreasing direction on both sides; the branches are never connected across the excluded value $x=2$. At $x=1$, $f(1)=-2$, whereas at $x=3$, $f(3)=4$, matching the sides of the asymptotes.

## 5. Final Answer
Domain $\mathbb R\setminus\{2\}$; zero $x=-1$; vertical asymptote $x=2$; horizontal asymptote $y=1$; strictly decreasing on $(-\infty,2)$ and $(2,\infty)$.
