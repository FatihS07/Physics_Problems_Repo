# Task 03 – Lorentz Transformation

## Problem Statement

Two events occur in frame $S$:
- Event 1: $x_1 = 0$, $t_1 = 0$
- Event 2: $x_2 = 900\,\text{m}$, $t_2 = 4\,\mu\text{s}$

Frame $S'$ moves at $v = 0.6c$ relative to $S$.

1. Apply the Lorentz transformation formulas.
2. Calculate coordinates $(x_2', t_2')$ in $S'$.
3. Determine if the order of events can change.
4. Calculate the spacetime interval $s^2$.
5. Verify the invariance of $s^2$.

## Theory

The Lorentz transformations relate coordinates $(x, t)$ in frame $S$ to $(x', t')$ in $S'$:

$$
x' = \gamma (x - vt)
$$

$$
t' = \gamma \left(t - \frac{vx}{c^2}\right)
$$

The spacetime interval is defined as:

$$
s^2 = c^2 t^2 - x^2
$$

## Step-by-Step Solution

### 1. Constants and Lorentz factor

For $v = 0.6c$, $\gamma = 1.25$.
Speed of light $c \approx 300\,\text{m}/\mu\text{s}$.
Velocity $v = 0.6 \times 300 = 180\,\text{m}/\mu\text{s}$.

### 2. Transformation of Event 2

For $x_2 = 900\,\text{m}$ and $t_2 = 4\,\mu\text{s}$:

$$
x_2' = 1.25 \times (900 - 180 \times 4)
$$

$$
x_2' = 1.25 \times (900 - 720) = 1.25 \times 180 = 225\,\text{m}
$$

Now for $t_2'$:

$$
t_2' = 1.25 \times \left(4 - \frac{180 \times 900}{300^2}\right)
$$

$$
t_2' = 1.25 \times \left(4 - \frac{162000}{90000}\right) = 1.25 \times (4 - 1.8) = 1.25 \times 2.2 = 2.75\,\mu\text{s}
$$

### 3. Order of events

Since $t_1' = 0$ (calculated from $x_1=0, t_1=0$) and $t_2' = 2.75\,\mu\text{s}$, the order remains the same ($t_2' > t_1'$). The order can only change if the events are "space-like" separated ($|x_2 - x_1| > c|t_2 - t_1|$). Here, $900\,\text{m} < 300 \times 4 = 1200\,\text{m}$, so they are "time-like."

### 4. Spacetime interval in $S$

$$
s^2 = (300 \times 4)^2 - (900)^2
$$

$$
s^2 = 1200^2 - 900^2 = 1,440,000 - 810,000 = 630,000\,\text{m}^2
$$

### 5. Verification in $S'$

$$
(s')^2 = (300 \times 2.75)^2 - (225)^2
$$

$$
(s')^2 = 825^2 - 225^2 = 680,625 - 50,625 = 630,000\,\text{m}^2
$$

## Final Result

- $x_2' = 225\,\text{m}$, $t_2' = 2.75\,\mu\text{s}$
- $s^2 = 630,000\,\text{m}^2$ (Invariant)

## Interpretation

The transformation shows that while space and time coordinates change, the spacetime interval remains constant. This confirms that $s^2$ is the objective "distance" in Minkowski spacetime.