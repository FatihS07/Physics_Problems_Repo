# Task 02 – Copernicus's Model

## Problem Statement

Implement the heliocentric motion of Earth and Mars. Determine the relative position of Mars as seen from Earth and identify the moments of retrograde motion. Compare this model to the epicyclic model.

## Theory

In the Copernican model, planets move in circular orbits around the Sun. Let $\vec{r}_Z$ be the position of Earth and $\vec{r}_M$ be the position of Mars.

$$
\vec{r}_Z(t) = R_Z \begin{pmatrix} \cos(\omega_Z t) \\ \sin(\omega_Z t) \end{pmatrix}
$$

$$
\vec{r}_M(t) = R_M \begin{pmatrix} \cos(\omega_M t) \\ \sin(\omega_M t) \end{pmatrix}
$$

Where $R_M > R_Z$ and $\omega_Z > \omega_M$ (Keplerian implication).

## Step-by-Step Solution

### 1. Relative Position

The position of Mars relative to Earth (geocentric vector) is:

$$
\vec{r}_{M/Z}(t) = \vec{r}_M(t) - \vec{r}_Z(t)
$$

$$
\vec{r}_{M/Z}(t) = \begin{pmatrix} R_M \cos(\omega_M t) - R_Z \cos(\omega_Z t) \\ R_M \sin(\omega_M t) - R_Z \sin(\omega_Z t) \end{pmatrix}
$$

### 2. Identifying Retrograde Motion

Retrograde motion occurs when the angular velocity of the relative vector $\vec{r}_{M/Z}$ becomes negative. Let $\Delta \theta = (\omega_Z - \omega_M)t$. By transforming the frame such that Earth's position is momentarily subtracted, we find that the condition for the start/end of retrograde motion is:

$$
\cos(\Delta \theta) = \frac{R_Z \omega_Z + R_M \omega_M}{R_Z \omega_M + R_M \omega_Z}
$$

Since $R \propto \omega^{-2/3}$ from Kepler's laws, and for Mars $R_M > R_Z$, we can solve for the specific time intervals $\Delta \theta$ where the planet appears to move backward.

### 3. Comparison with Ptolemy

If we define:
- $R = R_M$
- $r = R_Z$
- $\omega = \omega_M$
- $\Omega = \omega_Z$

The vector equation for $\vec{r}_{M/Z}$ becomes:

$$
\vec{r}_{M/Z}(t) = \begin{pmatrix} R \cos(\omega t) - r \cos(\Omega t) \\ R \sin(\omega t) - r \sin(\Omega t) \end{pmatrix}
$$

This is mathematically equivalent to a Ptolemaic model where the planet moves on an epicycle with radius equal to Earth's orbital radius, but the direction of rotation is adjusted.

## Final Result

The relative trajectory of Mars relative to Earth is:

$$
\vec{r}_{M/Z}(t) = \begin{pmatrix} R_M \cos(\omega_M t) - R_Z \cos(\omega_Z t) \\ R_M \sin(\omega_M t) - R_Z \sin(\omega_Z t) \end{pmatrix}
$$

## Interpretation

The Copernican model explains retrograde motion as an observational effect. It occurs when Earth "overtakes" the outer planet. This simplifies the system by removing the need for physical epicycles, replacing them with the actual motion of the observer (Earth).