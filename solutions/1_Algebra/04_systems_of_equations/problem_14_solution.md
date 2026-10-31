# Exercise 14 — A Small Change in the Right-Hand Side

## 1. Problem Statement
Compare the systems
$$\begin{cases}x+y=2,\\2x-y=1,\\3x=3\end{cases}
\qquad\text{and}\qquad
\begin{cases}x+y=2,\\2x-y=1,\\3x=3.1.\end{cases}$$
Check the consistency of each system and explain why a small change in one number can change the type of the system.

## 2. Method and Key Formula
First solve the first two equations. Then test whether the resulting values satisfy the third equation. A system is consistent only if one pair $(x,y)$ satisfies every equation.

## 3. Detailed Step-by-Step Solution
From the first two equations,
$$x+y=2,\qquad 2x-y=1.$$
Add them:
$$3x=3\quad\Longrightarrow\quad x=1.$$
Then $y=2-1=1$.

**First system:** The third equation is $3x=3$, which is satisfied by $x=1$. Therefore the first system is consistent and has the unique solution $(1,1)$.

**Second system:** The third equation is $3x=3.1$. But the first two equations force $x=1$, so they force $3x=3$, not $3.1$. The second system is inconsistent.

## 4. Verification and Consistency Checks
For $(1,1)$, the first two equations give $1+1=2$ and $2(1)-1=1$. The third equation of the first system gives $3(1)=3$. In the second system it would require $3=3.1$, a contradiction.

The third equation of the first system is exactly the sum of the first two. Changing its right-hand side from $3$ to $3.1$ breaks that dependency and makes the equations incompatible.

## 5. Final Answer
- First system: $\boxed{(x,y)=(1,1)}$ — one solution.
- Second system: $\boxed{\text{no solution}}$ — inconsistent.