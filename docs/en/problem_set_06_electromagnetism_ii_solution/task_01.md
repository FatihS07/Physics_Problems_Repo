# Task 01 – Lorentz force

## Problem Statement

Given the magnetic field $\vec B = (0,0,1)\ \mathrm{T}$, particle velocity $\vec v = (2,3,0)\ \mathrm{m/s}$, and charge $q = 1\ \mathrm{mC}$, determine the Lorentz force, the equation of motion, the force magnitude, whether the force does work, the trajectory radius for $m = 0.01\ \mathrm{kg}$, and the effect of doubling $B$.

## Theory

The magnetic Lorentz force on a moving point charge is given by the cross product:

$$
\vec F = q(\vec v \times \vec B)
$$

According to Newton's second law, the equation of motion is:

$$
m \frac{d\vec v}{dt} = \vec F
$$

For a velocity component perpendicular to a uniform magnetic field, the charge undergoes uniform circular motion where the magnetic force acts as the centripetal force:

$$
\frac{m v_{\perp}^2}{r} = q v_{\perp} B
$$

## Step-by-Step Solution

First, express the given quantities in standard SI units:

$$
q = 10^{-3}\ \mathrm{C}
$$

Calculate the cross product $\vec v \times \vec B$:

$$
\begin{align}
\vec v \times \vec B &= 
\begin{pmatrix}
2 \\
3 \\
0
\end{pmatrix}
\times
\begin{pmatrix}
0 \\
0 \\
1
\end{pmatrix} \\
&= 
\begin{pmatrix}
3\cdot 1 - 0\cdot 0 \\
0\cdot 2 - 2\cdot 1 \\
2\cdot 0 - 3\cdot 0
\end{pmatrix} \\
&=
\begin{pmatrix}
3 \\
-2 \\
0
\end{pmatrix}
\end{align}
$$

Calculate the force $\vec F$:

$$
\vec F = 10^{-3} 
\begin{pmatrix}
3 \\
-2 \\
0
\end{pmatrix}
\ \mathrm{N}
$$

To solve the equation of motion, set up the differential equations:

$$
m \frac{dv_x}{dt} = q v_y B
$$

$$
m \frac{dv_y}{dt} = -q v_x B
$$

$$
m \frac{dv_z}{dt} = 0
$$

This represents coupled harmonic oscillators in the $xy$-plane, leading to uniform circular motion. The initial velocity is entirely in the $xy$-plane, so $v_z = 0$ for all time $t$. 

Calculate the magnitude of the force:

$$
|\vec F| = 10^{-3} \sqrt{3^2 + (-2)^2 + 0^2}
$$

$$
|\vec F| = \sqrt{13} \times 10^{-3}\ \mathrm{N}
$$

Determine the work done by the magnetic force. Work is the dot product of force and displacement:

$$
W = \int \vec F \cdot d\vec r = \int (\vec F \cdot \vec v) dt
$$

Since $\vec F$ is mutually perpendicular to $\vec v$ and $\vec B$, $\vec F \cdot \vec v = 0$. Therefore, work is zero.

Calculate the radius of the trajectory for $m = 0.01\ \mathrm{kg}$:

$$
r = \frac{m v_{\perp}}{q B}
$$

The perpendicular speed is the magnitude of the velocity in the $xy$-plane:

$$
v_{\perp} = \sqrt{2^2 + 3^2} = \sqrt{13}\ \mathrm{m/s}
$$

Substitute the values:

$$
r = \frac{0.01 \cdot \sqrt{13}}{10^{-3} \cdot 1}
$$

$$
r = 10\sqrt{13}\ \mathrm{m}
$$

Analyze the effect of doubling $B$. From the radius formula, $r$ is inversely proportional to $B$. 

## Final Result

1. The force is $\vec F = (3, -2, 0) \times 10^{-3}\ \mathrm{N}$.
2. The motion is uniform circular in the $xy$-plane passing through the origin.
3. The magnitude is $|\vec F| = \sqrt{13} \times 10^{-3}\ \mathrm{N}$.
4. The magnetic force does zero work.
5. The radius is $r = 10\sqrt{13}\ \mathrm{m}$.
6. If $B$ is doubled, the radius $r$ is halved.

## Interpretation

The magnetic force is always perpendicular to the velocity vector. Because of this, it can only change the direction of the velocity, not its magnitude, meaning the kinetic energy remains constant and no work is performed by the static magnetic field.