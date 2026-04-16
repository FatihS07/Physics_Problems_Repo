# Task 10 – Numerical Simulation

## Problem Statement

1. Implement RK4 for $\frac{d}{dt}(\gamma m v) = F$.
2. Compare classical vs. relativistic motion.
3. Investigate the speed limit $c$.

## Theory

Relativistic force:

$$
F = \frac{dp}{dt} = \frac{d}{dt} \left( \frac{mv}{\sqrt{1-v^2/c^2}} \right)
$$

For a constant force, the acceleration $a = dv/dt$ decreases as $v$ increases:

$$
a = \frac{F}{m\gamma^3}
$$

## Step-by-Step Solution

### 1. Integration Logic

Using RK4, we update momentum $p$ linearly: $p_{n+1} = p_n + F\Delta t$. Then solve for $v$:

$$
v = \frac{p/m}{\sqrt{1 + (p/mc)^2}}
$$

### 2. Asymptotic Approach

In the classical model, $v = (F/m)t$ grows linearly to infinity. In the relativistic model, as $p \to \infty$, $v \to c$.

## Interpretation

Mass effectively increases with velocity (or rather, it becomes increasingly difficult to accelerate), ensuring that no massive particle exceeds the speed of light.