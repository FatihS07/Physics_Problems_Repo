# Task 08 – Orbit Perturbation and Precession

## Problem Statement

Investigate the effect of a non-Newtonian potential perturbation on the stability of an elliptical orbit.

## Theory

In a pure $1/r$ potential, orbits are closed ellipses (Bertrand's Theorem). If the potential is modified:

$$
U(r) = -\frac{GMm}{r} + \frac{\alpha}{r^2}
$$

The additional $\alpha/r^2$ term breaks the symmetry, and the orbit no longer closes. This leads to the precession of the perihelion.

## Step-by-Step Solution

### 1. Equations of Motion

The radial force is:

$$
F_r = -\frac{dU}{dr} = -\frac{GMm}{r^2} + \frac{2\alpha}{r^3}
$$

### 2. Precession Rate

The angular change between successive perihelia is no longer $2\pi$. The shift $\Delta \phi$ per revolution is approximately:

$$
\Delta \phi \approx \frac{2\pi \alpha}{G M m a (1-e^2)}