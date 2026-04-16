# Task 05 – Kepler's Third Law

## Problem Statement

Analyze the relationship between the semi-major axis $a$ and the orbital period $T$ of planets to verify Kepler's Third Law.

## Theory

Kepler's Third Law states that the square of the orbital period of a planet is proportional to the cube of the semi-major axis of its orbit:

$$
T^2 = C a^3
$$

Where $C$ is a proportionality constant. In SI units, for a mass $M$ at the center:

$$
C = \frac{4\pi^2}{GM}
$$

## Step-by-Step Solution

### 1. Linearization

To perform linear regression, we transform the power-law relationship into a linear form. Taking the logarithm of both sides:

$$
2 \log(T) = \log(C) + 3 \log(a)
$$

Alternatively, we plot $y = T^2$ against $x = a^3$. If the law holds, the plot will be a straight line passing through the origin $(0,0)$.

### 2. Regression Analysis

By plotting $T^2$ vs $a^3$ for the planets in our solar system, we calculate the slope $C$ using the least squares method:

$$
C = \frac{\sum (a_i^3 T_i^2)}{\sum (a_i^3)^2}
$$

### 3. Goodness of Fit

The $R^2$ coefficient is calculated to determine how well the data follows the $T^2 \propto a^3$ rule. For the solar system, $R^2$ is extremely close to 1.0.

## Final Result

The proportionality constant $C$ for the solar system is approximately:

$$
C \approx 2.97 \times 10^{-19} \text{ s}^2/\text{m}^3
$$

## Interpretation

The consistency of $C$ across all planets confirms that they all orbit the same central mass (the Sun) and that the gravitational force follows the inverse-square law.