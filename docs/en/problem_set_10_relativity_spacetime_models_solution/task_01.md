# Task 01 – Time Dilation

## Problem Statement

A spacecraft moves with a velocity $v = 0.8c$. 

1. Calculate the Lorentz factor $\gamma$.
2. Determine the time elapsed on Earth if 5 years pass on the ship.
3. Calculate the percentage effect of the dilation.
4. Investigate the limit as $v \to c$.
5. Provide a physical interpretation of the results.

## Theory

In special relativity, time is not absolute but depends on the relative velocity between observers. The time interval measured in the rest frame of an object is the proper time $\Delta t_0$. An observer in a different inertial frame moving at velocity $v$ relative to the object measures a dilated time $\Delta t$.

The relationship is governed by the Lorentz factor:

$$
\gamma = \frac{1}{\sqrt{1 - \frac{v^2}{c^2}}}
$$

The dilated time is given by:

$$
\Delta t = \gamma \Delta t_0
$$

## Step-by-Step Solution

### 1. Calculation of the Lorentz factor

Given $v = 0.8c$:

$$
\gamma = \frac{1}{\sqrt{1 - (0.8)^2}}
$$

$$
\gamma = \frac{1}{\sqrt{1 - 0.64}} = \frac{1}{\sqrt{0.36}}
$$

$$
\gamma = \frac{1}{0.6} = \frac{5}{3} \approx 1.667
$$

### 2. Time elapsed on Earth

The time elapsed on the ship is the proper time $\Delta t_0 = 5\,\text{years}$. The time measured by the Earth observer is:

$$
\Delta t = \gamma \Delta t_0
$$

$$
\Delta t = \left(\frac{5}{3}\right) \times 5 = \frac{25}{3} \approx 8.33\,\text{years}
$$

### 3. Percentage effect of dilation

The percentage increase in time compared to the proper time is:

$$
\text{Effect} = (\gamma - 1) \times 100\%
$$

$$
\text{Effect} = (1.667 - 1) \times 100\% = 66.7\%
$$

### 4. Limit as $v \to c$

As the velocity $v$ approaches the speed of light $c$:

$$
\lim_{v \to c} \left( 1 - \frac{v^2}{c^2} \right) = 0
$$

Consequently:

$$
\lim_{v \to c} \gamma = \infty
$$

This implies that as $v$ approaches $c$, the dilated time $\Delta t$ approaches infinity for any finite proper time $\Delta t_0$.

## Final Result

- Lorentz factor: $\gamma \approx 1.667$
- Time on Earth: $8.33\,\text{years}$
- Percentage effect: $66.7\%$

## Interpretation

The result demonstrates that "moving clocks run slow." For the Earth observer, the processes on the spacecraft (including the aging of the crew and the ticking of clocks) appear to take longer. At $0.8c$, this effect is significant, adding more than 3 years to the Earth-observed duration of a 5-year journey. The limit $v \to c$ suggests that for a photon (moving at $c$), proper time does not pass at all.