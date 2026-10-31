# Exercise 13 — Does Every Equation Add New Information?

## 1. Problem Statement
Consider
$$x_1+x_2=10,\qquad x_2+x_3=8,\qquad x_1-x_3=2.$$
Solve the system and check whether all three equations are independently necessary to describe the solution set. If one follows from the others, show this by calculation.

## 2. Method and Key Formula
Use the first two equations to express $x_1$ and $x_2$ in terms of one free variable. Then test whether the third equation follows by adding or subtracting the first two equations.

## 3. Detailed Step-by-Step Solution
Let $x_3=t$. From the second equation,
$$x_2=8-t.$$
Substitute into the first:
$$x_1+(8-t)=10\quad\Longrightarrow\quad x_1=2+t.$$
Thus the solutions determined by the first two equations are
$$(x_1,x_2,x_3)=(2+t,8-t,t).$$
Now subtract the second equation from the first:
$$(x_1+x_2)-(x_2+x_3)=10-8,$$
which simplifies to
$$x_1-x_3=2.$$
This is exactly the third equation.

## 4. Verification and Consistency Checks
Substitute the parametric solution:
$$x_1+x_2=(2+t)+(8-t)=10,$$
$$x_2+x_3=(8-t)+t=8,$$
$$x_1-x_3=(2+t)-t=2.$$
All three hold, but the third is a consequence of the first two and is therefore redundant.

## 5. Final Answer
$$\boxed{(x_1,x_2,x_3)=(2+t,8-t,t),\quad t\in\mathbb R.}$$
The third equation is redundant because it equals equation 1 minus equation 2.