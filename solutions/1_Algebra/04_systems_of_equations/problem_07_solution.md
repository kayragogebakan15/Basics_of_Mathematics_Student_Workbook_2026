# Exercise 7 — Choosing a Method Deliberately

## 1. Problem Statement
Choose the method that best uses the structure in each situation and justify the choice:
1. A triangular system $2x-y=3$, $4y=8$.
2. Three systems $Ax=b_i$ with the same invertible matrix $A$, when $A^{-1}$ is already known.
3. One $3\times3$ system for which the inverse is not given and the goal is only one solution vector.
Carry out case 1 completely. For cases 2 and 3, describe the plan and indicate reusable or unnecessary calculations.

## 2. Method and Key Formula
Use back-substitution for triangular systems. If $A^{-1}$ is already known, use $x_i=A^{-1}b_i$ for each right-hand side. For a single system where only a solution is needed, Gaussian elimination generally avoids the extra work of computing an entire inverse.

## 3. Detailed Step-by-Step Solution
**Case 1: triangular system.** The second equation gives
$$4y=8\quad\Longrightarrow\quad y=2.$$
Substitute into the first:
$$2x-2=3\quad\Longrightarrow\quad 2x=5\quad\Longrightarrow\quad x=\frac52.$$
Thus $(x,y)=(\frac52,2)$.

**Case 2: three right-hand sides and known inverse.** Reuse the given inverse and calculate
$$x_1=A^{-1}b_1,\qquad x_2=A^{-1}b_2,\qquad x_3=A^{-1}b_3.$$
There is no need to compute $A^{-1}$ again. The same matrix-vector multiplication procedure is used three times.

**Case 3: one system, inverse not given.** Form $[A\mid b]$ and use Gaussian elimination. This directly finds the required solution and avoids computing all entries of $A^{-1}$ when they are not needed.

## 4. Verification and Consistency Checks
For case 1, substitute:
$$2\left(\frac52\right)-2=5-2=3,\qquad 4(2)=8.$$
Both equations hold. The choices in cases 2 and 3 follow from whether the inverse is already available and whether it will be reused.

## 5. Final Answer
- Case 1: back-substitution, with $(x,y)=(\frac52,2)$.
- Case 2: reuse the known inverse for each right-hand side.
- Case 3: use Gaussian elimination rather than computing an unnecessary inverse.