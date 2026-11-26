# Exercise 12 — A Function with an Absolute Value

## 1. Problem Statement
Analyze $f(x)=|x^2-4|$. Begin with the parabola $y=x^2-4$, explain the reflection caused by absolute value, identify the points where the derivative does not exist, and justify this geometrically.

## 2. Theoretical Background and Concepts
For any real number $u$, $|u|=u$ if $u\ge0$ and $|u|=-u$ if $u<0$. The absolute value retains the part of the graph above the $x$-axis and reflects the negative part across that axis. At a zero where the original curve crosses the axis with nonzero slope, this folding creates a corner whose left and right derivatives disagree.

## 3. Detailed Step-by-Step Solution
Start with $q(x)=x^2-4$, an upward-opening parabola with vertex $(0,-4)$ and zeros at $x=-2$ and $x=2$. Its negative part is the interval $(-2,2)$. Applying absolute value reflects precisely this central portion upward:

$$
f(x)=|x^2-4|=
\begin{cases}
x^2-4,&x<-2,\\
4-x^2,&-2\le x\le2,\\
x^2-4,&x>2.
\end{cases}
$$

The function is continuous everywhere. Its derivative away from $\pm2$ is

$$
f'(x)=
\begin{cases}
2x,&x<-2,\\
-2x,&-2<x<2,\\
2x,&x>2.
\end{cases}
$$

At $x=-2$, the left derivative is $\lim_{x\to-2^-}2x=-4$, whereas the right derivative is $\lim_{x\to-2^+}(-2x)=4$. The two slopes differ, so the derivative does not exist there. At $x=2$, the left slope is $-2(2)=-4$ and the right slope is $2(2)=4$. Again, the derivative does not exist. More precisely these one-sided derivatives follow from the difference quotient because $f$ is continuous and each side follows a differentiable polynomial extending to the endpoint.

Signs of $f'$ give decreasing behavior on $(-\infty,-2)$, increasing on $(-2,0)$, decreasing on $(0,2)$, and increasing on $(2,\infty)$. Therefore $(-2,0)$ and $(2,0)$ are global minima; $(0,4)$ is a local maximum (not global, since $f(x)\to\infty$ as $|x|\to\infty$).

A qualitative sketch (not to scale, symmetric about the vertical axis):

~~~text
Plot window: x in [-3.4, 3.4], y in [-1, 8].
O = marked feature; * = sampled function curve.
+ = origin when visible; vertical | and horizontal - = axes.
                              |
*                             |                             *
 *                            |                            *
 **                           |                           **
  *                           |                           *
   *                          |                          *
   **                         |                         **
    **                        |                        **
     *                    ****O****                    *
      *                ***    |    ****               *
      **            ***       |       ***            **
       **         ***         |         ***         **
        **       **           |           **       **
         **    ***            |            ***    **
          **  **              |              **  **
           ****               |               ****
------------O*----------------+----------------*O------------
                              |
                              |
~~~

The three marked O points are corners/minima (-2,0) and (2,0) and the smooth central local maximum (0,4). Both outer branches rise away from the corners; the reflected middle arc bends downward.

The two sharp joining points on the horizontal axis are the nondifferentiable corners. The middle reflected arc is an inverted parabola rising from $(-2,0)$ to $(0,4)$ and falling back to $(2,0)$; the outer arms are upward-opening parabola portions.

## 4. Verification and Consistency Checks
At $x=0$, $f(0)=|-4|=4$, matching the reflected vertex. At $x=\pm2$, $f(\pm2)=|4-4|=0$. At $x=3$, $f(3)=|9-4|=5$, confirming the outer part is unchanged. The left/right slopes at both joining points differ by $8$, verifying corners rather than smooth minima. Although $f$ is continuous at both, differentiability fails there.

## 5. Final Answer
The graph is the parabola $x^2-4$ with its negative middle arc reflected upward. Nondifferentiable points are $x=-2$ and $x=2$, both global minima of value $0$. The central local maximum is $(0,4)$.
