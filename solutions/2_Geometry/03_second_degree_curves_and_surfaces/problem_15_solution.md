# Exercise 15 — Recognition and Sketch Without a Given Name

## 1. Problem Statement
For $4x^2+9y^2-8x+36y+4=0$, complete the square, identify its features, and sketch the curve. For $4x^2+y^2=z^2$, first analyze the sections $z=c$, $x=0$ and $y=0$ (including different axis scales); only then identify and sketch the surface.

## 2. Theoretical Background and Concepts
Completing the square converts a translated quadratic curve to canonical form. When both squared-coordinate terms have positive coefficients, a positive right-hand side produces an ellipse. In three dimensions, fixing coordinates reveals the surface from its sections: elliptical horizontal level curves, or pairs of crossing lines in vertical planes, indicate a cone, with unequal coefficients producing unequal horizontal radii.

## 3. Detailed Step-by-Step Solution
**Part A — Curve in the plane.**

Start with

$$
4x^2+9y^2-8x+36y+4=0.
$$

Group variable terms and factor their coefficients:

$$
4(x^2-2x)+9(y^2+4y)=-4.
$$

Complete squares inside the parentheses:

$$
4((x-1)^2-1)+9((y+2)^2-4)=-4.
$$

Combine constants:

$$
4(x-1)^2+9(y+2)^2-4-36=-4,
$$

$$
4(x-1)^2+9(y+2)^2=36.
$$

Divide by $36$:

$$
\frac{(x-1)^2}{9}+\frac{(y+2)^2}{4}=1.
$$

This is an ellipse centered at $(1,-2)$, with horizontal semiaxis $3$, vertical semiaxis $2$, and its longer axis parallel to the $x$-axis. The major vertices are $(-2,-2)$ and $(4,-2)$; the minor vertices are $(1,0)$ and $(1,-4)$. The full axis lengths are $6$ and $4$.

Qualitative sketch (not to scale):

~~~text
                 y
               (1,0)
             .---|---.
(-2,-2) ----*----C----*---- (4,-2) --> x
             '---|---'
               (1,-4)

C=(1,-2), horizontal semiaxis 3, vertical semiaxis 2.
~~~

**Part B — Surface in space, classified from sections first.**

For $4x^2+y^2=z^2$, start by fixing $z=c$:

$$
4x^2+y^2=c^2.
$$

If $c\ne0$, divide by $c^2$:

$$
\frac{x^2}{c^2/4}+\frac{y^2}{c^2}=1.
$$

The section is an ellipse in the horizontal plane $z=c$, centered on the $z$-axis, with semiaxis $|c|/2$ along $x$ and $|c|$ along $y$. Thus the horizontal extent along $y$ is twice that along $x$. At $c=0$, $4x^2+y^2=0$ forces $x=y=0$, so the section is a single point at the origin.

Next, in the vertical plane $x=0$:

$$
y^2=z^2\quad\Longrightarrow\quad y=z\ \text{or}\ y=-z.
$$

In the vertical plane $y=0$:

$$
4x^2=z^2\quad\Longrightarrow\quad z=2x\ \text{or}\ z=-2x.
$$

Both vertical sections are pairs of crossing straight lines through the origin, but the slopes differ because the $x$ direction is compressed by a factor of $2$ in horizontal slices. The horizontal ellipses expand in proportion to $|z|$ both above and below $z=0$.

Only after these observations do we identify the surface as a **double elliptic cone** with vertex at $(0,0,0)$ and symmetry axis $Oz$.

Qualitative vertical-profile sketches (not to scale):

~~~text
Surface viewed in yz-plane      Surface viewed in xz-plane
          z                              z
          ^                              ^
         / \                            / \
        /   \                          /   \
       /     \                        /     \
----------*---------- y      ---------*-------- x
       \     /                        \     /
        \   /                          \   /
         \ /                            \ /

At z=c: horizontal ellipse, x-radius |c|/2, y-radius |c|.
~~~

## 4. Verification and Consistency Checks
For Part A, the major vertex $(4,-2)$ satisfies the canonical equation:

$$
\frac{(4-1)^2}{9}+\frac{(-2+2)^2}{4}=\frac99+0=1.
$$

In the original equation, its value is $4(16)+9(4)-8(4)+36(-2)+4=64+36-32-72+4=0$. At the center $(1,-2)$, the original left-hand side is $-36$, consistent with the equivalent equation $4(x-1)^2+9(y+2)^2-36=0$.

For Part B, at $z=2$ the horizontal section is $4x^2+y^2=4$. The points $(1,0,2)$ and $(0,2,2)$ satisfy it and verify the unequal semiaxes: $1$ along $x$ and $2$ along $y$. At $z=0$, only $(0,0,0)$ satisfies the equation. The same structure occurs for $z=-2$ because only $z^2$ appears.

## 5. Final Answer
The first equation is the ellipse $\frac{(x-1)^2}{9}+\frac{(y+2)^2}{4}=1$, centered at $(1,-2)$ with semiaxes $3$ and $2$. The second equation is a double elliptic cone; at height $z=c\ne0$, its cross-section has semiaxes $|c|/2$ along $x$ and $|c|$ along $y$, shrinking to the vertex at $c=0$.
