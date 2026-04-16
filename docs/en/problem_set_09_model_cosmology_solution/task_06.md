# Task 06 – Two-body motion and the barycenter

## Problem Statement

Define the center of mass (barycenter) for a two-body system, prove its constant velocity in an isolated system, and set up the equations of motion.

## Theory

Consider two masses $m_1$ and $m_2$ at positions $\vec{r}_1$ and $\vec{r}_2$. The center of mass $\vec{R}$ is defined as:

$$
\vec{R} = \frac{m_1 \vec{r}_1 + m_2 \vec{r}_2}{m_1 + m_2}
$$

## Step-by-Step Solution

### 1. Conservation of Momentum

In an isolated system, the only forces are the internal gravitational forces $\vec{F}_{12}$ and $\vec{F}_{21}$. According to Newton's Third Law:

$$
\vec{F}_{12} = -\vec{F}_{21}
$$

The total force is:

$$
\vec{F}_{tot} = m_1 \ddot{\vec{r}}_1 + m_2 \ddot{\vec{r}}_2 = \frac{d^2}{dt^2}(m_1 \vec{r}_1 + m_2 \vec{r}_2) = 0
$$

Integrating once:

$$
m_1 \dot{\vec{r}}_1 + m_2 \dot{\vec{r}}_2 = \vec{P} = \text{const}
$$

Thus, the barycenter moves at a constant velocity.

### 2. Equations of Motion

The gravitational force exerted on $m_1$ by $m_2$ is:

$$
m_1 \ddot{\vec{r}}_1 = - G \frac{m_1 m_2}{|\vec{r}_1 - \vec{r}_2|^3} (\vec{r}_1 - \vec{r}_2)
$$

Similarly for $m_2$:

$$
m_2 \ddot{\vec{r}}_2 = - G \frac{m_1 m_2}{|\vec{r}_2 - \vec{r}_1|^3} (\vec{r}_2 - \vec{r}_1)
$$

### 3. Relative Motion

Defining the relative vector $\vec{r} = \vec{r}_1 - \vec{r}_2$, we can subtract the acceleration equations to find:

$$
\ddot{\vec{r}} = - G \frac{m_1 + m_2}{r^3} \vec{r}
$$

This reduces the two-body problem to an equivalent one-body problem with a reduced mass $\mu = \frac{m_1 m_2}{m_1 + m_2}$.

## Final Result

The system's motion is governed by:

$$
\begin{align}
\ddot{\vec{r}}_1 &= - G \frac{m_2}{|\vec{r}_1 - \vec{r}_2|^3} (\vec{r}_1 - \vec{r}_2) \\
\ddot{\vec{r}}_2 &= - G \frac{m_1}{|\vec{r}_2 - \vec{r}_1|^3} (\vec{r}_2 - \vec{r}_1)
\end{align}
$$

## Interpretation

If $m_1 \gg m_2$ (like the Sun and Earth), the barycenter $\vec{R}$ lies very close to the center of $m_1$. However, for binary stars of similar mass, both bodies visibly orbit a point in the empty space between them.