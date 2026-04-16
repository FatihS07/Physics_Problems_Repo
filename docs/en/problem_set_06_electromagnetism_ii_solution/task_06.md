# Task 06 – Rod on metal rails in a magnetic field

## Problem Statement

A conducting rod of mass $m=0.20\ \mathrm{kg}$ slides without friction on two parallel rails separated by $L=0.30\ \mathrm{m}$. The rails form an incline of angle $\alpha=25^\circ$. A uniform magnetic field $B=0.80\ \mathrm{T}$ is perpendicular to the plane of the rails. The total electrical resistance is $R=0.50\ \Omega$. Determine the motional EMF, current, magnetic braking force, equation of motion, terminal velocity, and power balance. 

## Theory

When the rod moves with velocity $v$, it sweeps out an area in the magnetic field, changing the magnetic flux and inducing a motional electromotive force according to Faraday's law. 

The induced current flowing through the rod in the presence of the external magnetic field results in a Lorentz force (specifically, the Laplace force) acting on the macroscopic conductor. The direction of this force, governed by Lenz's law, always opposes the motion that generated it.

## Step-by-Step Solution

Determine the motional EMF. The velocity vector is perpendicular to the magnetic field vector.

$$
\mathcal{E}(v) = v B L
$$

Determine the induced current using Ohm's law. 

$$
I(v) = \frac{\mathcal{E}(v)}{R} = \frac{v B L}{R}
$$

Determine the magnetic braking force. The force on a current-carrying wire of length $L$ in a perpendicular magnetic field is:

$$
F_m = I L B
$$

Substitute the expression for current:

$$
F_m = \left( \frac{v B L}{R} \right) L B
$$

$$
F_m = \frac{v B^2 L^2}{R}
$$

Write the equation of motion along the incline. The driving force is the component of gravity parallel to the incline. The opposing force is the magnetic braking force.

$$
m \frac{dv}{dt} = m g \sin\alpha - F_m
$$

Substitute the braking force expression to yield a differential equation with damping proportional to $v$:

$$
m \frac{dv}{dt} = m g \sin\alpha - \frac{B^2 L^2}{R} v
$$

Determine the terminal velocity $v_\infty$. In the steady state, acceleration is zero, meaning the net force is zero.

$$
0 = m g \sin\alpha - \frac{B^2 L^2}{R} v_\infty
$$

$$
v_\infty = \frac{m g R \sin\alpha}{B^2 L^2}
$$

Calculate the numerical value for $v_\infty$:

$$
v_\infty = \frac{0.20 \cdot 9.81 \cdot 0.50 \cdot \sin(25^\circ)}{(0.80)^2 \cdot (0.30)^2}
$$

$$
v_\infty = \frac{0.981 \cdot 0.4226}{0.64 \cdot 0.09}
$$

$$
v_\infty = \frac{0.4146}{0.0576} \approx 7.20\ \mathrm{m/s}
$$

Perform the power balance in the steady state. The mechanical power provided by gravity is:

$$
P_{grav} = F_g v_\infty = (m g \sin\alpha) v_\infty
$$

The thermal power dissipated as Joule heat is:

$$
P_{heat} = I^2 R = \left( \frac{v_\infty B L}{R} \right)^2 R
$$

$$
P_{heat} = \frac{v_\infty^2 B^2 L^2}{R}
$$

From the equilibrium condition, $m g \sin\alpha = \frac{v_\infty B^2 L^2}{R}$. Multiply both sides by $v_\infty$:

$$
(m g \sin\alpha) v_\infty = \frac{v_\infty^2 B^2 L^2}{R}
$$

Thus, $P_{grav} = P_{heat}$.

## Final Result

1. Motional EMF: $\mathcal{E}(v) = vBL$, Current: $I(v) = \frac{vBL}{R}$.
2. Braking force: $F_m = \frac{v B^2 L^2}{R}$.
3. Equation of motion: $m \frac{dv}{dt} = m g \sin\alpha - \frac{B^2 L^2}{R} v$.
4. Terminal velocity is $v_\infty \approx 7.20\ \mathrm{m/s}$.
5. The steady-state power balance $m g \sin\alpha \cdot v_\infty = I^2 R$ is confirmed.

## Interpretation

The system acts as a linear electric generator. The mechanical energy extracted from the gravitational field is completely converted into electrical energy, which is subsequently dissipated as heat in the resistors. The terminal velocity represents the point where energy conversion rates perfectly balance.