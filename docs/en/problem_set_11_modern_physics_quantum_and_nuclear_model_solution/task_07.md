# Task 07 – Quantum harmonic oscillator

## Problem Statement

1. Visualize the probability density for energy levels $n=0,1,2,3,4,5$.
2. Interpret the shape of the wavefunction and the probability density.
3. Explain why the particle must have zero-point energy.

## Theory

The potential is $V(x) = \frac{1}{2}m\omega^2 x^2$. The wavefunctions are:

$$
\psi_n(x) = \frac{1}{\sqrt{2^n n!}} \left( \frac{m\omega}{\pi \hbar} \right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}} H_n\left( \sqrt{\frac{m\omega}{\hbar}} x \right)
$$

where $H_n$ are Hermite polynomials.

## Step-by-Step Solution (Logic)

### 1. Visualization Logic
* **n=0 (Ground State):** A single Gaussian peak centered at $x=0$.
* **n=1:** Two peaks with a node at the center.
* **Higher n:** The number of peaks increases ($n+1$ peaks), and the probability shifts toward the classical "turning points."

### 2. Interpretation
Unlike a classical oscillator which spends most time at the edges (where velocity is lowest), the quantum ground state is most likely to be found at the center. As $n \to \infty$, the distribution approaches the classical probability density (Correspondence Principle).

## Final Result

The energy levels are equidistant:

$$
E_n = \hbar \omega \left( n + \frac{1}{2} \right)
$$

## Interpretation

**Zero-point energy:** Even at $n=0$, $E_0 = \frac{1}{2}\hbar \omega$. If $E=0$, both momentum and position would be exactly zero ($\Delta x=0, \Delta p=0$), violating the Uncertainty Principle. Thus, the particle must maintain a minimum "quiver" energy.