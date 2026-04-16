# Task 04 – Rotating loop (induction)

## Problem Statement

A loop with area $S$ and $N$ turns rotates with angular velocity $\omega$ in a uniform magnetic field $\vec B$ around an axis perpendicular to the field. Determine the magnetic flux $\Phi(t)$, electromotive force $\mathcal{E}(t)$, amplitude $\mathcal{E}_0$, dependence of amplitude on $\omega$, and interpret the mechanism.

## Theory

Faraday's Law of Induction states that the induced electromotive force (EMF) in a closed circuit is equal to the negative rate of change of the magnetic flux through the circuit:

$$
\mathcal{E} = -N \frac{d\Phi_{single}}{dt} = -\frac{d\Phi_{total}}{dt}
$$

The magnetic flux through a single loop is the dot product of the magnetic field and the area vector:

$$
\Phi_{single} = \vec B \cdot \vec S = B S \cos\theta
$$

## Step-by-Step Solution

Since the loop rotates with constant angular velocity $\omega$, the angle $\theta$ between the normal to the loop and the magnetic field changes linearly with time:

$$
\theta(t) = \omega t
$$

Determine the total magnetic flux $\Phi(t)$ linking the $N$ turns:

$$
\Phi(t) = N B S \cos(\omega t)
$$

Determine the induced EMF $\mathcal{E}(t)$ by taking the time derivative of the flux:

$$
\begin{align}
\mathcal{E}(t) &= -\frac{d}{dt} [N B S \cos(\omega t)] \\
&= -N B S \left[ -\omega \sin(\omega t) \right] \\
&= N B S \omega \sin(\omega t)
\end{align}
$$

Identify the amplitude of the induced EMF, $\mathcal{E}_0$. The sine function oscillates between -1 and 1, so the maximum value (amplitude) is the coefficient in front of the sine term:

$$
\mathcal{E}_0 = N B S \omega
$$

Analyze the dependence of the amplitude on the angular velocity $\omega$. The equation shows a direct, linear proportionality:

$$
\mathcal{E}_0 \propto \omega
$$

## Final Result

1. Flux: $\Phi(t) = N B S \cos(\omega t)$.
2. Induced EMF: $\mathcal{E}(t) = N B S \omega \sin(\omega t)$.
3. Amplitude: $\mathcal{E}_0 = N B S \omega$.
4. The amplitude is strictly directly proportional to $\omega$.

## Interpretation

This system describes the fundamental operating principle of an alternating current (AC) generator (alternator). Mechanical energy is used to rotate the loop, continuously changing the magnetic flux, which continuously generates a sinusoidal electromotive force.