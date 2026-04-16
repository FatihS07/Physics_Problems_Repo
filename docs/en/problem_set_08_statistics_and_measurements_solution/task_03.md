# Task 03 – Propagation of uncertainty (density)

## Problem Statement

The density of a rectangular cuboid is calculated using the formula:

$$
\rho = \frac{m}{abc}
$$

The given measurements and their uncertainties are:

$$
\begin{align}
m &= 128.4 \pm 0.2\ \mathrm{g} \\
a &= 5.20 \pm 0.02\ \mathrm{cm} \\
b &= 2.10 \pm 0.02\ \mathrm{cm} \\
c &= 1.50 \pm 0.01\ \mathrm{cm}
\end{align}
$$

The goal is to calculate the density, derive the relative uncertainty formula using the total differential method, and identify the largest contributor to the uncertainty.

## Theory

For a function of the form $f = \frac{x}{y \cdot z \cdot w}$, the total differential method for absolute uncertainty is:

$$
u(f) = \sum \left| \frac{\partial f}{\partial x_i} \right| u(x_i)
$$

The relative uncertainty $\frac{u(f)}{f}$ for products and quotients is the sum of the relative uncertainties of the individual variables:

$$
\frac{u(\rho)}{\rho} = \frac{u(m)}{m} + \frac{u(a)}{a} + \frac{u(b)}{b} + \frac{u(c)}{c}
$$

## Step-by-Step Solution

Calculate the nominal value of the density:

$$
\rho = \frac{128.4}{5.20 \cdot 2.10 \cdot 1.50} = \frac{128.4}{16.38} \approx 7.8388\ \mathrm{g/cm^3}
$$

To derive the relative uncertainty formula, calculate the partial derivatives:

$$
\frac{\partial \rho}{\partial m} = \frac{1}{abc}, \quad \frac{\partial \rho}{\partial a} = -\frac{m}{a^2 bc}, \quad \frac{\partial \rho}{\partial b} = -\frac{m}{ab^2 c}, \quad \frac{\partial \rho}{\partial c} = -\frac{m}{abc^2}
$$

Applying the total differential:

$$
u(\rho) = \left| \frac{1}{abc} \right| u(m) + \left| \frac{m}{a^2 bc} \right| u(a) + \left| \frac{m}{ab^2 c} \right| u(b) + \left| \frac{m}{abc^2} \right| u(c)
$$

Dividing by $\rho = \frac{m}{abc}$ yields the relative uncertainty:

$$
\frac{u(\rho)}{\rho} = \frac{u(m)}{m} + \frac{u(a)}{a} + \frac{u(b)}{b} + \frac{u(c)}{c}
$$

Calculate the individual relative contributions:

$$
\begin{align}
\frac{u(m)}{m} &= \frac{0.2}{128.4} \approx 0.0016\ (0.16\%) \\
\frac{u(a)}{a} &= \frac{0.02}{5.20} \approx 0.0038\ (0.38\%) \\
\frac{u(b)}{b} &= \frac{0.02}{2.10} \approx 0.0095\ (0.95\%) \\
\frac{u(c)}{c} &= \frac{0.01}{1.50} \approx 0.0067\ (0.67\%)
\end{align}
$$

Total relative uncertainty:

$$
\frac{u(\rho)}{\rho} = 0.0016 + 0.0038 + 0.0095 + 0.0067 = 0.0216\ (2.16\%)
$$

Absolute uncertainty:

$$
u(\rho) = 7.8388 \cdot 0.0216 \approx 0.169\ \mathrm{g/cm^3}
$$

## Final Result

The density is:

$$
\rho = 7.84 \pm 0.17\ \mathrm{g/cm^3}
$$

## Interpretation

The relative uncertainty is approximately 2.2%. Comparing the contributions, the measurement of dimension $b$ (0.95%) gives the largest contribution to the uncertainty, followed by dimension $c$. The mass measurement has the smallest relative impact. To improve the result, more precise calipers should be used for the smaller dimensions.