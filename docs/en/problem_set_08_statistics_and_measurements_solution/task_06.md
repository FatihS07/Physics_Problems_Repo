# Task 06 – Central Limit Theorem

## Problem Statement

The application simulates the distribution of the sample mean $\bar{x}$ for various source distributions.

## Theory

The Central Limit Theorem (CLT) states that for a sufficiently large sample size $n$, the distribution of the sample mean will be approximately normal, regardless of the original distribution's shape, provided the variance is finite. The expected standard deviation of the mean is $\sigma_{\bar{x}} = \sigma / \sqrt{n}$.

## Step-by-Step Solution (Analysis)

1.  **Effect of $n$:** As $n$ increases, the histogram of $\bar{x}$ becomes narrower and more symmetric (Gaussian).
2.  **Comparison:** The empirical standard deviation of the $N$ generated means aligns with the theoretical $\sigma/\sqrt{n}$.
3.  **Source Distributions:** Even for highly skewed distributions (like exponential), the mean distribution becomes normal as $n \to \infty$.

## Final Result

(The HTML file provides the interactive simulation and histogram.)

## Interpretation

The CLT is fundamental to statistics because it justifies using the normal distribution for uncertainty analysis even when the underlying physical process is not normally distributed.