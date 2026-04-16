# Task 05 – Quantum tunneling

## Problem Statement

A particle with energy $E = 3 \, \mathrm{eV}$ approaches a potential barrier with the following parameters:
* $U_0 = 5 \, \mathrm{eV}$
* $a = 0.5 \, \mathrm{nm}$

1. Explain what can happen.
2. Name a physical phenomenon that utilizes tunneling.

## Theory

In classical mechanics, a particle with $E < U_0$ is always reflected. In quantum mechanics, the wavefunction inside the barrier does not drop to zero but decays exponentially:

$$
\psi(x) \sim e^{-\kappa x}, \quad \kappa = \sqrt{\frac{2m(U_0 - E)}{\hbar^2}}
$$

There is a non-zero probability $T$ (transmission coefficient) that the particle appears on the other side of the barrier.

## Step-by-Step Solution

### 1. Physical Possibilities
Since $E < U_0$, the particle cannot classically pass the barrier. However, quantum mechanically, two things can happen:
* **Reflection:** The particle hits the barrier and bounces back.
* **Tunneling:** The particle "tunnels" through the forbidden region and emerges on the other side with its original energy $E=3 \, \mathrm{eV}$ but reduced probability amplitude.

### 2. Applications
Tunneling is a fundamental phenomenon utilized in:
* **Scanning Tunneling Microscopy (STM):** Uses tunneling current to image surfaces at the atomic level.
* **Alpha Decay:** Alpha particles tunnel out of the nucleus.
* **Flash Memory:** Floating-gate transistors use tunneling to store charge.

## Final Result

The particle has a finite probability of being found on the other side of the $5 \, \mathrm{eV}$ barrier despite having only $3 \, \mathrm{eV}$ of energy.

## Interpretation

The probability of tunneling is extremely sensitive to the width $a$ and the "height" difference $(U_0 - E)$. Even a small increase in barrier width leads to a massive drop in transmission probability due to the exponential nature of the decay.