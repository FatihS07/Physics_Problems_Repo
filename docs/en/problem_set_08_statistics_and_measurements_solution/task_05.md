# Task 05 – Systematic vs. statistical errors

## Problem Statement

Analyze the measurements of three groups (A, B, C) for a rod with a true length $x_{\mathrm{true}} = 10.00$.

## Theory

* **Statistical error:** Random fluctuations; reduced by increasing $n$.
* **Systematic error:** Consistent offset from the true value; not reduced by increasing $n$.
* **Accuracy:** How close the mean is to the true value.
* **Precision:** How small the standard deviation is.

## Step-by-Step Solution

### 1. Calculations

| Group | Mean $\bar{x}$ | Std Dev $s$ | $u(\bar{x})$ |
| :--- | :--- | :--- | :--- |
| **A** | 10.00 | 0.016 | 0.007 |
| **B** | 10.41 | 0.016 | 0.007 |
| **C** | 10.10 | 0.380 | 0.170 |

### 2. Comparison with True Value

* **Group A:** Result $10.00 \pm 0.01$. Matches $x_{\mathrm{true}}$.
* **Group B:** Result $10.41 \pm 0.01$. Does not match $x_{\mathrm{true}}$.
* **Group C:** Result $10.10 \pm 0.17$. Matches $x_{\mathrm{true}}$ within the uncertainty interval.

## Final Result

* **Group A:** Accurate and precise. Statistical error dominates but is small.
* **Group B:** Precise but inaccurate. Significant systematic error ($\approx +0.41$).
* **Group C:** Accurate but imprecise. Large statistical error.

## Interpretation

**Systematic error causes:**
1. Zero-point error (e.g., the ruler starts at 1mm instead of 0).
2. Environmental factors (e.g., thermal expansion of the rod).

**Increasing measurements:**
This reduces $u(\bar{x})$ (statistical error) because fluctuations average out. It does not eliminate systematic error because the offset is constant for every measurement.

**Comparison of Results:**
The result $x = 10.00 \pm 0.20$ is "better" in a scientific sense because it is **truthful**. The result $x = 10.41 \pm 0.01$ is highly precise but **wrong**, which can lead to dangerous errors in engineering.