# Exercise 10 — Paraboloids

## 1. Problem Statement
Compare $z=x^2+y^2$ and $z=x^2-y^2$. For each, classify sections $x=0$, $y=0$, and $z=c$, and give a qualitative sketch.

## 2. Theoretical Background and Concepts
Fixing one coordinate reduces a surface equation to a 2D curve. A sum of positive squares is nonnegative and produces an upward-opening elliptic paraboloid. A difference of squares takes both signs and produces a hyperbolic paraboloid (saddle). Horizontal sections distinguish circles from hyperbolas and crossing lines.

## 3. Detailed Step-by-Step Solution
**Surface A: $z=x^2+y^2$.**
- In the plane $x=0$: $z=y^2$, an upward-opening parabola in the $yz$-plane.
- In the plane $y=0$: $z=x^2$, an upward-opening parabola in the $xz$-plane.
- In the plane $z=c$: $x^2+y^2=c$. For $c>0$ this is a circle of radius $\sqrt c$; for $c=0$ it is the origin alone; for $c<0$ it has no real points.

Sketch (schematic vertical profile and horizontal levels):

~~~text
          z
          ^
       \     /
        \   /        bowl rising in every radial direction
         \_/
          +--------> x
      z=c>0: circular horizontal ring
~~~

**Surface B: $z=x^2-y^2$.**
- In the plane $x=0$: $z=-y^2$, a downward-opening parabola in the $yz$-plane.
- In the plane $y=0$: $z=x^2$, an upward-opening parabola in the $xz$-plane.
- In the plane $z=c$: $x^2-y^2=c$. For $c>0$, a hyperbola opening along $\pm x$; for $c<0$, a hyperbola opening along $\pm y$; for $c=0$, two crossing lines $y=x$ and $y=-x$ in the horizontal plane.

Sketch (qualitative vertical profiles along perpendicular directions):

~~~text
      xz-section: U       yz-section: inverted U
          \ /                      / \
           V                        ^
      rising along x         falling along y

         z=0:  y=x and y=-x  (crossing lines)
~~~

## 4. Verification and Consistency Checks
For A, $z\ge0$ everywhere and the sections $z=1$ have radius $1$. For B, $(1,0)$ has $z=1$, while $(0,1)$ has $z=-1$, proving it rises along $x$ and falls along $y$. At $z=0$, substituting either $y=x$ or $y=-x$ gives $x^2-y^2=0$.

## 5. Final Answer
$z=x^2+y^2$ is an upward elliptic (circular) paraboloid; $z=x^2-y^2$ is a saddle-shaped hyperbolic paraboloid. Their horizontal sections are, respectively, circles and hyperbolas (with the specified limiting cases).
