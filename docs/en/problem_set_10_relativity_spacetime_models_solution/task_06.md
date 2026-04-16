# Task 06 – Minkowski Diagram (Simulation Model)

## Problem Statement

Design a conceptual Minkowski diagram implemented via Lorentz transformations.

1. Implement the Lorentz matrix.
2. Define the $ct$ and $x$ axes.
3. Define the $ct'$ and $x'$ axes.
4. Mark the light cone.
5. Geometrically interpret dilation and contraction.

## Theory

The Lorentz transformation can be written in matrix form:

$$
\begin{pmatrix}
ct' \\
x'
\end{pmatrix}
=
\begin{pmatrix}
\gamma & -\beta\gamma \\
-\beta\gamma & \gamma
\end{pmatrix}
\begin{pmatrix}
ct \\
x
\end{pmatrix}
$$

where $\beta = v/c$.

## Step-by-Step Solution

### 1. Matrix Implementation

To transform coordinates from the rest frame to the moving frame, we use the inverse transformation or rotate the axes. The angle of the primed axes relative to the unprimed axes is:

$$
\theta = \arctan(\beta)
$$

### 2. Geometry of Axes

- The $ct'$ axis follows the line $x = \beta(ct)$.
- The $x'$ axis follows the line $ct = \beta x$.
- As $v \to c$, both axes "close in" on the $45^\circ$ light cone.

### 3. Light Cone

The light cone is defined by $s^2 = 0$, which implies $x = \pm ct$. These lines are invariant under Lorentz transformations.

## Final Result (Simulation Logic)

The simulation utilizes a slider for $\beta \in [0, 1)$. The rendering engine updates the slopes of the primed axes dynamically.

## Interpretation

Time dilation is seen as the stretching of units along the $ct'$ axis compared to the $ct$ axis. Length contraction is visualized by the intersection of the $x'$ axis with lines of simultaneity in the $S$ frame.