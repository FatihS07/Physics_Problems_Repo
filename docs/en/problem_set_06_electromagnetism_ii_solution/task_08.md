# Task 08 – Self-induction

## Problem Statement

An RL circuit with inductance $L=0.20\ \mathrm{H}$ and resistance $R=5.0\ \Omega$ is connected to $U=12\ \mathrm{V}$. The circuit reaches steady state and is then disconnected at $t=0$, forming a closed loop without the source. Determine the steady current, the transient current $I(t)$, the time constant, coil voltage, initial stored energy, prove the energy converts to Joule heat, and explain overvoltage.

## Theory

An inductor opposes changes in current by inducing a reverse electromotive force, a phenomenon known as self-induction. The self-induced EMF is proportional to the rate of change of current:

$$
\mathcal{E}_L = -L \frac{dI}{dt}
$$

When the external voltage source is removed but the circuit remains closed, the inductor acts as the energy source, driving a decaying current until its stored magnetic energy is depleted.

## Step-by-Step Solution

Determine the steady current $I_0$ before disconnection. In a steady state with direct current, the inductor acts as an ideal wire (zero resistance), so the current is limited only by the resistor:

$$
I_0 = \frac{U}{R} = \frac{12}{5.0} = 2.4\ \mathrm{A}
$$

Set up the circuit equation after disconnection. Kirchhoff's loop rule for the isolated LR circuit yields:

$$
-L \frac{dI}{dt} - I R = 0
$$

Solve the differential equation for $I(t)$:

$$
\frac{dI}{I} = -\frac{R}{L} dt
$$

Integrate both sides from $t=0$ where $I(0) = I_0$:

$$
\ln\left(\frac{I(t)}{I_0}\right) = -\frac{R}{L} t
$$

$$
I(t) = I_0 e^{-\frac{R}{L} t}
$$

Identify the time constant $\tau$:

$$
\tau = \frac{L}{R} = \frac{0.20}{5.0} = 0.04\ \mathrm{s}
$$

Calculate the voltage across the inductor $U_L(t)$:

$$
U_L(t) = -L \frac{dI}{dt} = -L \left( -I_0 \frac{R}{L} e^{-\frac{R}{L} t} \right) = I_0 R e^{-t/\tau}
$$

$$
U_L(t) = 12 e^{-25 t}\ \mathrm{V}
$$

Calculate the initial stored magnetic energy $W$:

$$
W = \frac{1}{2} L I_0^2 = 0.5 \cdot 0.20 \cdot (2.4)^2 = 0.576\ \mathrm{J}
$$

Show that this energy is converted into Joule heat. The total heat $Q$ dissipated in the resistor from $t=0$ to $t=\infty$ is the time integral of thermal power:

$$
Q = \int_0^\infty I^2(t) R dt
$$

Substitute the expression for $I(t)$:

$$
Q = \int_0^\infty \left( I_0 e^{-\frac{R}{L} t} \right)^2 R dt
$$

$$
Q = I_0^2 R \int_0^\infty e^{-\frac{2R}{L} t} dt
$$

Evaluate the integral:

$$
\begin{align}
Q &= I_0^2 R \left[ -\frac{L}{2R} e^{-\frac{2R}{L} t} \right]_0^\infty \\
&= I_0^2 R \left( 0 - \left( -\frac{L}{2R} \right) \right) \\
&= \frac{1}{2} L I_0^2
\end{align}
$$

This proves $Q = W$. 

Address the overvoltage phenomenon. If the circuit is broken physically (e.g., pulling a switch) rather than maintaining a closed loop, the current drops to zero almost instantly. A very small $dt$ creates an extremely large $dI/dt$. 

## Final Result

1. Steady current: $I_0 = 2.4\ \mathrm{A}$.
2. Transient current: $I(t) = 2.4 e^{-25t}\ \mathrm{A}$. Time constant: $\tau = 0.04\ \mathrm{s}$. Coil voltage: $U_L(t) = 12 e^{-25 t}\ \mathrm{V}$.
3. Stored energy: $W = 0.576\ \mathrm{J}$.
4. The integral of $I^2 R$ perfectly yields $\frac{1}{2} L I_0^2$.
5. Overvoltage occurs because an abrupt interruption of current forces a massive rate of change $dI/dt$, inducing a high voltage spike across the gap.

## Interpretation

An inductor provides electrical inertia. Just as mass resists abrupt changes in velocity, inductance resists abrupt changes in current. The stored energy acts as a temporary reservoir that smoothly powers the resistor until depletion. If interrupted abruptly, this inertia forces energy out as a high-voltage spark.