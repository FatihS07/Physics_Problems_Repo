# Task 01 – Descriptive statistics of a measurement series

## Problem Statement

Given are the measurements of a rod's length (in cm):

$$
x = [12.10,\ 12.08,\ 12.12,\ 12.11,\ 12.09,\ 12.13,\ 12.07,\ 12.10]
$$

The goal is to calculate the arithmetic mean, sample standard deviation, and the uncertainty of the mean. Additionally, the intervals corresponding to confidence levels for a normal distribution must be determined and interpreted.

## Theory

The arithmetic mean represents the best estimate of the true value of the measured quantity:

$$
\bar{x} = \frac{1}{n} \sum_{i=1}^{n} x_i
$$

The sample variance quantifies the dispersion of individual measurements around the mean:

$$
s^2 = \frac{1}{n-1} \sum_{i=1}^{n} (x_i - \bar{x})^2
$$

The standard deviation $s$ is the square root of the variance. The uncertainty of the mean (also known as the standard error) describes the precision of the calculated mean:

$$
u(\bar{x}) = \frac{s}{\sqrt{n}}
$$

For a normal distribution, the probability that a single measurement falls within $\bar{x} \pm s$, $\bar{x} \pm 2s$, and $\bar{x} \pm 3s$ is approximately 68.3%, 95.4%, and 99.7%, respectively.

## Step-by-Step Solution

The dataset contains $n = 8$ measurements. The sum of the measurements is:

$$
\sum x_i = 12.10 + 12.08 + 12.12 + 12.11 + 12.09 + 12.13 + 12.07 + 12.10 = 96.80
$$

The arithmetic mean is:

$$
\bar{x} = \frac{96.80}{8} = 12.10 \text{ cm}
$$

Next, the deviations from the mean $(x_i - \bar{x})$ are calculated:

$$
0.00,\ -0.02,\ 0.02,\ 0.01,\ -0.01,\ 0.03,\ -0.03,\ 0.00
$$

Squaring these deviations yields:

$$
0.0000,\ 0.0004,\ 0.0004,\ 0.0001,\ 0.0001,\ 0.0009,\ 0.0009,\ 0.0000
$$

The sum of the squared deviations is:

$$
\sum (x_i - \bar{x})^2 = 0.0028 \text{ cm}^2
$$

The sample variance is:

$$
s^2 = \frac{0.0028}{8 - 1} = \frac{0.0028}{7} = 0.0004 \text{ cm}^2
$$

The standard deviation is:

$$
s = \sqrt{0.0004} = 0.02 \text{ cm}
$$

The uncertainty of the mean is:

$$
u(\bar{x}) = \frac{0.02}{\sqrt{8}} = \frac{0.02}{2.828} \approx 0.007 \text{ cm}
$$

To determine the confidence intervals assuming a normal distribution:

$$
\begin{align}
\bar{x} \pm s &= 12.10 \pm 0.02 \implies [12.08, 12.12] \\
\bar{x} \pm 2s &= 12.10 \pm 0.04 \implies [12.06, 12.14] \\
\bar{x} \pm 3s &= 12.10 \pm 0.06 \implies [12.04, 12.16]
\end{align}
$$

## Final Result

The measurement result, formatted with its uncertainty, is:

$$
x = 12.100 \pm 0.007 \text{ cm}
$$

The confidence intervals are:
* $\bar{x} \pm s = [12.08, 12.12]$ cm
* $\bar{x} \pm 2s = [12.06, 12.14]$ cm
* $\bar{x} \pm 3s = [12.04, 12.16]$ cm

## Interpretation

The standard deviation $s = 0.02$ cm characterizes the spread of the individual measurements; it indicates how much a single new measurement of the rod is expected to deviate from the mean. The uncertainty of the mean $u(\bar{x}) = 0.007$ cm characterizes the reliability of the calculated mean itself. As more measurements are taken, $u(\bar{x})$ decreases, while $s$ tends toward a stable constant value representing the intrinsic precision of the measuring instrument.

The intervals represent confidence levels based on the empirical rule of the normal distribution. Approximately 68% of individual readings are expected to fall within $[12.08, 12.12]$, 95% within $[12.06, 12.14]$, and over 99% within $[12.04, 12.16]$.