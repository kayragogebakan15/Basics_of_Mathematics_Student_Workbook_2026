# Exercise 7 — Linear Dependence Without Heavy Computation

## 1. Problem Statement
Given
$$u=(1,2,3),\qquad v=(2,4,6),\qquad w=(0,1,1).$$
Identify a specific relation between $u$ and $v$, decide whether the three vectors can be linearly independent, and explain why no long calculation is needed.

## 2. Method and Key Formula
A set of vectors is linearly dependent if there are scalars, not all zero, whose linear combination equals the zero vector. In particular, if one vector is a scalar multiple of another, any set containing both is dependent.

## 3. Detailed Step-by-Step Solution
Compare the components:
$$2u=2(1,2,3)=(2,4,6)=v.$$
Thus,
$$v-2u=(0,0,0).$$
This is a nontrivial linear relation: the coefficients of $u,v,w$ can be chosen as $-2,1,0$, which are not all zero.

## 4. Verification and Consistency Checks
The equality $v=2u$ holds in all three components: $2=2(1)$, $4=2(2)$, and $6=2(3)$. Therefore, the set is dependent regardless of the third vector $w$; adding another vector cannot remove an existing dependence relation.

## 5. Final Answer
$$\boxed{v=2u\quad\Longrightarrow\quad \{u,v,w\}\text{ is linearly dependent.}}$$