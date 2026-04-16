# Task 04 – Kepler's First and Second Laws

## Problem Statement

Implement an elliptical orbit and verify Kepler's Second Law by calculating the area swept out by the radius vector in equal time intervals.

## Theory

Kepler's First Law states that planets move in ellipses with the Sun at one focus. The polar equation is:

$$
r(\theta) = \frac{a(1-e^2)}{1 + e \cos \theta}
$$

Kepler's Second Law (Law of Equal Areas) states that a line segment joining a planet and the Sun sweeps out equal areas during equal intervals of time. This is a consequence of the conservation of angular momentum $L$.

## Step-by-Step Solution

### 1. Area Calculation

The infinitesimal area $dA$ swept in polar coordinates is:

$$
dA = \frac{1}{2} r^2 d\theta
$$

To find the area between two angles $\theta_1$ and $\theta_2$:

$$
A = \frac{1}{2} \int_{\theta_1}^{\theta_2} r(\theta)^2 d\theta
$$

### 2. Relation to Time

From the definition of angular momentum:

$$
L = m r^2 \frac{d\theta}{dt} \implies r^2 d\theta = \frac{L}{m} dt
$$

Substituting this into the area integral:

$$
dA = \frac{L}{2m} dt
$$

Integrating both sides:

$$
A(t) = \frac{L}{2m} t
$$

Since $L$ and $m$ are constant for a central force, the area $A$ is directly proportional to time $t$.

## Final Result

The rate of area sweeping is constant:

$$
\frac{dA}{dt} = \frac{L}{2m} = \text{const}
$$

## Interpretation

The Second Law implies that the planet moves faster when it is closer to the Sun (perihelion) and slower when it is further away (aphelion). Physically, this confirms that gravity is a central force, which preserves the angular momentum of the orbiting body.