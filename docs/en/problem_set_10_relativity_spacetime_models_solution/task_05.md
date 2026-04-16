# Task 05 – Muons in the Atmosphere

## Problem Statement

Muons are created at an altitude of 10 km.
- Proper lifetime: $\tau_0 = 2.2\,\mu\text{s}$
- Velocity: $v = 0.995c$

1. Calculate the Lorentz factor.
2. Calculate the mean lifetime in the Earth's frame.
3. Calculate the average distance traveled.
4. Determine if the muon reaches the surface without relativity.

## Theory

Due to time dilation, a particle moving at relativistic speeds appears to live longer from the perspective of a stationary observer:

$$
\tau = \gamma \tau_0
$$

## Step-by-Step Solution

### 1. Lorentz factor

For $v = 0.995c$:

$$
\gamma = \frac{1}{\sqrt{1 - (0.995)^2}} \approx \frac{1}{\sqrt{1 - 0.990025}} \approx \frac{1}{0.09987} \approx 10.0125
$$

### 2. Lifetime in Earth frame

$$
\tau = 10.0125 \times 2.2\,\mu\text{s} \approx 22.03\,\mu\text{s}
$$

### 3. Average distance traveled

Using $d = v\tau$ and $c \approx 300\,\text{m}/\mu\text{s}$:

$$
d = (0.995 \times 300) \times 22.03 \approx 298.5 \times 22.03 \approx 6576\,\text{m}
$$

### 4. Classical limit

Without relativity, the distance would be:

$$
d_{class} = v\tau_0 = 298.5 \times 2.2 \approx 656.7\,\text{m}
$$

Since $656.7\,\text{m} \ll 10,000\,\text{m}$, the muon would never reach the surface classically.

## Final Result

- Lorentz factor: $\gamma \approx 10.0$
- Dilated lifetime: $22.03\,\mu\text{s}$
- Relativistic distance: $\approx 6.58\,\text{km}$

## Interpretation

While the muon still decays on average before hitting the ground from 10km, the flux of muons detected at sea level is only possible because time dilation extends their life significantly. From the muon's perspective, the atmosphere is length-contracted.