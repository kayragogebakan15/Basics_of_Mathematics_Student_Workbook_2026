# Exercise 14 — Cone and Cylinder

## 1. Problem Statement
Compare $x^2+y^2=z^2$ and $x^2+y^2=4$. For each, describe sections $z=c$, $x=0$ and $y=0$, sketch the surface, and explain why the horizontal radius changes with height only for the first equation.

## 2. Theoretical Background and Concepts
For a horizontal section, $x^2+y^2=R^2$ is a circle with radius $R$. A double cone has radius proportional to the absolute height, so it contracts to a point at its vertex. A circular cylinder has constant horizontal radius and extends unchanged along its axis. A vertical section is obtained by setting one horizontal coordinate to zero.

## 3. Detailed Step-by-Step Solution
**Surface A: $x^2+y^2=z^2$.**

At $z=c$, we obtain $x^2+y^2=c^2$, a circle of radius $R=|c|$ for $c\ne0$; at $c=0$, the cross-section is the single point $(0,0,0)$. At $x=0$:

$$
y^2=z^2\quad\Longrightarrow\quad y=z\quad\mathrm{or}\quady=-z.
$$

These are two crossing straight lines in the plane $x=0$. At $y=0$:

$$
x^2=z^2\quad\Longrightarrow\quad x=z\quad\mathrm{or}\quadx=-z.
$$

Again, two crossing straight lines. Rotating this pair of lines about the $z$-axis generates two nappes meeting at the origin: a double circular cone.

**Surface B: $x^2+y^2=4$.**

At any $z=c$, the section remains $x^2+y^2=4$, a circle of radius $2$. At $x=0$:

$$
y^2=4\quad\Longrightarrow\quad y=2\quad\mathrm{or}\quady=-2.
$$

These are two parallel vertical lines in the $yz$-plane. At $y=0$:

$$
x^2=4\quad\Longrightarrow\quad x=2\quad\mathrm{or}\quadx=-2.
$$

These are two parallel vertical lines in the $xz$-plane. Thus the surface is an infinite circular cylinder of radius $2$ around the $z$-axis.

Qualitative vertical-profile sketches (not to scale):

~~~text
Double cone                     Cylinder
      z                             z
      ^                             ^
     / \                           | |
    /   \                          | |
   /     \                         | |
      *  vertex                    | |
   \     /                         | |
    \   /                          | |
     \ /                           | |

R(z)=|z|                         R(z)=2
~~~

## 4. Verification and Consistency Checks
For the cone, at $z=3$ the point $(3,0,3)$ satisfies $9=9$ and the radius is $3$; at $z=0$ only the origin remains. For the cylinder, $(2,0,3)$ and $(2,0,-7)$ both satisfy $x^2+y^2=4$, confirming that its cross-section is independent of $z$. The cone's $z^2$ term makes its radius depend on $|z|$, whereas $z$ does not occur in the cylinder equation.

## 5. Final Answer
The first surface is a double circular cone with horizontal radius $|z|$; the second is a circular cylinder with constant horizontal radius $2$.
