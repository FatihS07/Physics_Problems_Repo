# Task 07 – Simple pendulum: measurement of $g$

## Problem Statement

Determine $g$ using a simple pendulum: $g=4\pi^2 \frac{L}{T^2}$.

## Theory

Using the total differential for $g(L, T)$:

$$
u(g) = \sqrt{ \left( \frac{4\pi^2}{T^2} u(L) \right)^2 + \left( -\frac{8\pi^2 L}{T^3} u(T) \right)^2 }
$$

## Step-by-Step Solution

1.  Measure $L$ and calculate $\bar{T}$ from multiple periods.
2.  Calculate nominal $g$.
3.  Calculate partial derivatives for uncertainty contributions.
4.  Determine percentage contributions: $C_L = \frac{u_L(g)^2}{u(g)^2}$ and $C_T = \frac{u_T(g)^2}{u(g)^2}$.

## Final Result

(Result provided in the format $g = \hat{g} \pm u(g)$ by the HTML application.)

## Interpretation

The uncertainty in $T$ usually contributes more to $u(g)$ because $T$ is squared in the denominator, making $g$ highly sensitive to timing errors.