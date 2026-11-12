# Exercise 5 — Hyperbola and Asymptotes

## 1. Problem Statement
For $\frac{x^2}{16}-\frac{y^2}{9}=1$, find its $x$-axis intercepts and asymptotes, sketch it, and explain the far-from-center role of the asymptotes.

## 2. Theoretical Background and Concepts
A horizontal hyperbola centered at the origin has form $\frac{x^2}{a^2}-\frac{y^2}{b^2}=1$, with vertices $(\pm a,0)$ and asymptotes $y=\pm\frac ba x$. The asymptote lines arise by dropping the constant $1$ in the large-coordinate approximation, or by considering the limiting slope.

## 3. Detailed Step-by-Step Solution
From $a^2=16$ and $b^2=9$, obtain $a=4$ and $b=3$. Setting $y=0$ gives

$$
\frac{x^2}{16}=1\quad\Longrightarrow\quad x=\pm4.
$$

The vertices and $x$-axis intercepts are therefore $(4,0)$ and $(-4,0)$. The asymptotes are

$$
y=\pm\frac{b}{a}x=\pm\frac34x.
$$

To see why, multiply the equation by $16$ and rearrange:

$$
x^2=16+\frac{16}{9}y^2,\qquad
y=\pm\frac34\sqrt{x^2-16}.
$$

For $x>4$, divide by $x$:

$$
\frac{y}{x}=\pm\frac34\sqrt{1-\frac{16}{x^2}}
\quad\longrightarrow\quad\pm\frac34
\qquad (x\to+\infty).
$$

The distance to the corresponding sloped lines approaches zero because $\sqrt{x^2-16}-x=-16/(\sqrt{x^2-16}+x)\to0$.

Qualitative sketch (not to scale; dotted diagonals indicate asymptote directions):

~~~text
               y
       .       |       .
        .      |      .
     (         |         )
------*--------+--------*------> x
     (-4,0)    |     (4,0)
     (         |         )
        .      |      .
       .       |       .
~~~

The two branches lie entirely in $x\le-4$ and $x\ge4$, and bend toward the diagonal asymptotes away from the center.

## 4. Verification and Consistency Checks
At $(\pm4,0)$, $16/16-0=1$. There are no $y$-axis intercepts: substituting $x=0$ gives $-y^2/9=1$, impossible for real $y$. Also $x^2/16=1+y^2/9\ge1$, confirming $|x|\ge4$.

## 5. Final Answer
Vertices/intercepts $(\pm4,0)$; asymptotes $y=\pm\frac34x$; horizontal left- and right-opening hyperbola.
