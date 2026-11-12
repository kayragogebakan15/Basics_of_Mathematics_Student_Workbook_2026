# Exercise 3 — Ellipse

## 1. Problem Statement
For $\frac{x^2}{25}+\frac{y^2}{9}=1$, find the semiaxis lengths and coordinate-axis intercepts, sketch the ellipse, and explain its greater horizontal extension.

## 2. Theoretical Background and Concepts
An axis-aligned ellipse centered at the origin has equation $\frac{x^2}{a^2}+\frac{y^2}{b^2}=1$. The square roots of the denominators give its semiaxis lengths. The larger denominator corresponds to the longer axis because setting the other coordinate to zero gives the maximum absolute coordinate.

## 3. Detailed Step-by-Step Solution
Compare denominators:

$$
a^2=25\quad\Longrightarrow\quad a=5,\qquad b^2=9\quad\Longrightarrow\quad b=3.
$$

For the $x$-axis, set $y=0$:

$$
\frac{x^2}{25}=1\quad\Longrightarrow\quad x=\pm5.
$$

For the $y$-axis, set $x=0$:

$$
\frac{y^2}{9}=1\quad\Longrightarrow\quad y=\pm3.
$$

The center is $(0,0)$. The major axis is horizontal, has full length $10$, and the minor axis is vertical, with full length $6$.

Qualitative sketch (not to scale):

~~~text
                   y
                   ^
                 (0,3)
              .----|----.
           .-'     |     '-.
(-5,0) ---*--------+--------*--- (5,0) --> x
           '-.     |     .-'
              '----|----'
                 (0,-3)
~~~

The wider horizontal span reflects $25>9$.

## 4. Verification and Consistency Checks
Substitution gives $25/25+0=1$ at $(\pm5,0)$ and $0+9/9=1$ at $(0,\pm3)$. Also, any point of the ellipse satisfies $x^2/25\le1$ and $y^2/9\le1$, so $|x|\le5$ and $|y|\le3$.

## 5. Final Answer
The center is $(0,0)$; horizontal semiaxis $5$, vertical semiaxis $3$; intercepts $(\pm5,0)$ and $(0,\pm3)$. It is stretched along the $x$-axis.
