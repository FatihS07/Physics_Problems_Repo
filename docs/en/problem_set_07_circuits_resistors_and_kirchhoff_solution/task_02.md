# Task 02 – Equivalent Resistance of a 3 Ohm Circuit

## Problem Statement

Calculate the equivalent resistance for the circuit shown in the figure. All resistors have a resistance of $3\ \Omega$.

*(Note: Assuming a topology where $R_1$ and $R_2$ are in series, and this entire branch is in parallel with $R_3$.)*

## Theory

The equivalent resistance of a circuit depends on identifying discrete series and parallel branches. The series branches must be simplified first before applying the parallel formula.

$$
R_\text{series} = \sum_{i=1}^{n} R_i
$$

## Step-by-Step Solution

First, find the resistance of the branch containing $R_1$ and $R_2$ in series.

$$
\begin{align}
R_{12} &= R_1 + R_2 \\
R_{12} &= 3 + 3 \\
R_{12} &= 6\ \Omega
\end{align}
$$

Next, treat $R_{12}$ as a single resistor in parallel with $R_3$.

$$
\frac{1}{R_\text{eq}} = \frac{1}{R_{12}} + \frac{1}{R_3}
$$

Isolate the equivalent resistance $R_\text{eq}$.

$$
R_\text{eq} = \frac{R_{12} R_3}{R_{12} + R_3}
$$

Substitute the known values into the expression.

$$
\begin{align}
R_\text{eq} &= \frac{6 \cdot 3}{6 + 3} \\
R_\text{eq} &= \frac{18}{9}
\end{align}
$$

## Final Result

$$
R_\text{eq} = 2\ \Omega
$$

## Interpretation

Placing a larger resistance branch in parallel with a smaller resistance branch yields an equivalent resistance that is strictly smaller than the smallest individual branch. The $3\ \Omega$ resistor dominates the current flow path.