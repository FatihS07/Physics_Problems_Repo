# Task 07 – Loop pulled into a magnetic field region

## Problem Statement

A rectangular conducting loop with resistance $R=0.40\ \Omega$ and dimensions $a=0.20\ \mathrm{m}$ by $b=0.10\ \mathrm{m}$ is pulled with constant velocity $v=1.5\ \mathrm{m/s}$ into a uniform perpendicular magnetic field $B=0.60\ \mathrm{T}$. Determine the flux, EMF, current, braking force, and mechanical power in the entering phase, and state what happens when fully submerged in the field.

## Theory

When the loop partially enters the field, the area containing magnetic flux changes. Assuming the leading edge entering the field has length $a$, the area swept over time is $A(t) = a \cdot x(t)$, where $x(t) = vt$. This changing flux induces an EMF. By Lenz's law, the induced current interacts with the external field to produce a force opposing the pulling motion.

## Step-by-Step Solution

Write the flux $\Phi(t)$ in the entering phase. The area inside the field at time $t$ is $A(t) = a v t$.

$$
\Phi(t) = B A(t) = B a v t
$$

Determine the induced EMF $\mathcal{E}$ using Faraday's law:

$$
\mathcal{E} = \left| \frac{d\Phi}{dt} \right| = B a v
$$

Substitute the numerical values to find $\mathcal{E}$:

$$
\mathcal{E} = 0.60 \cdot 0.20 \cdot 1.5 = 0.18\ \mathrm{V}
$$

Determine the current $I$ using Ohm's law:

$$
I = \frac{\mathcal{E}}{R} = \frac{B a v}{R}
$$

$$
I = \frac{0.18}{0.40} = 0.45\ \mathrm{A}
$$

Determine the braking force $F(v)$. Only the leading segment of length $a$ is inside the magnetic field and oriented perpendicular to the field lines. 

$$
F = I a B = \left( \frac{B a v}{R} \right) a B
$$

$$
F = \frac{B^2 a^2 v}{R}
$$

Substitute numerical values for the force:

$$
F = \frac{(0.60)^2 \cdot (0.20)^2 \cdot 1.5}{0.40} = 0.054\ \mathrm{N}
$$

Calculate the mechanical power $P_{mech}$ required to maintain constant velocity:

$$
P_{mech} = F v = 0.054 \cdot 1.5 = 0.081\ \mathrm{W}
$$

Show that this equals the thermal power $P_{thermal}$:

$$
P_{thermal} = I^2 R = (0.45)^2 \cdot 0.40 = 0.081\ \mathrm{W}
$$

Analyze the state when the loop is entirely in the uniform field. Once fully submerged, the total flux through the loop is constant:

$$
\Phi_{max} = B a b
$$

Because the flux is no longer changing with time, its derivative is zero.

$$
\frac{d\Phi}{dt} = 0 \implies \mathcal{E} = 0
$$

## Final Result

1. Flux in entering phase: $\Phi(t) = B a v t$.
2. Induced EMF: $\mathcal{E} = 0.18\ \mathrm{V}$, Current: $I = 0.45\ \mathrm{A}$.
3. Braking force: $F = 0.054\ \mathrm{N}$.
4. Mechanical power is $0.081\ \mathrm{W}$, which exactly equals the Joule heating $I^2R$.
5. When entirely in the field, $\Phi$ is constant, so $\mathcal{E}=0$, $I=0$, and the braking force drops to zero.

## Interpretation

Work must be done against the magnetic force specifically during the spatial transition between regions of different field strengths. Inside a uniform field, a purely translational motion of a closed loop induces no net EMF because the rate of flux entering at the front edge exactly equals the rate of flux leaving at the rear edge.