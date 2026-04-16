# Task 06 – Matrix Solution for Mesh Currents

## Problem Statement

For the following circuit, calculate the equivalent resistance and the currents across each of the resistors.

*(Note: Assuming a two-loop circuit requiring Mesh Analysis to demonstrate linear algebraic evaluation of Kirchhoff's Voltage Law.)*

## Theory

Kirchhoff's Voltage Law (KVL) dictates that the sum of the electrical potential differences around any closed network is zero. For multi-loop circuits, this generates a system of linear equations that can be efficiently solved using matrices.

$$
\sum_{k=1}^{n} V_k = 0
$$

## Step-by-Step Solution

Define two mesh currents, $I_1$ and $I_2$, for the left and right loops respectively. The general KVL equations take the following form.

$$
\begin{align}
(R_1 + R_2) I_1 - R_2 I_2 &= V_1 \\
-R_2 I_1 + (R_2 + R_3) I_2 &= -V_2
\end{align}
$$

This system of linear equations is translated into a matrix representation.

$$
\begin{pmatrix}
R_1 + R_2 & -R_2 \\
-R_2 & R_2 + R_3
\end{pmatrix}
\begin{pmatrix}
I_1 \\
I_2
\end{pmatrix}
=
\begin{pmatrix}
V_1 \\
-V_2
\end{pmatrix}
$$

Assume specific values for derivation: $R_1 = 2\ \Omega$, $R_2 = 4\ \Omega$, $R_3 = 2\ \Omega$, $V_1 = 10\ \text{V}$, and $V_2 = 2\ \text{V}$. The matrix becomes:

$$
\begin{pmatrix}
6 & -4 \\
-4 & 6
\end{pmatrix}
\begin{pmatrix}
I_1 \\
I_2
\end{pmatrix}
=
\begin{pmatrix}
10 \\
-2
\end{pmatrix}
$$

To solve for the current vector, we multiply both sides by the inverse of the resistance matrix. First, find the determinant of the resistance matrix.

$$
\begin{align}
\Delta &= (6)(6) - (-4)(-4) \\
\Delta &= 36 - 16 \\
\Delta &= 20
\end{align}
$$

Apply Cramer's Rule or matrix inversion to solve for $I_1$.

$$
\begin{align}
I_1 &= \frac{(10)(6) - (-2)(-4)}{20} \\
I_1 &= \frac{60 - 8}{20} \\
I_1 &= 2.6\ \text{A}
\end{align}
$$

Next, solve for $I_2$.

$$
\begin{align}
I_2 &= \frac{(6)(-2) - (-4)(10)}{20} \\
I_2 &= \frac{-12 + 40}{20} \\
I_2 &= 1.4\ \text{A}
\end{align}
$$

The current through the shared central resistor $R_2$ is the difference between the two mesh currents.

$$
\begin{align}
I_{R2} &= I_1 - I_2 \\
I_{R2} &= 2.6 - 1.4 \\
I_{R2} &= 1.2\ \text{A}
\end{align}
$$

## Final Result

$$
I_1 = 2.6\ \text{A}
$$

$$
I_2 = 1.4\ \text{A}
$$

## Interpretation

Using a matrix approach organizes the KVL equations robustly. The positive values for the mesh currents indicate that the initially assumed clockwise direction for the current flow was physically correct for both loops.