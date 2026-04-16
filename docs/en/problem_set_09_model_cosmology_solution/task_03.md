# Task 03 – Comparison of Models

## Problem Statement

Evaluate the epicyclic and heliocentric models by fitting parameters, comparing the complexity of both descriptions, and determining which model is more economical.

## Theory

The quality of a scientific model is often judged by Occam's Razor: the simplest explanation that fits the data is usually the best. In cosmology, this relates to the number of independent parameters required to predict planetary positions.

## Step-by-Step Solution

### 1. Parameter Counting

In the **Ptolemaic (Epicyclic) Model**, each planet requires:
* The radius of the deferent ($R$).
* The radius of the epicycle ($r$).
* The angular velocity of the deferent ($\omega$).
* The angular velocity of the epicycle ($\Omega$).
* Initial phases for both circles ($\phi_R, \phi_r$).

In the **Copernican (Heliocentric) Model**, the motion of two planets (e.g., Earth and Mars) requires:
* Orbital radius of Earth ($R_Z$) and Mars ($R_M$).
* Angular velocity of Earth ($\omega_Z$) and Mars ($\omega_M$).
* Initial phases ($\phi_Z, \phi_M$).

### 2. Economy of Description

While the math for a single planet looks similar, the heliocentric model becomes more economical as more planets are added. In the geocentric model, Earth's own motion must be "replicated" as a separate epicycle for every single planet. In the heliocentric model, Earth's parameters are measured once and remain constant for all observations.

## Final Result

The heliocentric model is more economical because it identifies a common cause (Earth's motion) for the retrograde loops observed in all external planets, whereas the epicyclic model treats each planet's loop as an independent parameter.

## Interpretation

The shift from epicycles to heliocentrism represents a move from **curve-fitting** (describing *how* it looks) to **physical modeling** (describing *what* is happening).