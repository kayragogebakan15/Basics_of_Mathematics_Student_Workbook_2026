# Exercise 7 — A Trigonometric Function

## 1. Problem Statement
On $[0,2\pi]$, find all intervals of monotonicity and extrema of $f(x)=\sin x+\cos x$. Include the endpoints and compare their function values with the interior critical values.

## 2. Theoretical Background and Concepts
On a closed interval, a continuous function attains its absolute maximum and minimum at endpoints or interior critical points. The derivative sign determines increasing and decreasing intervals, and critical points are obtained from $f'=0$. Trigonometric angles are measured in radians.

## 3. Detailed Step-by-Step Solution
Differentiate:

$$
f'(x)=\cos x-\sin x.
$$

Solve $\cos x-\sin x=0$, or $\sin x=\cos x$. On $[0,2\pi]$ this occurs at $x=\pi/4$ and $x=5\pi/4$. The derivative sign is positive on $(0,\pi/4)$, negative on $(\pi/4,5\pi/4)$, and positive on $(5\pi/4,2\pi)$. This can also be read from $f'(x)=\sqrt2\cos(x+\pi/4)$.

| Candidate | Function value |
|---|---|
| $x=0$ | $\sin0+\cos0=1$ |
| $x=\pi/4$ | $\sqrt2/2+\sqrt2/2=\sqrt2$ |
| $x=5\pi/4$ | $-\sqrt2/2-\sqrt2/2=-\sqrt2$ |
| $x=2\pi$ | $\sin2\pi+\cos2\pi=1$ |

The derivative changes from positive to negative at $\pi/4$, giving the absolute and local maximum $\sqrt2$. At $5\pi/4$ it changes from negative to positive, giving the absolute and local minimum $-\sqrt2$.

The endpoint values are both $1$, between the two extreme values. Relative to the one-sided intervals, $x=0$ is an endpoint minimum and $x=2\pi$ an endpoint maximum, but neither beats the interior absolute extrema.

## 4. Verification and Consistency Checks
Sample points give $f'(0)=1>0$, $f'(\pi)=-1<0$, and $f'(3\pi/2)=1>0$, confirming each sign interval. The identity

$$
\sin x+\cos x=\sqrt2\sin(x+\pi/4)
$$

also shows directly that the possible values lie between $-\sqrt2$ and $\sqrt2$ and confirms when those extremes are attained.

## 5. Final Answer
Increasing on $(0,\pi/4)$ and $(5\pi/4,2\pi)$; decreasing on $(\pi/4,5\pi/4)$. Absolute maximum $\sqrt2$ at $x=\pi/4$, absolute minimum $-\sqrt2$ at $x=5\pi/4$; both endpoint values equal $1$.
