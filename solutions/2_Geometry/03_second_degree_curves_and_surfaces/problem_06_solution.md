# Exercise 6 — Shifted Ellipse

## 1. Problem Statement
Reduce $4x^2+9y^2-16x+18y-11=0$ to canonical form, find its center and semiaxis lengths, and check the value of the original expression at the center.

## 2. Theoretical Background and Concepts
Completing the square rewrites $u^2+2au=(u+a)^2-a^2$. For an ellipse in standard form $\frac{(x-h)^2}{a^2}+\frac{(y-k)^2}{b^2}=1$, the center is $(h,k)$ and the semiaxes are $a,b>0$.

## 3. Detailed Step-by-Step Solution
Group like terms and factor the quadratic coefficients:

$$
4(x^2-4x)+9(y^2+2y)=11.
$$

Complete each square, keeping the corrections outside the parentheses:

$$
4((x-2)^2-4)+9((y+1)^2-1)=11.
$$

Expand only the constant terms, then move them to the right:

$$
4(x-2)^2+9(y+1)^2-16-9=11,
$$

$$
4(x-2)^2+9(y+1)^2=36.
$$

Divide by $36$:

$$
\frac{(x-2)^2}{9}+\frac{(y+1)^2}{4}=1.
$$

The center is $C=(2,-1)$; the horizontal semiaxis is $3$ and the vertical semiaxis is $2$. The major-axis endpoints are $(-1,-1)$ and $(5,-1)$; the minor-axis endpoints are $(2,-3)$ and $(2,1)$.

Qualitative sketch (not to scale):

~~~text
              y
           (2,1)
         .---|---.
(-1,-1) *---C-----* (5,-1)  --> x
         '---|---'
           (2,-3)

C = (2,-1)
~~~

## 4. Verification and Consistency Checks
Substitute the center into the original left-hand side:

$$
4(2)^2+9(-1)^2-16(2)+18(-1)-11
=16+9-32-18-11=-36.
$$

This is consistent with the canonical equation: at the center, both squares vanish and $4(x-2)^2+9(y+1)^2-36=-36$, not zero. The center is inside the ellipse, not on its boundary. As a boundary check, $(5,-1)$ gives $4(25)+9-80-18-11=0$ and canonical value $9/9=1$.

## 5. Final Answer
The ellipse is $\frac{(x-2)^2}{9}+\frac{(y+1)^2}{4}=1$, centered at $(2,-1)$, with horizontal semiaxis $3$ and vertical semiaxis $2$.
