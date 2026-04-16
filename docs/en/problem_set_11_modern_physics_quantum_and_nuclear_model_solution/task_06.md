# Task 06 – Evolution of a wave packet

## Problem Statement

1. Build a Gaussian wave packet: $\psi(x,0)=e^{-\frac{x^2}{2\sigma^2}} e^{ik_0 x}$.
2. Implement the time evolution using Fast Fourier Transform (FFT).
3. Investigate the spreading of the packet.
4. Interpret it in the context of the uncertainty principle.

## Theory

A wave packet represents a localized particle. Its evolution is governed by the Schrödinger equation. In momentum space, each component $\phi(k)$ evolves by a phase factor:

$$
\phi(k, t) = \phi(k, 0) e^{-i\omega(k)t}
$$

For a free particle, the dispersion relation is:

$$
\omega(k) = \frac{\hbar k^2}{2m}
$$

## Step-by-Step Solution (Simulation Logic)

### 1. Initialization
Define a spatial grid $x$ and the initial state $\psi(x,0)$. The term $e^{ik_0 x}$ gives the packet an initial group velocity $v_g = \frac{\hbar k_0}{m}$.

### 2. Spectral Transformation
Use FFT to move to the $k$-space. The Gaussian in $x$ remains a Gaussian in $k$:

$$
\psi(x,0) \xrightarrow{FFT} \phi(k,0)
$$

### 3. Time Advancement
Multiply by the propagator in $k$-space and transform back:

$$
\psi(x,t) = IFFT \left( \phi(k,0) e^{-i \frac{\hbar k^2}{2m} t} \right)
$$

### 4. Spreading
The width $\sigma(t)$ evolves as:

$$
\sigma(t) = \sigma_0 \sqrt{1 + \left( \frac{\hbar t}{m \sigma_0^2} \right)^2}
$$

## Final Result

The simulation shows a Gaussian envelope moving at $v_g$ while simultaneously broadening. The probability density $|\psi(x,t)|^2$ flattens over time.

## Interpretation

This spreading is a direct consequence of the **Heisenberg Uncertainty Principle**. A localized packet ($\Delta x$ small) contains a wide range of momenta ($\Delta p$ large). Since different momentum components travel at different speeds, the packet inevitably disperses.