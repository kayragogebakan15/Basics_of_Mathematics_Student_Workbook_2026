# Exercise 1 — Line Through Two Points

## 1. Problem Statement
Find the line through $A=(1,2)$ and $B=(4,-1)$ in parametric and general form. Identify a direction vector and a normal vector, and verify both points.

## 2. Theoretical Background and Concepts
For distinct points $A,B$ in the plane, $v=B-A$ is a direction vector. A line through $A$ is $X=A+tv$, where $t\in\mathbb R$. A nonzero vector $n$ perpendicular to $v$ determines its general equation $n\cdot(X-A)=0$.

## 3. Detailed Step-by-Step Solution
Subtract the coordinates:

$$
v=B-A=(4-1,-1-2)=(3,-3).
$$

Thus the parametric equation, including its individual coordinates, is

$$
(x,y)=(1,2)+t(3,-3),\qquad x=1+3t,\quad y=2-3t.
$$

Choose $n=(1,1)$ because $n\cdot v=3-3=0$. The general equation follows by taking the dot product with $X-A$:

$$
(1,1)\cdot(x-1,y-2)=0 \quad\Longrightarrow\quad x+y-3=0.
$$

## 4. Verification and Consistency Checks
In parametric form, $t=0$ gives $A=(1,2)$ and $t=1$ gives $B=(4,-1)$. In general form, $1+2-3=0$ and $4-1-3=0$. The normal is perpendicular to the direction because $(1,1)\cdot(3,-3)=0$.

## 5. Final Answer
The line is $(x,y)=(1,2)+t(3,-3)$, equivalently $x+y-3=0$; one direction is $(3,-3)$ and one normal is $(1,1)$.
