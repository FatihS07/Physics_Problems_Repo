# Task 02 – Velocity selection (crossed fields)

## Problem Statement

A system uses crossed electric $\vec E = (0,E,0)$ and magnetic $\vec B = (0,0,B)$ fields to select particles. Determine the condition for rectilinear motion, calculate the selected velocity $v_d$ for $E = 400\ \mathrm{V/m}$ and $B = 0.8\ \mathrm{T}$, check for kinetic energy changes, and interpret the operating principle.

## Theory

A charged particle moving through a region with both electric and magnetic fields experiences the full Lorentz force:

$$
\vec F = q(\vec E + \vec v \times \vec B)
$$

For the particle to move in a straight line with constant velocity (rectilinear motion), the net force acting on it must be zero. 

## Step-by-Step Solution

Set the net force to zero for rectilinear motion:

$$
q(\vec E + \vec v \times \vec B) = 0
$$

$$
\vec E = -(\vec v \times \vec B)
$$

Assuming the particle enters the selector along the $x$-axis, its velocity is $\vec v = (v_x, 0, 0)$. Calculate the cross product:

$$
\begin{align}
\vec v \times \vec B &= 
\begin{pmatrix}
v_x \\
0 \\
0
\end{pmatrix}
\times
\begin{pmatrix}
0 \\
0 \\
B
\end{pmatrix} \\
&=
\begin{pmatrix}
0 \\
-v_x B \\
0
\end{pmatrix}
\end{align}
$$

Substitute this back into the force balance equation:

$$
\begin{pmatrix}
0 \\
E \\
0
\end{pmatrix}
=
-
\begin{pmatrix}
0 \\
-v_x B \\
0
\end{pmatrix}
$$

$$
E = v_x B
$$

Solve for the drift velocity $v_d = v_x$:

$$
v_d = \frac{E}{B}
$$

Calculate the numerical value of $v_d$ using $E = 400\ \mathrm{V/m}$ and $B = 0.8\ \mathrm{T}$:

$$
v_d = \frac{400}{0.8}
$$

$$
v_d = 500\ \mathrm{m/s}
$$

Examine the kinetic energy change. In steady, rectilinear motion, the velocity is strictly constant in both magnitude and direction. 

$$
\Delta K = \frac{1}{2} m v_{final}^2 - \frac{1}{2} m v_{initial}^2 = 0
$$

## Final Result

1. The condition for rectilinear motion is $v_x = E / B$.
2. The selected velocity is $v_d = 500\ \mathrm{m/s}$.
3. The kinetic energy does not change in steady motion.

## Interpretation

The velocity selector balances the electric force (which is independent of velocity) against the magnetic force (which is proportional to velocity). Only particles traveling at the exact speed $v = E/B$ experience a net force of zero and pass through undeflected, regardless of their mass or charge.