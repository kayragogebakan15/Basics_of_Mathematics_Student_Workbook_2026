# Exercise 1 — Vector Operations and Their Meaning

## 1. Problem Statement
For $u=(2,-1,3)$ and $v=(-1,4,2)$ compute
$$u+v,\qquad u-v,\qquad 3u-2v.$$
Then verify that $(u+v)-v=u$, and explain geometrically what adding two vectors means.

## 2. Method and Key Formula
Vectors in $\mathbb R^3$ are added and subtracted component by component:
$$(a_1,a_2,a_3)\pm(b_1,b_2,b_3)=(a_1\pm b_1,a_2\pm b_2,a_3\pm b_3).$$
Scalar multiplication multiplies every component by the scalar. Geometrically, vector addition follows the head-to-tail rule: place the tail of the second vector at the head of the first; the resultant runs from the first tail to the final head.

## 3. Detailed Step-by-Step Solution
First add corresponding components:
$$u+v=(2+(-1),-1+4,3+2)=(1,3,5).$$
Subtract component by component:
$$u-v=(2-(-1),-1-4,3-2)=(3,-5,1).$$
For the linear combination, calculate the scalar multiples first:
$$3u=(6,-3,9),\qquad 2v=(-2,8,4).$$
Therefore,
$$3u-2v=(6-(-2),-3-8,9-4)=(8,-11,5).$$

## 4. Verification and Consistency Checks
Using the sum already calculated,
$$(u+v)-v=(1,3,5)-(-1,4,2)=(2,-1,3)=u.$$
This confirms the required identity component by component.

## 5. Final Answer
$$\boxed{u+v=(1,3,5),\quad u-v=(3,-5,1),\quad 3u-2v=(8,-11,5).}$$
Vector addition combines displacements according to the head-to-tail rule; the resultant represents the net displacement.