# Exercise 1 — Recognizing Curves from Canonical Form

## 1. Problem Statement
Recognize and sketch $x^2+y^2=9$, $\frac{x^2}{16}+\frac{y^2}{9}=1$, $y^2=8x$, and $\frac{x^2}{9}-\frac{y^2}{4}=1$. Identify their main geometric features and explain how the equations reveal the curve types.

## 2. Theoretical Background and Concepts
A sum of two equal squared-coordinate terms equal to $r^2$ describes a circle. A positive sum of squared-coordinate fractions equal to $1$ gives an ellipse. An equation with one coordinate squared and the other linear gives a parabola. A difference of squared-coordinate fractions equal to $1$ gives a hyperbola. Denominators show squared semiaxis lengths, and the sign of each term determines orientation.

## 3. Detailed Step-by-Step Solution

**Curve A: $x^2+y^2=9$.** The squared coordinates have equal coefficients and $9=3^2$. It is a circle centered at $(0,0)$ with radius $3$. Its axis intercepts are $(\pm3,0)$ and $(0,\pm3)$.

**Curve B: $\frac{x^2}{16}+\frac{y^2}{9}=1$.** Both terms are positive but have different denominators. It is an ellipse centered at $(0,0)$, with horizontal semiaxis $a=\sqrt{16}=4$ and vertical semiaxis $b=\sqrt9=3$. Its vertices on the coordinate axes are $(\pm4,0)$ and $(0,\pm3)$; the major axis is horizontal.

**Curve C: $y^2=8x$.** Compare with $y^2=4px$ to get $4p=8$, hence $p=2$. The parabola has vertex $(0,0)$, symmetry axis $y=0$, opens toward positive $x$, focus $(2,0)$, and directrix $x=-2$. For example, setting $x=2$ gives $y=\pm4$.

**Curve D: $\frac{x^2}{9}-\frac{y^2}{4}=1$.** The opposite signs identify a hyperbola opening left and right. It is centered at $(0,0)$ with $a=3$, $b=2$, vertices $(\pm3,0)$, asymptotes $y=\pm\frac23x$, and no $y$-axis intercepts.

Qualitative sketches (not to scale; the axes cross at the origin):

~~~text
Circle                 Ellipse
        y                      y
      ***                  ********
    *  |  *             **    |    **
 ---*---+---*--- x    --*------+------*-- x
    *  |  *             **    |    **
      ***                  ********

Parabola (opens right)   Hyperbola (opens both ways)
       y                       y
   \   |                 \     |     /
    \  |                  \    |    /
 ----\ +-------> x       )----+----( ----> x
    /  |                  /    |    \
   /   |                 /     |     \
~~~

In the parabola sketch, the vertex is at the origin; its branches extend into the right half-plane. The hyperbola sketches show separated left and right branches; the diagonal strokes represent asymptote directions.

## 4. Verification and Consistency Checks
For the circle, $(3,0)$ gives $9=9$. For the ellipse, $(4,0)$ gives $16/16=1$. For the parabola, $(2,4)$ gives $16=8(2)$. For the hyperbola, $(3,0)$ gives $9/9-0=1$. These checks confirm each scale and intercept.

## 5. Final Answer
The four curves are, respectively, a radius-$3$ circle, a horizontal ellipse with semiaxes $(4,3)$, a right-opening parabola with $p=2$, and a horizontal hyperbola with $a=3$, $b=2$ and asymptotes $y=\pm\frac23x$.
