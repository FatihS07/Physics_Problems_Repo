# Task 01 – Ptolemy's Model

## Problem Statement

Describe the motion of a planet using the geocentric epicyclic model. Derive the parametric equations for the trajectory based on the deferent and the epicycle. Investigate the conditions and timing for retrograde motion.

## Theory

In the Ptolemaic system, the Earth is stationary at the center. A planet moves along a small circle called the epicycle, whose center moves along a larger circle called the deferent.

Let $R$ be the radius of the deferent and $r$ be the radius of the epicycle. Let $\omega$ be the angular velocity of the epicycle's center around the Earth, and $\Omega$ be the angular velocity of the planet around the center of the epicycle.

The position vector of the planet $\vec{r}(t)$ is the vector sum of the deferent radius vector $\vec{R}(t)$ and the epicycle radius vector $\vec{\rho}(t)$:

$$
\vec{r}(t) = \vec{R}(t) + \vec{\rho}(t)
$$

## Step-by-Step Solution

### 1. Parametric Representation

Using the definitions of circular motion in a 2D plane:

$$
\vec{R}(t) = \begin{pmatrix} R \cos(\omega t) \\ R \sin(\omega t) \end{pmatrix}
$$

$$
\vec{\rho}(t) = \begin{pmatrix} r \cos(\Omega t) \\ r \sin(\Omega t) \end{pmatrix}
$$

The trajectory $(x(t), y(t))$ is given by:

$$
x(t) = R \cos(\omega t) + r \cos(\Omega t)
$$

$$
y(t) = R \sin(\omega t) + r \sin(\Omega t)
$$

### 2. Angular Velocity and Retrograde Motion

The angular position (ecliptic longitude) $\phi(t)$ is defined as:

$$
\tan \phi(t) = \frac{y(t)}{x(t)}
$$

Differentiating with respect to time gives the angular velocity $\dot{\phi}$. Retrograde motion occurs when the direction of the angular velocity of the planet as seen from Earth is opposite to the direction of the deferent's motion. Assuming $\omega > 0$, retrograde motion occurs when:

$$
\dot{\phi} < 0
$$

To simplify, consider the velocity components:

$$
\dot{x}(t) = -R\omega \sin(\omega t) - r\Omega \sin(\Omega t)
$$

$$
\dot{y}(t) = R\omega \cos(\omega t) + r\Omega \cos(\Omega t)
$$

The angular momentum per unit mass relative to the origin is $L = x\dot{y} - y\dot{x}$. Since $\dot{\phi} = L / r^2$, the condition $\dot{\phi} < 0$ is equivalent to $L < 0$:

$$
(R \cos \omega t + r \cos \Omega t)(R\omega \cos \omega t + r\Omega \cos \Omega t) - (R \sin \omega t + r \sin \Omega t)(-R\omega \sin \omega t - r\Omega \sin \Omega t) < 0
$$

Expanding the terms:

$$
R^2\omega + r^2\Omega + Rr(\omega + \Omega) \cos((\Omega - \omega)t) < 0
$$

### 3. Conditions for Occurrence

For the inequality to hold at any point, the minimum value of the expression must be less than zero. The minimum occurs when $\cos((\Omega - \omega)t) = -1$:

$$
R^2\omega + r^2\Omega - Rr(\omega + \Omega) < 0
$$

$$
(R\omega - r\Omega)(R - r) < 0
$$

Assuming $R > r$ (the deferent is larger than the epicycle), the condition becomes:

$$
r\Omega > R\omega
$$

The planet's tangential speed on the epicycle must exceed the center's tangential speed on the deferent.

## Final Result

The parametric equations are:

$$
\begin{pmatrix} x(t) \\ y(t) \end{pmatrix} = \begin{pmatrix} R \cos(\omega t) + r \cos(\Omega t) \\ R \sin(\omega t) + r \sin(\Omega t) \end{pmatrix}
$$

Retrograde motion begins and ends when:

$$
\cos((\Omega - \omega)t) = -\frac{R^2\omega + r^2\Omega}{Rr(\omega + \Omega)}
$$

## Interpretation

Retrograde motion in the Ptolemaic model is a real reversal of the planet's path in space caused by the superposition of two circular motions. It is a "kinematic illusion" only in the sense that the Earth is assumed to be stationary; however, the loops in the trajectory are physical features of this specific coordinate description.