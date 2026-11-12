# Exercise 12 — Recognizing a Surface from Cross-Sections

## 1. Problem Statement
Find a simple surface whose $z=0$ section is a point, whose horizontal sections $z>0$ are circles of increasing radius, and whose vertical sections through the $Oz$ axis are parabolas. Justify the choice.

## 2. Theoretical Background and Concepts
A rotationally symmetric surface can be described by an equation depending on $x^2+y^2$, the squared horizontal distance from the $z$-axis. If the height is proportional to this quantity, fixing $z$ gives circles and fixing a vertical plane through the axis gives a parabola.

## 3. Detailed Step-by-Step Solution
Choose the simple equation

$$
z=x^2+y^2.
$$

First, for $z=0$:

$$
x^2+y^2=0.
$$

Since both squares are nonnegative, $x=y=0$. Thus the horizontal cross-section is the single point $(0,0,0)$.

For a horizontal section $z=c>0$, the equation becomes

$$
x^2+y^2=c.
$$

This is a circle centered at $(0,0,c)$ in its horizontal plane with radius

$$
R(c)=\sqrt c.
$$

If $0<c_1<c_2$, then $\sqrt{c_1}<\sqrt{c_2}$, so the radius increases with height. No section exists for $c<0$.

Any vertical plane through the $Oz$ axis can be described using coordinates $s$ along a horizontal unit direction and $z$ vertically:

$$
x=s\cos\theta,\qquad y=s\sin\theta.
$$

Substituting gives

$$
z=s^2\cos^2\theta+s^2\sin^2\theta=s^2.
$$

This is an upward-opening parabola for every angle $\theta$.

Qualitative sketch (not to scale):

~~~text
           z
           ^
         /   \
        /     \
       /       \
      /         \
     *-----------*   circular level
        \     /
         \___/       vertex at origin in vertical profile
          (0,0,0)

Horizontal level sets are circles; vertical meridians are parabolas.
~~~

The diagram schematically combines a bowl-like surface with a horizontal circular level.

## 4. Verification and Consistency Checks
At $z=1$, the horizontal section is $x^2+y^2=1$, radius $1$. At $z=4$, it is $x^2+y^2=4$, radius $2$, confirming growth. In the vertical plane $y=0$, the equation reduces to $z=x^2$; in $x=0$, it reduces to $z=y^2$. Both are parabolas, and the general vertical-plane computation establishes the same fact for all orientations.

## 5. Final Answer
One valid surface is the upward circular paraboloid $z=x^2+y^2$.
