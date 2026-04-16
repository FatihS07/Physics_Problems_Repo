# Task 02 – Propagation of uncertainty using the total differential method

## Problem Statement

Resistance is determined from voltage and current measurements using Ohm's law:

$$
R = \frac{U}{I}
$$

The measured data with uncertainties are:

$$
\begin{align}
U &= 5.23 \pm 0.04 \text{ V} \\
I &= 0.482 \pm 0.006 \text{ A}
\end{align}
$$

The objective is to calculate the resistance $R$, derive the formula for relative uncertainty using the total differential method, and identify the measurement dominating the overall uncertainty.

## Theory

The total differential method estimates the maximum possible uncertainty (absolute error) of a function $f(x, y, ...)$ by summing the absolute values of the partial derivatives multiplied by the uncertainties of the respective variables:

$$
\Delta f = \left| \frac{\partial f}{\partial x} \right| \Delta x + \left| \frac{\partial f}{\partial y} \right| \Delta y + \dots
$$

In standard metrology notation, where $\Delta x$ is denoted as $u(x)$, the maximum absolute uncertainty is:

$$
u(R) = \left| \frac{\partial R}{\partial U} \right| u(U) + \left| \frac{\partial R}{\partial I} \right| u(I)
$$

The relative uncertainty is given by dividing the absolute uncertainty by the value of the function, yielding $\frac{u(R)}{R}$.

## Step-by-Step Solution

First, calculate the nominal value of the resistance $R$:

$$
R = \frac{5.23}{0.482} \approx 10.8506 \text{ }\Omega
$$

Next, derive the partial derivatives of $R$ with respect to $U$ and $I$:

$$
\begin{align}
\frac{\partial R}{\partial U} &= \frac{1}{I} \\
\frac{\partial R}{\partial I} &= -\frac{U}{I^2}
\end{align}
$$

Substitute these into the total differential formula for absolute uncertainty:

$$
u(R) = \left| \frac{1}{I} \right| u(U) + \left| -\frac{U}{I^2} \right| u(I)
$$

To find the relative uncertainty, divide both sides by $R = \frac{U}{I}$:

$$
\begin{align}
\frac{u(R)}{R} &= \frac{\frac{1}{I} u(U) + \frac{U}{I^2} u(I)}{\frac{U}{I}} \\
               &= \frac{u(U)}{U} + \frac{u(I)}{I}
\end{align}
$$

Calculate the individual relative contributions:

$$
\begin{align}
\frac{u(U)}{U} &= \frac{0.04}{5.23} \approx 0.0076 \quad (0.76\%) \\
\frac{u(I)}{I} &= \frac{0.006}{0.482} \approx 0.0124 \quad (1.24\%)
\end{align}
$$

Sum the contributions to find the total relative uncertainty:

$$
\frac{u(R)}{R} = 0.0076 + 0.0124 = 0.0200 \quad (2.0\%)
$$

Finally, calculate the absolute uncertainty $u(R)$:

$$
u(R) = R \times \frac{u(R)}{R} = 10.8506 \times 0.0200 \approx 0.217 \text{ }\Omega
$$

Rounding to appropriate significant figures, the absolute uncertainty is $0.22 \text{ }\Omega$.

## Final Result

The final calculated resistance is:

$$
R = 10.85 \pm 0.22 \text{ }\Omega
$$

The relative uncertainty is:

$$
\frac{u(R)}{R} = 2.0\%
$$

## Interpretation

The relative uncertainty derived using the total differential method simplifies to the sum of the relative uncertainties of the variables in the quotient. 

Comparing the individual contributions, the relative uncertainty from the current measurement ($\approx 1.24\%$) is larger than the relative uncertainty from the voltage measurement ($\approx 0.76\%$). Therefore, the current measurement dominates the overall uncertainty of the calculated resistance. To improve the precision of the resistance measurement, better instrumentation or methods should primarily target the current measurement.