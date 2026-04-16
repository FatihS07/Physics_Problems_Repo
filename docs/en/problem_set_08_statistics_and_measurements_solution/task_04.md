# Task 04 – Linear regression and determination of $g$

## Problem Statement

The model for free fall is given by:

$$
h = \frac{1}{2} g t^2
$$

Based on the provided data for height $h$ and time $t$, determine the acceleration due to gravity $g$ using linear regression and estimate its uncertainty.

## Theory

To use linear regression, we transform the model into the form $y = kx$.
Let $y = h$ and $x = t^2$. Then the slope $k$ is:

$$
k = \frac{1}{2} g \implies g = 2k
$$

The slope $k$ for a line passing through the origin is calculated as:

$$
k = \frac{\sum x_i y_i}{\sum x_i^2}
$$

## Step-by-Step Solution

First, transform the time data into $t^2$:

$$
\begin{align}
t &= [0.202,\ 0.287,\ 0.351,\ 0.404,\ 0.452] \\
t^2 &= [0.0408,\ 0.0824,\ 0.1232,\ 0.1632,\ 0.2043]
\end{align}
$$

Perform regression for $h = k(t^2)$. Let $X = t^2$ and $Y = h$:

$$
\begin{align}
\sum X_i Y_i &= (0.0408 \cdot 0.20) + \dots + (0.2043 \cdot 1.00) \approx 0.4431 \\
\sum X_i^2 &= (0.0408)^2 + \dots + (0.2043)^2 \approx 0.0904
\end{align}
$$

The slope is:

$$
k = \frac{0.4431}{0.0904} \approx 4.9015
$$

Determine $g$:

$$
g = 2k = 2 \cdot 4.9015 = 9.803\ \mathrm{m/s^2}
$$

To estimate $u(g)$, calculate the standard error of the slope $s_k$. Using the residuals $d_i = Y_i - kX_i$:

$$
s_k = \sqrt{\frac{\sum d_i^2}{(n-1)\sum X_i^2}}
$$

Residuals squared $\sum d_i^2 \approx 0.00004$. This yields $s_k \approx 0.01$. Thus $u(g) = 2 \cdot s_k \approx 0.02$.

The coefficient of determination $R^2$ is calculated as:

$$
R^2 = 1 - \frac{\sum (Y_i - \hat{Y_i})^2}{\sum (Y_i - \bar{Y})^2}
$$

Given the near-zero residuals, $R^2 \approx 0.999$.

## Final Result

The acceleration due to gravity is:

$$
g = 9.80 \pm 0.02\ \mathrm{m/s^2}
$$

## Interpretation

The value $g \approx 9.80\ \mathrm{m/s^2}$ is consistent with the standard gravity on Earth ($9.81\ \mathrm{m/s^2}$). The high $R^2$ value indicates that the quadratic model $h \propto t^2$ describes the experimental data with high accuracy, confirming the laws of uniformly accelerated motion.