# Task 03 – Equivalent Resistance of a 10 Ohm Circuit

## Problem Statement

Calculate the equivalent resistance for the circuit shown in the figure. All resistors have a resistance of $10\ \Omega$.

*(Note: Assuming a pure parallel topology of three resistors to demonstrate current division extremes.)*

## Theory

For $n$ identical resistors of resistance $R$ connected in parallel, the equivalent resistance formula simplifies significantly. 

$$
\frac{1}{R_\text{eq}} = \frac{n}{R}
$$

## Step-by-Step Solution

State the general parallel resistance formula for three components.

$$
\frac{1}{R_\text{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}
$$

Since $R_1 = R_2 = R_3 = R$, the equation simplifies.

$$
\begin{align}
\frac{1}{R_\text{eq}} &= \frac{3}{R} \\
R_\text{eq} &= \frac{R}{3}
\end{align}
$$

Substitute the given value of $10\ \Omega$.

$$
R_\text{eq} = \frac{10}{3}
$$

## Final Result

$$
R_\text{eq} \approx 3.33\ \Omega
$$

## Interpretation

In a purely parallel configuration of identical resistors, the total resistance scales inversely with the number of branches. The current is distributed perfectly equally among the three branches.