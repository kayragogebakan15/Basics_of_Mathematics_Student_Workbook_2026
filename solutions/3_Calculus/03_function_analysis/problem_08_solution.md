# Exercise 8 — The Second Derivative

## 1. Problem Statement
For $f(x)=x^4-4x^2$, find the local extrema, intervals of convexity and concavity, and inflection points. Sketch the graph and mark the identified features.

## 2. Theoretical Background and Concepts
Critical points are found from $f'=0$ and classified using changes in its sign or the second derivative. Where $f''>0$, the graph is concave upward (convex); where $f''<0$, it is concave downward. A genuine inflection point requires a change of concavity, not merely $f''=0$.

## 3. Detailed Step-by-Step Solution
The function is a polynomial on $\mathbb R$. Differentiate twice:

$$
f'(x)=4x^3-8x=4x(x^2-2),
$$

$$
f''(x)=12x^2-8=4(3x^2-2).
$$

The critical numbers are $x=-\sqrt2$, $x=0$, and $x=\sqrt2$. Evaluate:

$$
f(\pm\sqrt2)=(\sqrt2)^4-4(\sqrt2)^2=4-8=-4,\qquad f(0)=0.
$$

At $x=0$, $f''(0)=-8<0$, so $(0,0)$ is a local maximum. At $x=\pm\sqrt2$, $f''=12(2)-8=16>0$, so $(\pm\sqrt2,-4)$ are local minima; since $f(x)=(x^2-2)^2-4\ge-4$, they are global minima.

For inflections, solve $f''(x)=0$:

$$
12x^2-8=0\quad\Longrightarrow\quad x^2=\frac23
\quad\Longrightarrow\quad x=\pm\sqrt{\frac23}.
$$

The second derivative is positive for $|x|>\sqrt{2/3}$ and negative for $|x|<\sqrt{2/3}$. Hence the graph is concave upward on $(-\infty,-\sqrt{2/3})$ and $(\sqrt{2/3},\infty)$, and concave downward on $(-\sqrt{2/3},\sqrt{2/3})$.

At both inflection abscissas $x^2=2/3$, so

$$
f(x)=\left(\frac23\right)^2-4\left(\frac23\right)
=\frac49-\frac83=-\frac{20}{9}.
$$

Thus the inflection points are $(\pm\sqrt{2/3},-20/9)$.

Qualitative sketch (not to scale, symmetric about the $y$-axis):

~~~text
Plot window: x in [-2.5, 2.5], y in [-5, 9].
O = marked feature; * = sampled function curve.
+ = origin when visible; vertical | and horizontal - = axes.
  *                           |                           *
  *                           |                           *
  *                           |                           *
  **                          |                          **
   *                          |                          *
   *                          |                          *
   **                         |                         **
    *                         |                         *
    *                         |                         *
     *                        |                        *
     *                        |                        *
      *                       |                       *
------**-----------------*****O*****-----------------**------
       *              ****    |    ****              *
       **           O**       |       **O           **
        **        ***         |         ***        **
         ***   ****           |           ****   ***
           **O**              |              **O**
                              |
~~~

The five marked O locations are the left minimum, left inflection, central maximum, right inflection, and right minimum (in increasing x order). The W-shaped curve rises toward +infinity at both ends.

To read the sketch correctly: starting from high values on the far left, the curve falls to its left minimum, rises to $(0,0)$, falls to its right minimum, and rises toward $+\infty$ on the far right. The inflection points, on the inner rising/falling portions, have height $-20/9$.

## 4. Verification and Consistency Checks
The derivative factorization gives signs negative on $(-\infty,-\sqrt2)$, positive on $(-\sqrt2,0)$, negative on $(0,\sqrt2)$, positive on $(\sqrt2,\infty)$, confirming all three extrema. The even identity $f(-x)=f(x)$ confirms symmetric features. Since $f''$ changes sign at both $\pm\sqrt{2/3}$, neither is merely a stationary candidate without inflection.

## 5. Final Answer
Local maximum $(0,0)$; global minima $(\pm\sqrt2,-4)$; concave up for $|x|>\sqrt{2/3}$, concave down for $|x|<\sqrt{2/3}$; inflection points $(\pm\sqrt{2/3},-20/9)$.
