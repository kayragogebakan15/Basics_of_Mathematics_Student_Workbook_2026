# Exercise 10 — Complete Function Analysis

## 1. Problem Statement
Completely analyze $f(x)=x/(x^2+1)$: domain, symmetry, zeros, limits, monotonicity, extrema, and convexity. Sketch the graph from these features.

## 2. Theoretical Background and Concepts
A continuous rational function has no domain breaks wherever its denominator is positive. Symmetry follows by comparing $f(-x)$ and $f(x)$. The first derivative determines monotonicity and extrema; the second determines concavity and inflection points when its sign changes. Limits at infinity determine horizontal asymptotes.

## 3. Detailed Step-by-Step Solution
**Domain, symmetry, zeros, and limits.** Because $x^2+1>0$ for all real $x$, the domain is $\mathbb R$. Since

$$
f(-x)=\frac{-x}{(-x)^2+1}=-f(x),
$$

the function is odd and its graph has rotational symmetry about the origin. The only zero and both coordinate-axis intercepts are at $(0,0)$. Also

$$
\lim_{x\to+\infty}f(x)=0^+,\qquad
\lim_{x\to-\infty}f(x)=0^-,
$$

by division by $x^2$ or dominant degrees. The horizontal asymptote is $y=0$.

**First derivative and extrema.** The quotient rule gives

$$
f'(x)=\frac{(x^2+1)-2x^2}{(x^2+1)^2}
=\frac{1-x^2}{(x^2+1)^2}.
$$

Its denominator is strictly positive. The numerator is positive for $|x|<1$, zero at $x=\pm1$, and negative for $|x|>1$. Therefore $f$ decreases on $(-\infty,-1)$, increases on $(-1,1)$, and decreases on $(1,\infty)$. There is a global minimum $f(-1)=-1/2$ at $x=-1$ and a global maximum $f(1)=1/2$ at $x=1$. These are global since

$$
(|x|-1)^2\ge0\quad\Longrightarrow\quad
x^2+1\ge2|x|,
$$

so $|x|/(x^2+1)\le1/2$.

**Second derivative and convexity.** Differentiate $f'=(1-x^2)(x^2+1)^{-2}$:

$$
\begin{aligned}
f''(x)
&=(-2x)(x^2+1)^{-2}
 +(1-x^2)(-2)(x^2+1)^{-3}(2x)\\
&=\frac{-2x(x^2+1)-4x(1-x^2)}{(x^2+1)^3}\\
&=\frac{2x(x^2-3)}{(x^2+1)^3}.
\end{aligned}
$$

Its zeros are $x=-\sqrt3$, $0$, and $\sqrt3$. The denominator stays positive; the numerator $2x(x^2-3)$ has signs

| Interval | Sign of $f''$ | Curvature |
|---|---|---|
| $(-\infty,-\sqrt3)$ | Negative | Concave down |
| $(-\sqrt3,0)$ | Positive | Concave up |
| $(0,\sqrt3)$ | Negative | Concave down |
| $(\sqrt3,\infty)$ | Positive | Concave up |

The second derivative changes sign at all three, so they are inflection points. Since $f(\pm\sqrt3)=\pm\sqrt3/4$ and $f(0)=0$, these are $(-\sqrt3,-\sqrt3/4)$, $(0,0)$, and $(\sqrt3,\sqrt3/4)$.

**Sketch instructions.** Read from left to right: approach $y=0$ from below while decreasing to the minimum $(-1,-1/2)$; rise through $(0,0)$ to the maximum $(1,1/2)$; then decrease toward $y=0$ from above. Mark the three inflection points where concavity changes. The left and right halves are rotations of each other through $180^\circ$.

A schematic guide for the height and direction of the branches:

~~~text
Plot window: x in [-5, 5], y in [-0.7, 0.7].
O = marked feature; * = sampled function curve.
+ = origin when visible; vertical | and horizontal - = axes.
                              |
                              |
                              |
                              |   **O****
                              |  *       *****
                              | *            ******
                              |**                 ***********
                              |*                            *
                              **
------------------------------O------------------------------
                             **
*                            *|
***********                 **|
          ******            * |
               *****       *  |
                    ****O**   |
                              |
                              |
                              |
~~~

The three marked O points are the global minimum (-1,-1/2), origin (0,0), and global maximum (1,1/2). The distant tails approach the horizontal axis from below and above, respectively.

The guide is qualitative; the ordered extrema, inflections, and end behavior above define the sketch precisely.

## 4. Verification and Consistency Checks
At $x=0$, $f'(0)=1>0$ as expected from the rise through the origin. At $x=2$, $f'(2)=(1-4)/25=-3/25<0$, confirming descent on the right. For the curvature, test $x=-2$, $-1$, $1$, $2$: the signs of $2x(x^2-3)$ are negative, positive, negative, positive, respectively. The three sign changes verify the claimed inflections; oddness confirms symmetry of the coordinates and curvature.

## 5. Final Answer
Domain $\mathbb R$; odd symmetry; zero $(0,0)$; horizontal asymptote $y=0$; decreasing on $(-\infty,-1)$ and $(1,\infty)$, increasing on $(-1,1)$; global minimum $(-1,-1/2)$ and maximum $(1,1/2)$; inflection points $(-\sqrt3,-\sqrt3/4)$, $(0,0)$, $(\sqrt3,\sqrt3/4)$, with the four concavity intervals listed above.
