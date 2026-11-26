# Exercise 14 — Reconstructing Information from the Derivative

## 1. Problem Statement
Given $f'(x)=(x-1)(x+2)$, determine where $f$ increases or decreases and the positions and nature of its extrema. Sketch a possible qualitative graph. Then verify that $g(x)=x^3/3+x^2/2-2x$ has this derivative and compare its graph with the qualitative analysis.

## 2. Theoretical Background and Concepts
The derivative's zeros divide the real line into sign intervals. Positive derivative means increasing; negative derivative means decreasing. Changing from positive to negative produces a local maximum, while changing from negative to positive produces a local minimum. Any two differentiable functions on a connected interval with the same derivative differ only by a constant.

## 3. Detailed Step-by-Step Solution
The critical numbers come from

$$
(x-1)(x+2)=0\quad\Longrightarrow\quad x\in\{-2,1\}.
$$

Use signs of each factor:

| Interval | $x-1$ | $x+2$ | $f'$ | Behavior |
|---|---|---|---|---|
| $(-\infty,-2)$ | Negative | Negative | Positive | Increasing |
| $(-2,1)$ | Negative | Positive | Negative | Decreasing |
| $(1,\infty)$ | Positive | Positive | Positive | Increasing |

Thus the function rises to a local maximum at $x=-2$, then falls to a local minimum at $x=1$, then rises again. No vertical positions are fixed by the derivative alone: shifting the entire graph up or down preserves these slopes and extrema abscissas.

A qualitative sketch (not to scale) must rise on the far left, turn down at the left critical point, and turn up again at the right critical point:

~~~text
Plot window: x in [-4, 3.5], y in [-4, 5].
O = marked feature; * = sampled function curve.
+ = origin when visible; vertical | and horizontal - = axes.
                                |                     *
                                |                    *
                                |                    *
              **O**             |                   *
           ****   ****          |                  **
          **          **        |                  *
         **             **      |                 **
        *                 **    |                **
       **                  ***  |               **
      **                     ***|              **
-----**------------------------***------------**-------------
     *                          |***        ***
    *                           |   ****O****
   **                           |
   *                            |
  **                            |
  *                             |
 **                             |
 *                              |
~~~

The two O marks identify g's local maximum (-2,10/3) and local minimum (1,-7/6); a possible f has this same curve translated vertically by an arbitrary constant.

Now differentiate the proposed example:

$$
\begin{aligned}
g'(x)
&=\frac13(3x^2)+\frac12(2x)-2\\
&=x^2+x-2\\
&=(x-1)(x+2),
\end{aligned}
$$

which agrees exactly with the supplied derivative. Compute its extrema values:

$$
\begin{aligned}
g(-2)&=\frac{-8}{3}+\frac{4}{2}-2(-2)
=-\frac83+2+4=\frac{10}{3},\\
g(1)&=\frac13+\frac12-2
=\frac{2+3-12}{6}=-\frac76.
\end{aligned}
$$

The specific maximum is $(-2,10/3)$ and minimum $(1,-7/6)$. Since all antiderivatives of the same derivative on $\mathbb R$ differ by a constant, any $f$ satisfying the premise has the form $f(x)=g(x)+C$ for some real constant $C$; its extrema values differ from those of $g$ by $C$, but the shape and critical abscissas are unchanged.

## 4. Verification and Consistency Checks
Test $f'(-3)=(-4)(-1)=4>0$, $f'(0)=(-1)(2)=-2<0$, and $f'(2)=(1)(4)=4>0$. These confirm the full sign pattern. Independently, $g''(x)=2x+1$, so $g''(-2)=-3<0$ and $g''(1)=3>0$, confirming the maximum and minimum. The two derivative expressions are identical for all real $x$, not merely at the critical points.

## 5. Final Answer
Every such $f$ increases on $(-\infty,-2)$ and $(1,\infty)$ and decreases on $(-2,1)$, with a local maximum at $x=-2$ and minimum at $x=1$. The specified $g$ has extrema $(-2,10/3)$ and $(1,-7/6)$, and all other possible graphs are vertical translates $g+C$.
