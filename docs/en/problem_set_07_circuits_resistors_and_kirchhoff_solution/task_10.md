# Task 10 – Ammeter Current via Thevenin Equivalence

## Problem Statement

Calculate the current flowing through the ammeter.

*(Note: Assuming a complex linear network that has been reduced to its Thevenin equivalent connected to the ammeter branch. Thevenin voltage $V_\text{th} = 12\ \text{V}$, Thevenin resistance $R_\text{th} = 4\ \Omega$, and the ammeter branch has a load resistance $R_L = 2\ \Omega$.)*

## Theory

Thevenin's Theorem states that any linear electrical network containing independent sources and resistances can be replaced at terminals A-B by an equivalent voltage source $V_\text{th}$ in series with an equivalent resistance $R_\text{th}$.

$$
I_L = \frac{V_\text{th}}{R_\text{th} + R_L}
$$

## Step-by-Step Solution

Define the parameters of the simplified equivalent circuit. The load branch containing the ammeter acts as the termination for the Thevenin equivalent circuit.

Substitute the equivalent values into the series current equation.

$$
\begin{align}
I_L &= \frac{12}{4 + 2} \\
I_L &= \frac{12}{6} \\
I_L &= 2\ \text{A}
\end{align}
$$

If a matrix formulation of the original multi-node circuit was required to find the Thevenin parameters, it would take the following form before simplification.

$$
\begin{pmatrix}
G_{11} & -G_{12} \\
-G_{21} & G_{22}
\end{pmatrix}
\begin{pmatrix}
V_1 \\
V_2
\end{pmatrix}
=
\begin{pmatrix}
I_{s1} \\
I_{s2}
\end{pmatrix}
$$

Given the pre-calculated Thevenin parameters, no matrix inversion is necessary for the final load current.

## Final Result

$$
I_A = 2\ \text{A}
$$

## Interpretation

By reducing the surrounding circuit topology to a single voltage source and series resistor, the effect of the entire network on the ammeter branch is easily evaluated. The current is strictly limited by the sum of the network's internal Thevenin resistance and the branch's localized resistance.