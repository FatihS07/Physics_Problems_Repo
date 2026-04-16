# Task 03 – Magnetic moment of a loop

## Problem Statement

A conducting loop with $N$ turns, area $S$, and current $I$ is placed in a uniform magnetic field $\vec B$. Define its magnetic moment, determine the torque, find the angle for maximum torque, determine the potential energy, and identify stable/unstable positions.

## Theory

A current-carrying loop acts as a magnetic dipole. The magnetic dipole moment $\vec \mu$ depends on the current, area, and number of turns. 

When placed in an external magnetic field, a torque $\vec M$ acts on the dipole, attempting to align the magnetic moment with the field. The potential energy $U$ of the dipole depends on its orientation relative to the field.

## Step-by-Step Solution

Define the magnetic moment:

$$
\vec \mu = N I S \hat{n}
$$

Here, $\hat{n}$ is the unit vector normal to the surface of the loop, determined by the right-hand rule based on the direction of current flow.

Determine the torque $\vec M$ acting on the loop:

$$
\vec M = \vec \mu \times \vec B
$$

The magnitude of the torque is:

$$
|\vec M| = \mu B \sin\theta
$$

where $\theta$ is the angle between $\vec \mu$ and $\vec B$.

Determine the angle for maximum torque. The sine function reaches its maximum absolute value at $90^\circ$ and $270^\circ$:

$$
\sin\theta = 1 \implies \theta = 90^\circ = \frac{\pi}{2}\ \mathrm{rad}
$$

Determine the potential energy $U$ of the magnetic dipole in the external field:

$$
U = -\vec \mu \cdot \vec B
$$

$$
U = -\mu B \cos\theta
$$

Identify stable and unstable equilibrium positions. Equilibrium occurs when the torque is zero, which happens at $\theta = 0^\circ$ and $\theta = 180^\circ$. 

For $\theta = 0^\circ$:

$$
U(0^\circ) = -\mu B \cos(0^\circ) = -\mu B
$$

This is the minimum potential energy state.

For $\theta = 180^\circ$:

$$
U(180^\circ) = -\mu B \cos(180^\circ) = +\mu B
$$

This is the maximum potential energy state.

## Final Result

1. Magnetic moment: $\vec \mu = N I S \hat{n}$.
2. Torque: $\vec M = \vec \mu \times \vec B$.
3. Maximum torque occurs at $\theta = 90^\circ$.
4. Potential energy: $U = -\vec \mu \cdot \vec B$.
5. Stable position is at $\theta = 0^\circ$ (aligned). Unstable position is at $\theta = 180^\circ$ (anti-aligned).

## Interpretation

The loop behaves analogously to a compass needle. The magnetic field exerts a torque that attempts to rotate the loop so that its magnetic moment aligns with the external field, minimizing the potential energy of the system.