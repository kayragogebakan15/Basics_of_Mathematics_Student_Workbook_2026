# Exercise 2 — Circle by Completing the Square

## 1. Problem Statement
Reduce $x^2+y^2-6x+4y-3=0$ to canonical form. Find the center and radius, and verify two simple points in both the original and canonical equations.

## 2. Theoretical Background and Concepts
Completing the square uses $u^2+2au=(u+a)^2-a^2$. A circle in canonical form $(x-h)^2+(y-k)^2=r^2$ has center $(h,k)$ and radius $r>0$.

## 3. Detailed Step-by-Step Solution
Group terms of the same variable and move the constant:

$$
(x^2-6x)+(y^2+4y)=3.
$$

Complete each square by adding $9$ for the $x$ terms and $4$ for the $y$ terms to both sides:

$$
(x^2-6x+9)+(y^2+4y+4)=3+9+4.
$$

Therefore

$$
(x-3)^2+(y+2)^2=16.
$$

The center is $C=(3,-2)$ and the radius is $r=\sqrt{16}=4$. Choose the simple points $A=(7,-2)$ and $B=(3,2)$ by moving a distance of $4$ horizontally and vertically from the center.

## 4. Verification and Consistency Checks
For $A=(7,-2)$, the original left-hand side is

$$
7^2+(-2)^2-6(7)+4(-2)-3=49+4-42-8-3=0.
$$

In canonical form, $(7-3)^2+(-2+2)^2=16+0=16$.

For $B=(3,2)$, the original left-hand side is

$$
3^2+2^2-6(3)+4(2)-3=9+4-18+8-3=0.
$$

In canonical form, $(3-3)^2+(2+2)^2=0+16=16$. Both descriptions agree at both points.

## 5. Final Answer
The circle is $(x-3)^2+(y+2)^2=16$, with center $(3,-2)$ and radius $4$.
