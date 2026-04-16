# Task 03 – Photoelectric effect

## Problem Statement

For a metal with a work function of $W = 3.2 \, \mathrm{eV}$.

1. Determine the threshold frequency.
2. Calculate the maximum kinetic energy of the electrons for light with $f = 1.5 f_0$.
3. Calculate the stopping potential.
4. Does increasing the intensity change the kinetic energy?
5. What contradicted the classical wave theory?

## Theory

Einstein's photoelectric equation is:

$$
hf = W + K_{max}
$$

The threshold frequency $f_0$ is the minimum frequency required to eject an electron ($K_{max} = 0$):

$$
hf_0 = W
$$

## Step-by-Step Solution

### 1. Threshold Frequency
Given $W = 3.2 \, \mathrm{eV}$:

$$
f_0 = \frac{W}{h} = \frac{3.2 \times 1.6 \times 10^{-19} \, \mathrm{J}}{6.626 \times 10^{-34} \, \mathrm{J \cdot s}}
$$

$$
f_0 \approx 7.73 \times 10^{14} \, \mathrm{Hz}
$$

### 2. Maximum Kinetic Energy
If $f = 1.5 f_0$:

$$
K_{max} = h(1.5f_0) - W = 1.5(hf_0) - W
$$

Since $hf_0 = W$:

$$
K_{max} = 1.5W - W = 0.5W
$$

$$
K_{max} = 0.5(3.2 \, \mathrm{eV}) = 1.6 \, \mathrm{eV}
$$

### 3. Stopping Potential
The stopping potential $V_s$ is defined by $eV_s = K_{max}$:

$$
V_s = \frac{1.6 \, \mathrm{eV}}{e} = 1.6 \, \mathrm{V}
$$

## Final Result

* **Threshold Frequency:** $7.73 \times 10^{14} \, \mathrm{Hz}$
* **Kinetic Energy:** $1.6 \, \mathrm{eV}$
* **Stopping Potential:** $1.6 \, \mathrm{V}$

## Interpretation

4. **Intensity:** Increasing the intensity increases the number of photons (and thus the number of emitted electrons), but it does **not** change the kinetic energy of individual electrons, as $K_{max}$ depends only on frequency.

5. **Classical Contradictions:**
* **Existence of Threshold Frequency:** Classically, any frequency should eventually eject electrons if intensity is high enough.
* **Instantaneous Emission:** Classically, low-intensity light would require a "soak time" to build energy; experimentally, emission is nearly instant.
* **Energy Dependence:** Classically, $K_{max}$ should depend on intensity, not frequency.