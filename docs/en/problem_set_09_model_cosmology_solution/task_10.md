# Task 10 – Stability and Conserved Quantities

## Problem Statement

Evaluate the stability of the numerical integration by monitoring conserved quantities ($E, \vec{L}$) in a three-body system.

## Theory

In a perfect physical system, the total energy $E$ and angular momentum $\vec{L}$ are constant. Numerical errors in integration (truncation and rounding) cause these values to drift over time.

## Step-by-Step Solution

### 1. Conserved Quantities

$$
E = \sum_i \frac{1}{2}m_i v_i^2 - \sum_{i < j} \frac{Gm_i m_j}{r_{ij}}
$$

$$
\vec{L} = \sum_i m_i (\vec{r}_i \times \vec{v}_i)
$$

### 2. Stability Analysis

* **Time Step $\Delta t$:** A smaller $\Delta t$ reduces truncation error but increases computation time and may accumulate more floating-point rounding errors.
* **Symplectic Integrators:** For long-term stability in orbits, methods like the Verlet integrator are preferred over RK4 because they better conserve the Hamiltonian (energy) of the system.

## Final Result

A stable numerical simulation is characterized by $E(t) \approx \text{const}$. If $E$ increases or decreases monotonically, the integration step is too large or the method is unsuitable for long-term orbital mechanics.

## Interpretation

Numerical stability is crucial in cosmology. Even a $0.01\%$ error per orbit can lead to a planet "flying away" or crashing into the Sun after several simulated millennia.