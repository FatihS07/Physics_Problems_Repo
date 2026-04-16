# Task 07 – Equivalent Resistance and Node Potential

## Problem Statement

For the following circuit, calculate the equivalent resistance and the potential difference between points A and B.

*(Note: Assuming a circuit driven by a $20\ \text{V}$ source, consisting of a series resistor $R_1 = 5\ \Omega$ connected to a parallel combination of $R_2 = 10\ \Omega$ and $R_3 = 10\ \Omega$. Points A and B are located across the parallel branches.)*

## Theory

The potential difference across a specific section of a circuit depends on the current flowing through that section and its equivalent resistance. For a series-parallel combination, the circuit must be simplified sequentially.

$$
R_\text{parallel} = \left( \sum_{i=1}^{n} \frac{1}{R_i} \right)^{-1}
$$

$$
V_{AB} = I_\text{total} R_{AB}
$$

## Step-by-Step Solution

First, determine the equivalent resistance of the parallel section between nodes A and B.

$$
\begin{align}
\frac{1}{R_{AB}} &= \frac{1}{R_2} + \frac{1}{R_3} \\
\frac{1}{R_{AB}} &= \frac{1}{10} + \frac{1}{10} \\
\frac{1}{R_{AB}} &= \frac{2}{10}
\end{align}
$$

Invert the result to find $R_{AB}$.

$$
R_{AB} = 5\ \Omega
$$

Next, calculate the total equivalent resistance of the circuit.

$$
\begin{align}
R_\text{eq} &= R_1 + R_{AB} \\
R_\text{eq} &= 5 + 5 \\
R_\text{eq} &= 10\ \Omega
\end{align}
$$

Determine the total current flowing from the source.

$$
\begin{align}
I_\text{total} &= \frac{V_s}{R_\text{eq}} \\
I_\text{total} &= \frac{20}{10} \\
I_\text{total} &= 2\ \text{A}
\end{align}
$$

Finally, calculate the potential difference between points A and B using Ohm's Law for that specific network segment.

$$
\begin{align}
V_{AB} &= I_\text{total} R_{AB} \\
V_{AB} &= 2 \cdot 5 \\
V_{AB} &= 10\ \text{V}
\end{align}
$$

## Final Result

$$
R_\text{eq} = 10\ \Omega
$$

$$
V_{AB} = 10\ \text{V}
$$

## Interpretation

The parallel combination of $R_2$ and $R_3$ yields an equivalent resistance identical to $R_1$. Consequently, the total source voltage is divided equally across the series resistor and the parallel network.