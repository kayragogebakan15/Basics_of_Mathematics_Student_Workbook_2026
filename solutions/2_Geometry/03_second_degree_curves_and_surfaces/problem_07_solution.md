# Exercise 7 — Classifying a Second-Degree Equation

## 1. Problem Statement
Classify $4x^2+9y^2=36$, $x^2-y^2=1$, $x^2-4y=0$, and $x^2+y^2+1=0$. Explain why the last equation has no real points.

## 2. Theoretical Background and Concepts
Two positive squared-coordinate terms producing a positive constant typically define an ellipse. Opposite signs indicate a hyperbola; one squared coordinate and one linear coordinate indicate a parabola. Over the real numbers, a sum of squares cannot be negative, so algebraic form must also be checked for existence.

## 3. Detailed Step-by-Step Solution
**1.** Divide $4x^2+9y^2=36$ by $36$:

$$
\frac{x^2}{9}+\frac{y^2}{4}=1.
$$

This is an ellipse centered at $(0,0)$, with horizontal semiaxis $3$, vertical semiaxis $2$, and intercepts $(\pm3,0)$, $(0,\pm2)$.

**2.** The equation $x^2-y^2=1$ is already the canonical form of a horizontal hyperbola. Its center is $(0,0)$, vertices $(\pm1,0)$ and asymptotes $y=\pm x$.

**3.** Rearranging $x^2-4y=0$ gives

$$
x^2=4y.
$$

This is an upward-opening parabola with vertex $(0,0)$, vertical symmetry axis $x=0$, and $p=1$ in the form $x^2=4py$.

**4.** Rearrange $x^2+y^2+1=0$:

$$
x^2+y^2=-1.
$$

For all real $x,y$, $x^2\ge0$ and $y^2\ge0$, hence $x^2+y^2\ge0$. It cannot equal $-1$. The real solution set is empty; this is not a real circle.

## 4. Verification and Consistency Checks
For the ellipse, $(3,0)$ gives $4(9)=36$. For the hyperbola, $(1,0)$ gives $1-0=1$. For the parabola, $(2,1)$ gives $4-4=0$. For the last equation, its left-hand side is always at least $1$, so it can never vanish.

## 5. Final Answer
The objects are (1) an ellipse, (2) a horizontal hyperbola, (3) an upward-opening parabola, and (4) the empty real set.
