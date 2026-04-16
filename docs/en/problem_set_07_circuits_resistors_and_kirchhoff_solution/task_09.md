# Task 09 – Ammeter Current via Current Division

## Problem Statement

Calculate the current flowing through the ammeter.

*(Note: Assuming a circuit where a known total current $I_\text{in} = 5\ \text{A}$ enters a parallel junction consisting of $R_1 = 4\ \Omega$ and $R_2 = 1\ \Omega$. The ammeter is located in series with $R_1$.)*

## Theory

For a parallel circuit consisting of two branches, the current divider rule provides a direct method to calculate the current in one branch without needing to determine the node voltage first.

$$
I_x = I_\text{total} \frac{R_\text{other}}{R_x + R_\text{other}}
$$

## Step-by-Step Solution

State the current divider formula specifically for the branch containing $R_1$.

$$
I_1 = I_\text{in} \frac{R_2}{R_1 + R_2}
$$

Substitute the given resistance and current values into the expression.

$$
\begin{align}
I_1 &= 5 \cdot \frac{1}{4 + 1} \\
I_1 &= 5 \cdot \frac{1}{5} \\
I_1 &= 1\ \text{A}
\end{align}
$$

Verify the result by calculating the current through the second branch.

$$
\begin{align}
I_2 &= I_\text{in} \frac{R_1}{R_1 + R_2} \\
I_2 &= 5 \cdot \frac{4}{5} \\
I_2 &= 4\ \text{A}
\end{align}
$$

Confirm that KCL is satisfied at the input node.

$$
I_1 + I_2 = 1 + 4 = 5\ \text{A}
$$

## Final Result

$$
I_A = 1\ \text{A}
$$

## Interpretation

The ammeter reading is consistent with the principle of least resistance. The branch with four times the resistance draws exactly one quarter of the current drawn by the lower-resistance branch.