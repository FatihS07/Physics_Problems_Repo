# Task 01 – Equivalent Resistance of a 5 Ohm Circuit

## Problem Statement

Calculate the equivalent resistance for the circuit shown in the figure. All resistors have a resistance of $5\ \Omega$.

*(Note: Assuming a topology where $R_1$ is in series with a parallel combination of $R_2$ and $R_3$.)*

## Theory

For resistors in series, the equivalent resistance is the algebraic sum of the individual resistances.

$$
R_\text{series} = R_1 + R_2 + \dots + R_n
$$

For resistors in parallel, the reciprocal of the equivalent resistance is the sum of the reciprocals.

$$
\frac{1}{R_\text{parallel}} = \frac{1}{R_1} + \frac{1}{R_2} + \dots + \frac{1}{R_n}
$$

## Step-by-Step Solution

First, compute the equivalent resistance of the parallel section containing $R_2$ and $R_3$.

$$
\begin{align}
\frac{1}{R_{23}} &= \frac{1}{R_2} + \frac{1}{R_3} \\
R_{23} &= \frac{R_2 R_3}{R_2 + R_3}
\end{align}
$$

Substitute the given resistance value of $5\ \Omega$ into the equation.

$$
\begin{align}
R_{23} &= \frac{5 \cdot 5}{5 + 5} \\
R_{23} &= \frac{25}{10} \\
R_{23} &= 2.5\ \Omega
\end{align}
$$

Next, add the series resistance $R_1$ to the parallel equivalent.

$$
R_\text{eq} = R_1 + R_{23}
$$

Substitute the known values.

$$
\begin{align}
R_\text{eq} &= 5 + 2.5 \\
R_\text{eq} &= 7.5\ \Omega
\end{align}
$$

## Final Result

$$
R_\text{eq} = 7.5\ \Omega
$$

## Interpretation

The total equivalent resistance is less than the sum of all three individual resistors. This occurs because the parallel branch provides multiple pathways for charge flow, effectively decreasing the overall opposition to the current in that section.