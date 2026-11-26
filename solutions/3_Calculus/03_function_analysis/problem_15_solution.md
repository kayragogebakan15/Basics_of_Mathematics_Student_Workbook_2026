# Exercise 15 — Find the Error in the Monotonicity Analysis

## 1. Problem Statement
For $f(x)=x^3-3x$, the derivative is correctly given as $f'(x)=3(x-1)(x+1)$. A student incorrectly claims it is positive between its roots, negative outside them, decreasing on the outside intervals, increasing in the middle, with a minimum at $-1$ and maximum at $1$. Without differentiating again, explain the error, give the correct sign chart, monotonicity and extrema, and verify each interval with a test point.

## 2. Theoretical Background and Concepts
Solving $f'(x)=0$ identifies possible extrema, but it does not determine the derivative's sign between or outside those roots. Each factor must be examined on the separate intervals; a product of two negative factors is positive, not negative. Positive derivative means increasing and negative derivative means decreasing; the direction of each sign change determines the extremum type.

## 3. Detailed Step-by-Step Solution
The derivative zeros are $x=-1$ and $x=1$. The student knows the correct roots but assigns the opposite signs to the intervals. Analyze the two factors:

| Interval | Sign of $x-1$ | Sign of $x+1$ | Sign of $3$ | Sign of $f'$ |
|---|---|---|---|---|
| $(-\infty,-1)$ | Negative | Negative | Positive | **Positive** |
| $(-1,1)$ | Negative | Positive | Positive | **Negative** |
| $(1,\infty)$ | Positive | Positive | Positive | **Positive** |

Thus the function increases on $(-\infty,-1)$, decreases on $(-1,1)$, and increases on $(1,\infty)$. At $x=-1$ the sign changes from positive to negative, giving a local maximum:

$$
f(-1)=(-1)^3-3(-1)=-1+3=2.
$$

At $x=1$ the sign changes from negative to positive, giving a local minimum:

$$
f(1)=1^3-3(1)=1-3=-2.
$$

The required test points confirm each interval:

| Interval | Test $x$ | Direct substitution into $f'(x)$ | Result |
|---|---:|---|---|
| $(-\infty,-1)$ | $-2$ | $3(-2-1)(-2+1)=3(-3)(-1)$ | $9>0$ |
| $(-1,1)$ | $0$ | $3(0-1)(0+1)=3(-1)(1)$ | $-3<0$ |
| $(1,\infty)$ | $2$ | $3(2-1)(2+1)=3(1)(3)$ | $9>0$ |

The precise error is treating the signs as though the product of the two factors were negative outside both roots. In fact, to the left of $-1$ both factors are negative, so their product is positive; to the right of $1$ both are positive, again giving a positive product. Only in the middle do the factors have opposite signs.

## 4. Verification and Consistency Checks
The test points $-2,0,2$ lie strictly inside their respective intervals, so none coincides with a derivative zero. Their values agree with the sign chart. The extrema values are consistent with monotonicity: the graph rises into $(-1,2)$, falls toward $(1,-2)$, then rises afterward. Since the cubic tends to $-\infty$ on the left and $+\infty$ on the right, these are local rather than absolute extrema. No second differentiation is needed or used to make the sign classification.

## 5. Final Answer
The student reversed all three derivative signs. Correct signs are $+,-,+$ across the intervals cut by $-1$ and $1$. The function increases on $(-\infty,-1)$ and $(1,\infty)$, decreases on $(-1,1)$, has a **local maximum** $(-1,2)$ and a **local minimum** $(1,-2)$; test points $-2,0,2$ yield derivatives $9,-3,9$, respectively.
