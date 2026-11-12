# Exercise 8 — Sphere

## 1. Problem Statement
Reduce $x^2+y^2+z^2-4x+2y-6z-2=0$ to canonical form, find the center and radius, and verify two points of the sphere.

## 2. Theoretical Background and Concepts
The sphere with center $(h,k,l)$ and radius $r>0$ satisfies $(x-h)^2+(y-k)^2+(z-l)^2=r^2$. Completing the square separately in all three coordinates reveals these quantities.

## 3. Detailed Step-by-Step Solution
Collect the terms involving each coordinate and move the constant:

$$
(x^2-4x)+(y^2+2y)+(z^2-6z)=2.
$$

Complete the three squares, adding $4$, $1$, and $9$ on both sides:

$$
(x^2-4x+4)+(y^2+2y+1)+(z^2-6z+9)=2+4+1+9.
$$

Therefore

$$
(x-2)^2+(y+1)^2+(z-3)^2=16.
$$

Thus the center is $C=(2,-1,3)$ and the radius is $r=4$. Choose points by moving $4$ units along coordinate axes: $A=(6,-1,3)$ and $B=(2,3,3)$.

## 4. Verification and Consistency Checks
At $A$, canonical form yields $(6-2)^2+0+0=16$. The original polynomial gives

$$
36+1+9-4(6)+2(-1)-6(3)-2=46-24-2-18-2=0.
$$

At $B$, canonical form yields $0+(3+1)^2+0=16$. The original gives

$$
4+9+9-4(2)+2(3)-6(3)-2=22-8+6-18-2=0.
$$

The center itself gives zero distance and therefore lies inside the sphere, not on its surface.

## 5. Final Answer
The sphere is $(x-2)^2+(y+1)^2+(z-3)^2=16$, centered at $(2,-1,3)$ with radius $4$.
