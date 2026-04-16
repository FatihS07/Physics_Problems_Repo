# Task 04 – Schrödinger equation (1D infinite potential well)

## Problem Statement

For a well of width $L$:

1. Write down the Schrödinger equation and the boundary conditions.
2. Derive the formula for the energy levels.
3. Calculate the ratio $E_2/E_1$.
4. How does the energy change when $L$ is doubled?
5. Where is the probability maximum for $n=1$?

## Theory

Inside the well ($0 < x < L$), the potential $V(x) = 0$. Outside, $V(x) = \infty$. The time-independent Schrödinger equation is:

$$
-\frac{\hbar^2}{2m} \frac{d^2\psi}{dx^2} = E\psi
$$

## Step-by-Step Solution

### 1. Schrödinger Equation and Boundaries
The equation is:

$$
\frac{d^2\psi}{dx^2} + k^2\psi = 0, \quad k^2 = \frac{2mE}{\hbar^2}
$$

Boundary conditions: $\psi(0) = 0$ and $\psi(L) = 0$.

### 2. Energy Level Derivation
The general solution is $\psi(x) = A \sin(kx) + B \cos(kx)$.
Applying $\psi(0)=0 \implies B=0$.
Applying $\psi(L)=0 \implies \sin(kL) = 0 \implies kL = n\pi$ for $n=1, 2, 3...$

Substituting $k$:

$$
\frac{2mE}{\hbar^2} = \left( \frac{n\pi}{L} \right)^2
$$

$$
E_n = \frac{n^2 \pi^2 \hbar^2}{2mL^2}
$$

### 3. Ratio E2/E1
Since $E_n \propto n^2$:

$$
\frac{E_2}{E_1} = \frac{2^2}{1^2} = 4
$$

### 4. Doubling L
Since $E_n \propto \frac{1}{L^2}$:
If $L \to 2L$, the energy becomes $E' = \frac{1}{4}E$. The energy levels decrease by a factor of 4.

## Final Result

* **Energy Levels:** $E_n = \frac{n^2 \pi^2 \hbar^2}{2mL^2}$
* **Ratio:** $E_2/E_1 = 4$

## Interpretation

5. **Probability Maximum ($n=1$):**
The wavefunction is $\psi_1(x) = \sqrt{\frac{2}{L}} \sin\left(\frac{\pi x}{L}\right)$. The probability density is $|\psi_1(x)|^2$. The maximum of $\sin^2$ occurs when the argument is $\pi/2$:

$$
\frac{\pi x}{L} = \frac{\pi}{2} \implies x = \frac{L}{2}
$$

The particle is most likely to be found in the center of the well.