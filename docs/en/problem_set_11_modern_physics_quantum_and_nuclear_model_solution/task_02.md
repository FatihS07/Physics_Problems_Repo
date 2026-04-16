# Task 02 – Bohr model of the hydrogen atom

## Problem Statement

1. Derive the quantization condition for angular momentum.
2. Derive the formula for the orbit radius.
3. Calculate the energy of the $n=1$ level.
4. Calculate the energy of the $n=3 \to n=2$ transition.
5. Determine the wavelength of the emitted photon.

## Theory

The Bohr model assumes that electrons move in circular orbits around the nucleus, held by Coulombic attraction. Bohr postulated that the angular momentum $L$ is quantized in units of $\hbar = h/2\pi$.

$$
L = n\hbar = n\frac{h}{2\pi}
$$

For a circular orbit, $L = mvr$. The centripetal force is provided by the Coulomb force:

$$
\frac{mv^2}{r} = \frac{ke^2}{r^2}
$$

where $k = \frac{1}{4\pi\epsilon_0}$.

## Step-by-Step Solution

### 1. Angular Momentum Quantization
From the de Broglie hypothesis, a standing wave condition on the orbit circumference $2\pi r$ requires:

$$
2\pi r = n\lambda = n\frac{h}{p}
$$

Rearranging gives the quantization condition:

$$
pr = n\frac{h}{2\pi} \implies L = n\hbar
$$

### 2. Orbit Radius Derivation
From the force balance:

$$
v^2 = \frac{ke^2}{mr}
$$

From quantization:

$$
v = \frac{n\hbar}{mr} \implies v^2 = \frac{n^2\hbar^2}{m^2r^2}
$$

Equating the two expressions for $v^2$:

$$
\frac{ke^2}{mr} = \frac{n^2\hbar^2}{m^2r^2}
$$

$$
r_n = \frac{n^2\hbar^2}{mke^2}
$$

### 3. Energy of n=1 Level
The total energy is $E = K + U = \frac{1}{2}mv^2 - \frac{ke^2}{r}$. Using the force balance $\frac{1}{2}mv^2 = \frac{ke^2}{2r}$:

$$
E_n = -\frac{ke^2}{2r_n} = -\frac{mk^2e^4}{2\hbar^2 n^2}
$$

For $n=1$:

$$
E_1 = -13.6 \, \mathrm{eV}
$$

### 4. Transition Energy (n=3 to n=2)
The energy of the emitted photon is $\Delta E = E_3 - E_2$:

$$
\Delta E = -13.6 \left( \frac{1}{3^2} - \frac{1}{2^2} \right) = -13.6 \left( \frac{1}{9} - \frac{1}{4} \right)
$$

$$
\Delta E = -13.6 \left( \frac{4-9}{36} \right) = -13.6 \left( -\frac{5}{36} \right) \approx 1.89 \, \mathrm{eV}
$$

### 5. Wavelength Calculation
Using $E = \frac{hc}{\lambda}$:

$$
\lambda = \frac{1240 \, \mathrm{eV \cdot nm}}{1.89 \, \mathrm{eV}} \approx 656 \, \mathrm{nm}
$$

## Final Result

* **Radius:** $r_n = \frac{n^2\hbar^2}{mke^2}$
* **Ground State Energy:** $-13.6 \, \mathrm{eV}$
* **Transition Energy:** $1.89 \, \mathrm{eV}$
* **Wavelength:** $656 \, \mathrm{nm}$ (H-alpha line)

## Interpretation

The calculated wavelength corresponds to the visible red line in the Balmer series. This demonstrates that discrete energy levels in atoms lead to discrete spectral lines, confirming the quantized nature of atomic structures.