# Task 08 – Radioactive decay

## Problem Statement

1. Implement a Monte Carlo simulation of decay.
2. Compare the simulation with the analytical solution: $N(t)=N_0 e^{-\lambda t}$.
3. Investigate the fluctuations for a small $N_0$.
4. Determine the half-life.

## Theory

Radioactive decay is a stochastic process. The probability that a specific nucleus decays in a small interval $dt$ is $\lambda dt$.

## Step-by-Step Solution

### 1. Monte Carlo Algorithm
For each of $N_0$ nuclei:
1. Generate a random number $r \in [0, 1]$.
2. Calculate the decay time $\tau = -\frac{\ln(r)}{\lambda}$.
3. Sort these times to find $N(t)$ at any moment.

### 2. Comparison
The simulation follows the exponential curve closely for large $N_0$. For small $N_0$ (e.g., $N_0 = 20$), the "steps" in the decay become visible, representing individual quantum events.

### 3. Half-life Calculation
The half-life $T_{1/2}$ is the time when $N(t) = \frac{N_0}{2}$:

$$
\frac{1}{2} = e^{-\lambda T_{1/2}} \implies T_{1/2} = \frac{\ln 2}{\lambda}
$$

## Final Result

The continuous solution $N(t)$ is the **expectation value** of the stochastic process. 

## Interpretation

Fluctuations ($\sqrt{N}$ noise) are dominant when $N$ is small. This demonstrates that while we can predict the behavior of a bulk sample with high precision, the decay time of a single nucleus is fundamentally unpredictable.