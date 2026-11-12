# Exercise 11 — Two Similar Surfaces

## 1. Problem Statement
Compare the surfaces $x^2+y^2-z^2=1$ and $x^2+y^2-z^2=-1$. Examine horizontal cross-sections $z=c$ for several values, determine their radii or absence, and use those sections to describe and sketch both shapes.

## 2. Theoretical Background and Concepts
At a fixed height $z=c$, an equation of the form $x^2+y^2=R^2$ describes a circle of radius $R$ if $R^2>0$, a single point if $R^2=0$, and no real points if $R^2<0$. Reading how $R$ changes with height identifies whether a surface is connected or split into components.

## 3. Detailed Step-by-Step Solution
**Surface A: $x^2+y^2-z^2=1$.** Substitute $z=c$:

$$
x^2+y^2=1+c^2,\qquad R_A(c)=\sqrt{1+c^2}.
$$

Because $1+c^2\ge1$ for every real $c$, each horizontal section is a circle, and the minimum radius is $R_A(0)=1$. Examples:

| Height $c$ | $R_A(c)$ | Section |
|---|---|---|
| $0$ | $1$ | Circle |
| $\pm1$ | $\sqrt2$ | Circle |
| $\pm2$ | $\sqrt5$ | Circle |

The surface narrows to a circular waist at $z=0$ and widens upward and downward without splitting. It is a **hyperboloid of one sheet**.

**Surface B: $x^2+y^2-z^2=-1$.** Substitute $z=c$:

$$
x^2+y^2=c^2-1.
$$

If $|c|>1$, the section is a circle of radius $R_B(c)=\sqrt{c^2-1}$. If $|c|=1$, it is a single point $(0,0,c)$. If $|c|<1$, the right side is negative and there is no real section.

| Height $c$ | Section |
|---|---|
| $0$ | No real points |
| $\pm1$ | Single point of radius $0$ |
| $\pm2$ | Circle of radius $\sqrt3$ |

The surface consists of two disconnected parts, one beginning at $(0,0,1)$ and expanding upward and the other beginning at $(0,0,-1)$ and expanding downward. It is a **hyperboloid of two sheets**.

Qualitative vertical-profile sketches (not to scale; left/right edges indicate rotational surfaces):

~~~text
One sheet                     Two sheets
       z                            z
     \   /                        \   /
      \ /                          \ /
      | |                           *   z=1
      | |                         (gap)
      / \                           *   z=-1
     /   \                         / \
   waist at z=0                   /   \
                               no points for |z|<1
~~~

## 4. Verification and Consistency Checks
For A at $z=0$, $(1,0,0)$ satisfies $1=1$. At $z=2$, $(\sqrt5,0,2)$ gives $5-4=1$. For B at $z=1$, $(0,0,1)$ gives $-1=-1$. At $z=2$, $(\sqrt3,0,2)$ gives $3-4=-1$. At $z=0$, B would require $x^2+y^2=-1$, which is impossible over the real numbers.

## 5. Final Answer
$x^2+y^2-z^2=1$ is a connected one-sheet hyperboloid with radius $\sqrt{1+c^2}$ at height $c$. The equation $x^2+y^2-z^2=-1$ gives a two-sheet hyperboloid with sections only for $|c|\ge1$ (radius $\sqrt{c^2-1}$ when $|c|>1$).
