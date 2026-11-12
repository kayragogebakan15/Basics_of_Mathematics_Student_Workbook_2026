# Exercise 9 — Ellipsoid and Its Cross-Sections

## 1. Problem Statement
For $\frac{x^2}{9}+\frac{y^2}{4}+\frac{z^2}{16}=1$, give the semiaxis lengths, describe the section $z=0$, and analyze the family of sections $z=c$ for $|c|<4$.

## 2. Theoretical Background and Concepts
An ellipsoid with positive squared-coordinate terms is the 3D analogue of an ellipse. Its semiaxes are the square roots of the denominators. A horizontal section is found by substituting $z=c$; the sign of the resulting right-hand side determines whether the section is an ellipse, a point, or empty.

## 3. Detailed Step-by-Step Solution
The semiaxes are $a_x=\sqrt9=3$, $a_y=\sqrt4=2$, and $a_z=\sqrt{16}=4$, all centered at the origin. The longest is vertical, along $z$.

At $z=0$:

$$
\frac{x^2}{9}+\frac{y^2}{4}=1.
$$

This is an ellipse with semiaxes $3$ (along $x$) and $2$ (along $y$). For a general horizontal section $z=c$:

$$
\frac{x^2}{9}+\frac{y^2}{4}=1-\frac{c^2}{16}=k.
$$

When $|c|<4$, $k>0$ and dividing by $k$ gives

$$
\frac{x^2}{9k}+\frac{y^2}{4k}=1.
$$

Consequently the section semiaxes are

$$
a_x(c)=3\sqrt{1-\frac{c^2}{16}},\qquad
a_y(c)=2\sqrt{1-\frac{c^2}{16}}.
$$

Both shrink as $|c|$ increases toward $4$; their ratio remains $3:2$. At $c=0$ the section is widest; at $c=\pm4$ it reduces to the point $(0,0,\pm4)$; for $|c|>4$ no real section exists.

Qualitative side-view sketch (not to scale):

~~~text
               z
               ^
            (0,0,4)
               *
            .-' '-.
          .'   |   '.
z=0  ----(-----+-----)----> x
          '.   |   .'
            '-.-'
               *
            (0,0,-4)

Horizontal slices are ellipses, widest at z=0.
~~~

## 4. Verification and Consistency Checks
At $z=0$, $(3,0,0)$ and $(0,2,0)$ both satisfy the surface equation. For $c=2$, $k=1-4/16=3/4$, giving horizontal semiaxis $3\sqrt3/2$ and vertical-in-slice semiaxis $\sqrt3$. At $c=4$, the equation becomes $x^2/9+y^2/4=0$, forcing $x=y=0$.

## 5. Final Answer
The ellipsoid semiaxes are $(3,2,4)$ along $(x,y,z)$. Its horizontal slices are ellipses with semiaxes $3\sqrt{1-c^2/16}$ and $2\sqrt{1-c^2/16}$ for $|c|<4$.
