# Task 09 – Three-body System

## Problem Statement

Establish the mathematical framework for the gravitational interaction of three point masses. Implement a numerical approach to solve the coupled differential equations and investigate the stability of the resulting trajectories.

## Theory

The three-body problem involves predicting the individual motions of three celestial objects interacting with each other gravitationally. Unlike the two-body problem, this system is generally non-integrable, meaning there is no general analytical solution in terms of standard algebraic functions.

The motion is governed by Newton's Law of Universal Gravitation. For any body $i$ in a system of $N$ bodies, the net force is the vector sum of the forces exerted by all other bodies $j$:

$$
\vec{F}_i = \sum_{j \neq i}^{N} \frac{G m_i m_j}{|\vec{r}_j - \vec{r}_i|^3} (\vec{r}_j - \vec{r}_i)
$$

## Step-by-Step Solution

### 1. Equations of Motion

For a system where $N=3$, we define the acceleration $\ddot{\vec{r}}_i$ for each mass $m_1, m_2, m_3$:

$$
\ddot{\vec{r}}_1 = G m_2 \frac{\vec{r}_2 - \vec{r}_1}{|\vec{r}_2 - \vec{r}_1|^3} + G m_3 \frac{\vec{r}_3 - \vec{r}_1}{|\vec{r}_3 - \vec{r}_1|^3}
$$

$$
\ddot{\vec{r}}_2 = G m_1 \frac{\vec{r}_1 - \vec{r}_2}{|\vec{r}_1 - \vec{r}_2|^3} + G m_3 \frac{\vec{r}_3 - \vec{r}_2}{|\vec{r}_3 - \vec{r}_2|^3}
$$

$$
\ddot{\vec{r}}_3 = G m_1 \frac{\vec{r}_1 - \vec{r}_3}{|\vec{r}_1 - \vec{r}_3|^3} + G m_2 \frac{\vec{r}_2 - \vec{r}_3}{|\vec{r}_2 - \vec{r}_3|^3}
$$

### 2. State-Space Representation

To solve these numerically, the three second-order vectors are decomposed into eighteen first-order ordinary differential equations (ODEs). Let the state vector $\mathbf{S}$ be:

$$
\mathbf{S} = [x_1, y_1, z_1, v_{x1}, v_{y1}, v_{z1}, \dots, v_{z3}]^T
$$

The derivative $\dot{\mathbf{S}}$ is then:

$$
\dot{\mathbf{S}} = [v_{x1}, v_{y1}, v_{z1}, a_{x1}, a_{y1}, a_{z1}, \dots, a_{z3}]^T
$$

### 3. Numerical Integration (RK4)

The Runge-Kutta 4th Order (RK4) method is applied to evolve the system over small time steps $\Delta t$. Given $\dot{\mathbf{S}} = f(t, \mathbf{S})$:

$$
\begin{align}
k_1 &= f(t_n, \mathbf{S}_n) \\
k_2 &= f(t_n + \frac{\Delta t}{2}, \mathbf{S}_n + \frac{\Delta t}{2} k_1) \\
k_3 &= f(t_n + \frac{\Delta t}{2}, \mathbf{S}_n + \frac{\Delta t}{2} k_2) \\
k_4 &= f(t_n + \Delta t, \mathbf{S}_n + \Delta t k_3)
\end{align}
$$

The next state is:

$$
\mathbf{S}_{n+1} = \mathbf{S}_n + \frac{\Delta t}{6}(k_1 + 2k_2 + 2k_3 + k_4)
$$

## Final Result

The implementation results in trajectories that are highly sensitive to initial conditions. Except for specific periodic solutions (such as the Lagrange points or the "figure-eight" orbit), most three-body configurations eventually lead to a "slingshot" effect where one body is ejected to infinity while the remaining two form a tightly bound binary.

## Interpretation

The three-body system serves as a fundamental example of deterministic chaos in physics. Although the governing laws are simple and fixed, the long-term behavior is unpredictable. This highlights the necessity of high-precision numerical methods and small time steps to maintain the conservation of energy and angular momentum.