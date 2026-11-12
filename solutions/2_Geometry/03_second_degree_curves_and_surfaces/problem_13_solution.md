# Exercise 13 — Intersection of a Sphere and a Plane

## 1. Problem Statement
Intersect the sphere $x^2+y^2+z^2=25$ with the plane $z=3$. Find the intersection equation and its radius, then classify the sections $z=c$ for all real $c$.

## 2. Theoretical Background and Concepts
A sphere centered at the origin with radius $5$ has equation $x^2+y^2+z^2=25$. Fixing the height $z=c$ gives a horizontal section. The resulting squared radius must be nonnegative for real points to exist.

## 3. Detailed Step-by-Step Solution
Substitute $z=3$ into the sphere equation:

$$
x^2+y^2+3^2=25
\quad\Longrightarrow\quad
x^2+y^2=25-9=16.
$$

The intersection is a circle in the plane $z=3$ with center $(0,0,3)$ and radius $R=\sqrt{16}=4$. Its points are exactly

$$
(x,y,z)=(4\cos t,4\sin t,3),\qquad 0\le t<2\pi.
$$

For arbitrary height $z=c$, substitute:

$$
x^2+y^2=25-c^2.
$$

The possibilities are:
- If $|c|<5$, the section is a circle centered at $(0,0,c)$ with radius $\sqrt{25-c^2}$.
- If $c=\pm5$, the section is one point, $(0,0,\pm5)$.
- If $|c|>5$, no real points exist because $25-c^2<0$.

Qualitative side-profile sketch (not to scale):

~~~text
            z
            ^
          (0,0,5)
             *
          .-' '-.
 z=3  ---*-------*---    section radius 4
        /    |    \
 z=0  *----- + -----*   section radius 5
        \    |    /
          '-._.-'
             *
          (0,0,-5)
~~~

## 4. Verification and Consistency Checks
The point $(4,0,3)$ belongs to both surfaces because $4^2+0+3^2=16+9=25$ and $z=3$. The parametrization satisfies the sphere since $16(\cos^2t+\sin^2t)+9=25$. At $c=0$, the section radius $5$ equals the sphere's maximum radius, which is consistent with symmetry.

## 5. Final Answer
At $z=3$, the intersection is $x^2+y^2=16$ in the plane $z=3$, a circle of radius $4$. In general its radius is $\sqrt{25-c^2}$ for $|c|<5$, with point sections at $\pm5$ and no sections outside.
