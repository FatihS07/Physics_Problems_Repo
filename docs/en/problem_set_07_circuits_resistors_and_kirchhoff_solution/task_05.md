# Task 05 – Equivalent Resistance and Branch Current

## Problem Statement

For the following circuit, calculate the equivalent resistance and the current flowing through ammeter A.

*(Note: Assuming a $24\text{ V}$ source driving a circuit where $R_1 = 4\ \Omega$ is in series with a parallel pair $R_2 = 6\ \Omega$ and $R_3 = 12\ \Omega$. The ammeter is situated in the branch containing $R_3$.)*

## Theory

The total equivalent resistance of a mixed circuit is found by sequentially simplifying parallel and series sub-circuits. Ohm's Law relates the voltage drop across any component to the current flowing through it.

$$
V = I R
$$

For a parallel two-resistor branch, the equivalent resistance is the product over the sum.

$$
R_\text{parallel} = \frac{R_a R_b}{R_a + R_b}
$$

## Step-by-Step Solution

First, determine the equivalent resistance of the parallel section containing $R_2$ and $R_3$.

$$
\begin{align}
R_{23} &= \frac{R_2 R_3}{R_2 + R_3} \\
R_{23} &= \frac{6 \cdot 12}{6 + 12} \\
R_{23} &= \frac{72}{18} \\
R_{23} &= 4\ \Omega
\end{align}
$$

Next, calculate the total equivalent resistance of the entire circuit by adding the series resistor $R_1$.

$$
\begin{align}
R_\text{eq} &= R_1 + R_{23} \\
R_\text{eq} &= 4 + 4 \\
R_\text{eq} &= 8\ \Omega
\end{align}
$$

Determine the total current supplied by the voltage source.

$$
\begin{align}
I_\text{total} &= \frac{V}{R_\text{eq}} \\
I_\text{total} &= \frac{24}{8} \\
I_\text{total} &= 3\ \text{A}
\end{align}
$$

Calculate the voltage drop across the parallel branch. This is the voltage available to push current through $R_2$ and $R_3$.

$$
\begin{align}
V_{23} &= I_\text{total} R_{23} \\
V_{23} &= 3 \cdot 4 \\
V_{23} &= 12\ \text{V}
\end{align}
$$

Finally, calculate the current flowing through the branch with ammeter A, which is the branch containing $R_3$.

$$
\begin{align}
I_A &= \frac{V_{23}}{R_3} \\
I_A &= \frac{12}{12} \\
I_A &= 1\ \text{A}
\end{align}
$$

## Final Result

$$
R_\text{eq} = 8\ \Omega
$$

$$
I_A = 1\ \text{A}
$$

## Interpretation

The total equivalent resistance dictates the overall current drawn from the source. The initial series resistor causes a voltage drop, leaving the remaining voltage strictly across the parallel branches. The ammeter measures only the localized current through its specific branch, which is a fraction of the total current determined by the inverse ratio of the parallel resistances.