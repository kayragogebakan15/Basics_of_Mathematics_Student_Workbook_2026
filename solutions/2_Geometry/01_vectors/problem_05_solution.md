# Exercise 5 — Angle Between Vectors

## 1. Problem Statement
Given $u=(1,1,0)$ and $v=(1,0,1)$:
1. Use the sign of $u\cdot v$ to predict the type of angle.
2. Compute the angle.
3. Compare the result with the prediction.

## 2. Method and Key Formula
For nonzero vectors, the angle $\theta\in[0,\pi]$ satisfies
$$\cos\theta=\frac{u\cdot v}{\|u\|\,\|v\|}.$$
A positive dot product means an acute angle, a zero dot product means a right angle, and a negative dot product means an obtuse angle.

## 3. Detailed Step-by-Step Solution
First calculate the dot product:
$$u\cdot v=1\cdot1+1\cdot0+0\cdot1=1.$$
Since it is positive, the angle is expected to be acute.

The vector lengths are
$$\|u\|=\sqrt{1^2+1^2+0^2}=\sqrt2,\qquad
\|v\|=\sqrt{1^2+0^2+1^2}=\sqrt2.$$
Therefore,
$$\cos\theta=\frac1{\sqrt2\sqrt2}=\frac12.$$
Hence,
$$\theta=\arccos\left(\frac12\right)=60^\circ=\frac\pi3.$$

## 4. Verification and Consistency Checks
The computed angle $60^\circ$ is between $0^\circ$ and $90^\circ$, so it is acute. This agrees with the positive dot product.

## 5. Final Answer
$$\boxed{\theta=60^\circ=\frac\pi3\text{ radians (acute).}}$$