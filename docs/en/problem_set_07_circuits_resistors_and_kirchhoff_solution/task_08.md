# Task 08 – Current in a Multi-Source Loop

## Problem Statement

Calculate the current flowing through the ammeter.

*(Note: Assuming a single-loop circuit containing two opposing voltage sources, $V_1 = 15\ \text{V}$ and $V_2 = 5\ \text{V}$, and two series resistors, $R_1 = 2\ \Omega$ and $R_2 = 3\ \Omega$.)*

## Theory

Kirchhoff's Voltage Law (KVL) states that the algebraic sum of all voltages around a closed loop must equal zero. When voltage sources are in opposition, the net electromotive force is the difference between their magnitudes.

$$
\sum V_\text{rises} = \sum V_\text{drops}
$$

## Step-by-Step Solution

Establish the KVL equation for the single loop, assuming a current direction driven by the larger voltage source ($V_1$).

$$
V_1 - V_2 - I R_1 - I R_2 = 0
$$

Rearrange the equation to solve for the current $I$.

$$
\begin{align}
I(R_1 + R_2) &= V_1 - V_2 \\
I &= \frac{V_1 - V_2}{R_1 + R_2}
\end{align}
$$

Substitute the known circuit parameters into the equation.

$$
\begin{align}
I &= \frac{15 - 5}{2 + 3} \\
I &= \frac{10}{5} \\
I &= 2\ \text{A}
\end{align}
$$

## Final Result

$$
I = 2\ \text{A}
$$

## Interpretation

The opposing voltage source $V_2$ acts as a load, reducing the net potential available to drive current through the resistors. The ammeter records a steady-state current determined by the net voltage and the total series resistance.