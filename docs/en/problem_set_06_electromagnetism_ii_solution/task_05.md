# Task 05 – Induction in a moving rod

## Problem Statement

A rod of length $L=0.25\,\mathrm{m}$ moves with velocity $v=4\,\mathrm{m/s}$ perpendicular to a uniform magnetic field $\vec B=0.6\,\mathrm{T}$. Determine the induced EMF $\mathcal{E}$, the potential difference, the effect of non-perpendicular motion, the dependence of $\mathcal{E}$ on $L$, and the origin of the electric field energy.

## Theory

When a conducting rod moves through a magnetic field, the free charges within the rod experience a Lorentz force. This force displaces the charges, creating an internal electric field that eventually balances the magnetic force, leading to a steady motional electromotive force (EMF) across the rod's ends.

The generalized motional EMF formula is:

$$
\mathcal{E} = \int (\vec v \times \vec B) \cdot d\vec l
$$

## Step-by-Step Solution

For a straight rod moving perpendicular to the magnetic field, the vectors $\vec v$, $\vec B$, and the rod length vector $\vec L$ are mutually orthogonal. The cross product $\vec v \times \vec B$ has a magnitude $vB$ and points along the rod.

Calculate the induced EMF:

$$
\mathcal{E} = v B L
$$

Substitute the given numerical values:

$$
\mathcal{E} = 4 \cdot 0.6 \cdot 0.25
$$

$$
\mathcal{E} = 0.6\ \mathrm{V}
$$

Determine the potential difference between the ends. In an open circuit (the rod alone), the equilibrium potential difference $\Delta V$ is exactly equal to the induced EMF:

$$
\Delta V = \mathcal{E} = 0.6\ \mathrm{V}
$$

Consider the case where the motion is not perpendicular to $\vec B$. If there is an angle $\theta$ between $\vec v$ and $\vec B$, the cross product magnitude is reduced:

$$
|\vec v \times \vec B| = v B \sin\theta
$$

If the rod itself is not aligned with the cross product direction (angle $\phi$), the dot product adds another projection:

$$
\mathcal{E} = (\vec v \times \vec B) \cdot \vec L = v B L \sin\theta \cos\phi
$$

Analyze the dependence of $\mathcal{E}$ on $L$. The formula $\mathcal{E} = v B L$ shows that the EMF is directly proportional to the length of the rod.

Address the origin of the energy. Moving the rod through the magnetic field separates the charges against the Coulomb attraction of the generated internal electric field. 

## Final Result

1. Induced EMF: $\mathcal{E} = 0.6\ \mathrm{V}$.
2. Potential difference: $\Delta V = 0.6\ \mathrm{V}$.
3. If not perpendicular, $\mathcal{E}$ is reduced according to the vector triple product $\mathcal{E} = (\vec v \times \vec B) \cdot \vec L$.
4. $\mathcal{E}$ is directly proportional to $L$.
5. The energy comes from the external mechanical work performed to keep the rod moving.

## Interpretation

Motional EMF acts like a battery. The Lorentz force separates the charges, creating electrical potential energy. To sustain this in a closed circuit, an external agent must continuously do work against the opposing magnetic braking force.