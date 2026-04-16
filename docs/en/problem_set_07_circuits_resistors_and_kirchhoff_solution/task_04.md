# Task 04 – Voltage and Current Across R3

## Problem Statement

Calculate the voltage across resistor $R_3$ and the current flowing through this resistor.

*(Note: Assuming a $12\text{ V}$ source driving a circuit where $R_1 = 4\ \Omega$ is in series with a parallel pair $R_2 = 6\ \Omega$ and $R_3 = 3\ \Omega$.)*

## Theory

Ohm's Law relates voltage, current, and resistance.

$$
V = I R
$$

Kirchhoff's Current Law (KCL) dictates that the total current entering a parallel junction splits according to the inverse ratio of the resistances.

## Step-by-Step Solution

First, determine the equivalent resistance of the parallel pair $R_2$ and $R_3$.

$$
\begin{align}
R_{23} &= \frac{R_2 R_3}{R_2 + R_3} \\
R_{23} &= \frac{6 \cdot 3}{6 + 3} \\
R_{23} &= 2\ \Omega
\end{align}
$$

Determine the total equivalent resistance of the circuit.

$$
\begin{align}
R_\text{eq} &= R_1 + R_{23} \\
R_\text{eq} &= 4 + 2 \\
R_\text{eq} &= 6\ \Omega
\end{align}
$$

Calculate the total current leaving the voltage source.

$$
\begin{align}
I_\text{total} &= \frac{V}{R_\text{eq}} \\
I_\text{total} &= \frac{12}{6} \\
I_\text{total} &= 2\ \text{A}
\end{align}
$$

The voltage across the parallel branch is the total current multiplied by the parallel equivalent resistance.

$$
\begin{align}
V_{23} &= I_\text{total} R_{23} \\
V_{23} &= 2 \cdot 2 \\
V_{23} &= 4\ \text{V}
\end{align}
$$

Because $R_3$ is in this parallel branch, the voltage across it is exactly $V_{23}$. The current through $R_3$ is found via Ohm's Law.

$$
\begin{align}
I_3 &= \frac{V_{23}}{R_3} \\
I_3 &= \frac{4}{3}\ \text{A}
\end{align}
$$

## Final Result

$$
V_3 = 4\ \text{V}
$$

$$
I_3 = 1.33\ \text{A}
$$

## Interpretation

The parallel configuration ensures that the voltage across $R_2$ and $R_3$ remains identical. However, because $R_3$ has a lower resistance than $R_2$, it permits a proportionally larger fraction of the total current to flow through its branch.