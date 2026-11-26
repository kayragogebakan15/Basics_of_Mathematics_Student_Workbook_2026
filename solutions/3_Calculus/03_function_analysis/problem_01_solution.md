# Exercise 1 — A Cubic Polynomial

## 1. Problem Statement
Analyze the monotonicity and extrema of $f(x)=x^3-3x^2+2$. Sketch the graph and mark its critical points.

## 2. Theoretical Background and Concepts
A differentiable function increases where $f'>0$ and decreases where $f'<0$. An interior critical point with a derivative sign change from positive to negative is a local maximum; a change from negative to positive is a local minimum. A polynomial is continuous and differentiable on all real numbers.

## 3. Detailed Step-by-Step Solution
The domain is all real numbers. Differentiate and factor:

$$
f'(x)=3x^2-6x=3x(x-2).
$$

The critical numbers satisfy $3x(x-2)=0$, so $x=0$ and $x=2$. Check factor signs on the three intervals:

| Interval | Sign of $x$ | Sign of $x-2$ | Sign of $f'$ | Behavior |
|---|---|---|---|---|
| $(-\infty,0)$ | Negative | Negative | Positive | Increasing |
| $(0,2)$ | Positive | Negative | Negative | Decreasing |
| $(2,\infty)$ | Positive | Positive | Positive | Increasing |

At $x=0$, the derivative changes from positive to negative, giving a local maximum:

$$
f(0)=2.
$$

At $x=2$, it changes from negative to positive, giving a local minimum:

$$
f(2)=8-12+2=-2.
$$

For a more accurately located sketch, note that $f(1)=0$ and

$$
f(x)=(x-1)(x^2-2x-2),
$$

so the three horizontal-axis intercepts are $x=1-\sqrt3$, $x=1$, and $x=1+\sqrt3$. The positive leading cubic term implies $f(x)\to-\infty$ to the far left and $f(x)\to+\infty$ to the far right.

Qualitative shape (not to scale; critical points are labeled):

~~~text
Plot window: x in [-1.8, 3.7], y in [-4, 4].
O = marked feature; * = sampled function curve.
+ = origin when visible; vertical | and horizontal - = axes.
                    |                                 **
                    |                                 *
                    |                                **
                    |                                *
                    |                                *
                ****O****                           *
              ***   |   ***                        **
             **     |     ***                      *
            **      |       ***                   **
-----------**-------+---------**-----------------**----------
           *        |          ***              **
          *         |            ***           **
         **         |              ***        **
         *          |                *********
        **          |                    O
        *           |
       **           |
       *            |
       *            |
~~~

The sampled curve rises to the marked maximum O at (0,2), falls to the marked minimum O at (2,-2), then rises. Its three zeros are x=1-sqrt(3), 1, and 1+sqrt(3).

The shape rises to $(0,2)$, falls to $(2,-2)$, then rises again. The schematic spacing is not a coordinate scale.

## 4. Verification and Consistency Checks
Test $x=-1,1,3$: $f'(-1)=3(-1)(-3)=9>0$, $f'(1)=3(1)(-1)=-3<0$, and $f'(3)=3(3)(1)=9>0$. These confirm both slope directions. The second derivative $f''(x)=6x-6$ is negative at $0$ and positive at $2$, independently confirming the local maximum and minimum. Because the cubic is unbounded above and below, these extrema are local, not absolute.

## 5. Final Answer
Increasing on $(-\infty,0)$ and $(2,\infty)$, decreasing on $(0,2)$; local maximum $(0,2)$ and local minimum $(2,-2)$.
