# Task 07 – Relativistic Energy and Momentum

## Problem Statement

1. Calculate total energy $E$ of an electron for $v = 0.95c$.
2. Calculate kinetic energy $E_k$.
3. Compare with classical $K = \frac{1}{2}mv^2$.
4. Investigate the limit $v \ll c$.
5. Interpret the energy-momentum relation.

## Theory

The total relativistic energy and momentum are:

$$
E = \gamma mc^2
$$

$$
p = \gamma mv
$$

The kinetic energy is the total energy minus rest energy:

$$
E_k = (\gamma - 1)mc^2
$$

## Step-by-Step Solution

### 1. Lorentz factor for $v = 0.95c$

$$
\gamma = \frac{1}{\sqrt{1 - 0.95^2}} \approx 3.203
$$

### 2. Total and Kinetic Energy

For an electron ($mc^2 \approx 0.511\,\text{MeV}$):

$$
E = 3.203 \times 0.511 \approx 1.637\,\text{MeV}
$$

$$
E_k = (3.203 - 1) \times 0.511 \approx 1.126\,\text{MeV}
$$

### 3. Classical comparison

$$
K_{class} = \frac{1}{2} m (0.95c)^2 = 0.451 \times mc^2 \approx 0.230\,\text{MeV}
$$

The relativistic result is nearly 5 times larger.

### 4. Low velocity limit

Using Taylor expansion for $\gamma$:

$$
\gamma \approx 1 + \frac{1}{2}\beta^2 + \dots
$$

$$
E_k \approx (1 + \frac{1}{2}\frac{v^2}{c^2} - 1)mc^2 = \frac{1}{2}mv^2
$$

## Final Result

- $E_{total} \approx 1.64\,\text{MeV}$
- $E_k \approx 1.13\,\text{MeV}$
- $K_{class} \approx 0.23\,\text{MeV}$

## Interpretation

The relation $E^2 = p^2c^2 + m^2c^4$ shows that energy and momentum are coupled. It also allows for massless particles ($m=0$), where $E=pc$.