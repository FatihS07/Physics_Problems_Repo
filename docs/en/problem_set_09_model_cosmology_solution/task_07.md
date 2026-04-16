# Task 07 – Newton's Gravity and Orbit Classification

## Problem Statement

Classify the trajectories of a mass in a central gravitational field based on its total energy $E$.

## Theory

The total energy $E$ of a body of mass $m$ in the field of a mass $M$ is:

$$
E = \frac{1}{2} m v^2 - \frac{GMm}{r}
$$

The shape of the orbit is determined by the eccentricity $e$, which is related to energy:

$$
e = \sqrt{1 + \frac{2EL^2}{m(GMm)^2}}
$$

## Step-by-Step Solution

### 1. Case Analysis

The type of conic section depends on the sign of $E$:

* **$E < 0$**: The body does not have enough kinetic energy to escape the potential well. The orbit is **bound** (ellipse or circle). $e < 1$.
* **$E = 0$**: The body has exactly the escape velocity. The orbit is a **parabola**. $e = 1$.
* **$E > 0$**: The body has excess kinetic energy. The orbit is **unbound** (hyperbola). $e > 1$.

### 2. Escape Velocity

Setting $E = 0$:

$$
\frac{1}{2} m v_e^2 = \frac{GMm}{r} \implies v_e = \sqrt{\frac{2GM}{r}}
$$

## Final Result

Orbits are classified as follows:
- Bound: $v < v_e$
- Critical: $v = v_e$
- Unbound: $v > v_e$

## Interpretation

Energy conservation dictates that a planet cannot change its orbit type unless an external force (work) is applied. This ensures the long-term stability of bound planetary orbits.