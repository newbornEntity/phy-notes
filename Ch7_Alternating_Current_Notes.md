# ⚡ Chapter 7 — Alternating Current
### CBSE Class 12 Boards + JEE Main | Complete Study Notes
*Based on NCERT Physics Part 2, Chapter 7 (2026-27 reprint edition)*

> 📍 **Scope note:** This chapter is usually clubbed with Ch. 6 (EMI) under the **"Electromagnetic Induction & Alternating Current"** unit — one of the highest-weightage units in the electrodynamics section. Expect conceptual MCQs/Assertion-Reason, 2–3 mark derivations, and numerical/case-study questions on LCR circuits, resonance, and transformers.

---

## 🗂️ Table of Contents
1. [Introduction](#1-introduction)
2. [AC Voltage Applied to a Resistor](#2-ac-voltage-applied-to-a-resistor)
3. [Phasors](#3-phasors)
4. [AC Voltage Applied to an Inductor](#4-ac-voltage-applied-to-an-inductor)
5. [AC Voltage Applied to a Capacitor](#5-ac-voltage-applied-to-a-capacitor)
6. [Series LCR Circuit](#6-series-lcr-circuit)
7. [Resonance](#7-resonance)
8. [Power in AC Circuits — Power Factor](#8-power-in-ac-circuits--power-factor)
9. [Transformers](#9-transformers)
10. [Master Formula & Dimensions Table](#10-master-formula--dimensions-table)
11. [NCERT "Points to Ponder" (Conceptual Traps)](#11-points-to-ponder-conceptual-traps)
12. [Worked Examples — Quick Reference](#12-worked-examples--quick-reference)
13. [Practice Problems (Chapter-End Exercises)](#13-practice-problems-chapter-end-exercises)
14. [⚠️ NOT in this reduced NCERT chapter but relevant for JEE Main](#14-️-not-in-this-reduced-ncert-chapter-but-relevant-for-jee-main)
15. [One-Page Formula Cheat Sheet](#15-one-page-formula-cheat-sheet)

---

## 1. Introduction

- **DC**: current that does not change direction with time.
- **Alternating Voltage (ac voltage)**: potential difference that varies sinusoidally with time.
- **Alternating Current (ac current)**: current driven by ac voltage in a circuit.
- Household/mains supply voltage varies like a **sine function** of time.

**Why AC is preferred over DC for transmission:**
| Reason | Explanation |
|---|---|
| Easy voltage conversion | Transformers can step up/down ac voltage efficiently |
| Economical long-distance transmission | Step-up before transmission → lower current → lower I²R loss |
| Exploitable circuit properties | e.g., resonance used in radio tuning |

> 📝 Footnote (asked sometimes in 1-markers): The terms *"ac voltage"* and *"ac current"* are technically redundant/contradictory since "ac" itself means "alternating current," but the usage is universally accepted.

---

## 2. AC Voltage Applied to a Resistor

**Circuit:** Source ε connected to resistor R. Source symbol: ⊙

$$v = v_m \sin\omega t \tag{7.1}$$

Applying Kirchhoff's loop rule Σε(t) = 0:

$$v_m \sin\omega t = iR \implies i = i_m \sin\omega t \tag{7.2}$$

$$i_m = \dfrac{v_m}{R} \tag{7.3 — Ohm's law, works for both ac & dc}$$

### ⭐ Key Result: Voltage and current are **IN PHASE** (φ = 0) for a pure resistor.
- Both reach zero, minimum, maximum values simultaneously.

### Instantaneous & Average Power (Board favorite derivation)

Instantaneous power: 
$$p = i^2R = i_m^2 R\sin^2\omega t \tag{7.4}$$

Average over one cycle:
$$\bar p = i_m^2 R \langle \sin^2\omega t\rangle$$

Using $\sin^2\omega t = \tfrac12(1-\cos2\omega t)$ and $\langle\cos2\omega t\rangle = 0$:

$$\langle \sin^2\omega t\rangle = \tfrac12 \implies \bar p = \tfrac12 i_m^2 R \tag{7.5(c)}$$

> **Key insight:** Average current over a cycle is ZERO, but average **power is NOT zero** — because power depends on i² (always positive), not on i. This is Joule heating.

### RMS (Root Mean Square) / Effective Values — Very important definition

$$I = \sqrt{\overline{i^2}} = \dfrac{i_m}{\sqrt2} = 0.707\,i_m \tag{7.6}$$

$$V = \dfrac{v_m}{\sqrt2} = 0.707\,v_m \tag{7.8}$$

$$P = \bar p = \tfrac12 i_m^2R = I^2R \tag{7.7}$$

$$V = IR \tag{7.9}$$

> 💡 **Definition to remember for boards:** *RMS/effective current is that steady DC current which would produce the same average heating (power loss) in a resistor as the given AC does in one full cycle.*

- **All meter readings & rated values of ac quantities (220 V, 230 V, etc.) are RMS values**, not peak values.
- Peak voltage $v_m = \sqrt2\,V$

> ⚠️ **Note on numbers used in NCERT itself:** The book uses **220 V** in §7.2 examples (peak = 311 V) but switches to **240 V** in the Summary/"Points to Ponder" for the actual household supply (peak = 340 V). Both values appear in the official text — use whichever value the question specifies.

---

## 3. Phasors

- A **phasor** is a rotating vector of constant magnitude, rotating counter-clockwise about the origin with angular speed **ω**.
- **Magnitude** of phasor = amplitude/peak value ($v_m$ or $i_m$) of the oscillating quantity.
- **Vertical projection** of the phasor at any instant = instantaneous value of that quantity ($v_m\sin\omega t$ or $i_m\sin\omega t$).
- For a **pure resistor**: phasors **V** and **I** point in the **same direction at all times** → phase angle = 0.

> ⚠️ **Conceptual trap (often an Assertion-Reason Q):** Voltage and current are **scalar quantities**, NOT vectors. Phasors are just a geometric device — their amplitudes/phases combine mathematically the same way rotating-vector projections do, which is why the trick works, but v and i themselves are not "vectors."

---

## 4. AC Voltage Applied to an Inductor

**Assumption:** Pure inductor L, negligible resistance. Source: $v = v_m\sin\omega t$

Kirchhoff's loop rule (no resistor term):
$$v - L\dfrac{di}{dt} = 0 \tag{7.10}$$

$$\dfrac{di}{dt} = \dfrac{v}{L} = \dfrac{v_m}{L}\sin\omega t \tag{7.11}$$

**Integrating** (integration constant = 0, since current oscillates symmetrically about zero, no DC offset):

$$i = -\dfrac{v_m}{\omega L}\cos\omega t$$

Using $-\cos\omega t = \sin(\omega t - \pi/2)$:

$$\boxed{i = i_m\sin\left(\omega t - \dfrac{\pi}{2}\right)} \tag{7.12}$$

$$i_m = \dfrac{v_m}{\omega L} = \dfrac{v_m}{X_L}$$

### Inductive Reactance
$$X_L = \omega L \tag{7.13}$$
- SI unit: **ohm (Ω)** — same dimension as resistance.
- **Directly proportional** to L and to frequency ν (since ω = 2πν).
- At ω = 0 (DC), $X_L = 0$ → inductor behaves like a plain wire for steady DC.
- At ω → ∞, $X_L \to \infty$ → inductor blocks high frequencies.

### ⭐ Key Result: **Current LAGS voltage by π/2 (90°)**, i.e., by one-quarter cycle, in a pure inductor.
("**ELI**" mnemonic: in an inducto**L**, EMF/voltage leads Current → "ELI the ICE man")

### Average Power over one cycle
$$p_L = iv = -\dfrac{i_mv_m}{2}\sin(2\omega t)$$
$$\bar P_L = \left\langle -\dfrac{i_mv_m}{2}\sin2\omega t\right\rangle = 0$$

> **A pure inductor consumes ZERO average power** over a complete cycle (energy is stored in the magnetic field during one quarter-cycle and returned to the source in the next — no net dissipation).

📌 **Example 7.2 result** (for quick recall): L = 25.0 mH, V = 220 V, ν = 50 Hz → $X_L$ = 7.85 Ω, I = 28 A.

---

## 5. AC Voltage Applied to a Capacitor

**Circuit:** Source $v = v_m\sin\omega t$ connected only to capacitor C.

- In a **DC circuit**, a capacitor charges up, current flows briefly, then falls to zero once fully charged.
- In an **AC circuit**, the capacitor is continuously charged and discharged each half-cycle → allows continuous (but limited) current flow.

Instantaneous voltage across capacitor: $v = q/C$ (7.15)

From Kirchhoff's loop rule: $v_m\sin\omega t = q/C$

Using $i = dq/dt$:
$$i = \dfrac{d}{dt}(v_mC\sin\omega t) = \omega C v_m\cos\omega t$$

Using $\cos\omega t = \sin(\omega t + \pi/2)$:

$$\boxed{i = i_m\sin\left(\omega t + \dfrac{\pi}{2}\right)} \tag{7.16}$$

$$i_m = \omega C v_m = \dfrac{v_m}{1/\omega C} = \dfrac{v_m}{X_C}$$

### Capacitive Reactance
$$X_C = \dfrac{1}{\omega C} \tag{7.17}$$
- SI unit: ohm (Ω).
- **Inversely proportional** to C and to frequency.
- At ω = 0 (DC steady-state), $X_C \to \infty$ → capacitor blocks DC completely.
- At ω → ∞, $X_C \to 0$ → behaves like a short circuit at very high frequency.

### ⭐ Key Result: **Current LEADS voltage by π/2 (90°)** in a pure capacitor.
("**ICE**" mnemonic: in a **C**apacitor, Current leads EMF → "ELI the ICE man")

### Average Power
$$p_C = \dfrac{i_mv_m}{2}\sin(2\omega t) \implies \bar P_C = 0$$

> **A pure capacitor also consumes ZERO average power** over a complete cycle — same reasoning (energy stored in electric field, returned to source).

📌 **Example 7.3** (conceptual, frequently asked): Lamp in series with capacitor —
- **DC source**: capacitor charges then blocks current → lamp does **not** glow (regardless of C value).
- **AC source**: capacitor offers reactance $X_C$, current flows continuously → lamp **glows**.
- **Reducing C** → $X_C$ increases → current decreases → lamp glows **less brightly**.

📌 **Example 7.4 result**: C = 15.0 µF, 220 V, 50 Hz → $X_C$ = 212 Ω, $I_{rms}$ = 1.04 A, $i_m$ = 1.47 A.
- **If frequency is doubled** → $X_C$ is **halved** → current is **doubled**. (Very common numerical trick.)

---

## 6. Series LCR Circuit

**Circuit:** R, L, C all in series with source $v = v_m\sin\omega t$.

Kirchhoff's voltage law:
$$L\dfrac{di}{dt} + iR + \dfrac{q}{C} = v \tag{7.20}$$

Let current: $i = i_m\sin(\omega t + \phi)$ (7.21), where φ = phase difference between source voltage and circuit current.

### 6.1 Phasor-Diagram Method

Since it's a series circuit, current is common to all three elements (same amplitude & phase everywhere).

| Element | Phasor relation to I |
|---|---|
| $V_R$ | Parallel to **I** (in phase) |
| $V_L$ | π/2 **ahead** of **I** |
| $V_C$ | π/2 **behind** of **I** |

Amplitudes: $v_{Rm} = i_mR,\quad v_{Cm} = i_mX_C,\quad v_{Lm} = i_mX_L$ (7.22)

Since $V_L$ and $V_C$ are exactly opposite (antiparallel) phasors, they combine into a single phasor of magnitude $|v_{Cm}-v_{Lm}|$. Applying the Pythagorean theorem with $V_R$ as the other leg and **V** as hypotenuse:

$$v_m^2 = v_{Rm}^2 + (v_{Cm}-v_{Lm})^2 = i_m^2\left[R^2+(X_C-X_L)^2\right]$$

$$\boxed{i_m = \dfrac{v_m}{\sqrt{R^2+(X_C-X_L)^2}} = \dfrac{v_m}{Z}} \tag{7.25}$$

### Impedance
$$Z = \sqrt{R^2+(X_C-X_L)^2} \tag{7.26}$$
- SI unit: ohm (Ω). Plays the role of "AC resistance" for the whole circuit.

### Phase Angle
$$\tan\phi = \dfrac{X_C-X_L}{R} \tag{7.27}$$

**Impedance Triangle:** right triangle with base R, perpendicular $(X_C-X_L)$, hypotenuse Z.

| Condition | φ | Circuit nature | Current vs Voltage |
|---|---|---|---|
| $X_C > X_L$ | **positive** | predominantly **capacitive** | current **leads** voltage |
| $X_C < X_L$ | **negative** | predominantly **inductive** | current **lags** voltage |
| $X_C = X_L$ | **zero** | purely resistive (resonance) | in phase |

> ⚠️ **Conceptual note (important for boards):** The phasor method gives only the **steady-state solution**. It says nothing about initial conditions. A complete solution = transient solution (exists even when v = 0) + steady-state solution. After a long time, the transient dies out and only the steady-state (phasor) solution survives. *(NCERT explicitly states the analytical/calculus method exists but only presents the phasor method in this edition — see Section 14 below.)*

---

## 7. Resonance

**Concept:** Every LCR system driven at a frequency close to its "natural frequency" shows a large amplitude response — analogous to pushing a swing at its natural swinging frequency.

$$i_m = \dfrac{v_m}{Z} = \dfrac{v_m}{\sqrt{R^2+(X_C-X_L)^2}}$$

As ω is varied, impedance Z is **minimum** when $X_C = X_L$, i.e., $Z_{min} = R$.

This special frequency is the **resonant frequency**:
$$\dfrac{1}{\omega_0 C} = \omega_0 L \implies \boxed{\omega_0 = \dfrac{1}{\sqrt{LC}}} \tag{7.28}$$

**At resonance:**
- Impedance is **minimum**: Z = R
- Current amplitude is **maximum**: $i_m = v_m/R$
- Phase angle φ = 0 (current and voltage in phase)

### Graph: $i_m$ vs ω
- Sharp peak at $\omega = \omega_0$.
- **Smaller R → sharper/taller peak** (more selective).
- **Larger R → broader/shorter peak** (less selective).

### Application: Radio/TV Tuning
- Antenna signal drives the tuning circuit at many frequencies simultaneously.
- Varying the **capacitance** changes $\omega_0$ of the tuning circuit to match the desired station's frequency.
- Current (and hence signal strength) becomes maximum only for that station.

### ⭐ CRITICAL POINT (frequently tested):
> **Resonance requires BOTH L and C to be present in the circuit.** Only then can $V_L$ and $V_C$ (which are out of phase by π, i.e., opposite) cancel each other, leaving the full source voltage across R alone.
> **Resonance is NOT possible in a pure RL or pure RC circuit** — only in a **series RLC (or LC)** circuit.

📌 **Example 7.6 — The "voltage paradox" (very popular conceptual question):**
- R = 200 Ω, C = 15.0 µF, 220 V, 50 Hz (RC circuit) → Z = 291.67 Ω, I = 0.755 A
- $V_R = 151$ V, $V_C = 160.3$ V → algebraic sum = 311.3 V > 220 V (source voltage)!
- **Resolution:** $V_R$ and $V_C$ are 90° out of phase — they cannot be added arithmetically. Correct addition uses Pythagoras:
$$V_{R+C} = \sqrt{V_R^2+V_C^2} = 220\text{ V} ✓$$

📌 **Example 7.9 result** (same LCR values as Ex 7.8): At resonance, $\omega_0$ = 222.1 rad/s, $\nu_r$ = 35.4 Hz, Z = R = 3 Ω, I = 66.7 A, P = 13.35 kW (**greater than power dissipated off-resonance** in Ex 7.8, confirming max power at resonance).

📌 **Example 7.10 — Metal detector application:** Works on **resonance principle**. Walking through the coil (tuned to resonance with a capacitor) changes circuit impedance when metal is present → detectable change in current → triggers alarm circuitry.

---

## 8. Power in AC Circuits — Power Factor

For LCR circuit: $v = v_m\sin\omega t$, $i = i_m\sin(\omega t+\phi)$

$$p = vi = \dfrac{v_mi_m}{2}\left[\cos\phi - \cos(2\omega t+\phi)\right] \tag{7.29}$$

Averaging over a cycle (the time-dependent term averages to zero):

$$\boxed{P = \dfrac{v_mi_m}{2}\cos\phi = VI\cos\phi} \tag{7.30(a)}$$
$$P = I^2Z\cos\phi \tag{7.30(b)}$$

### Power Factor = $\cos\phi$

| Case | φ | cos φ | Power dissipated |
|---|---|---|---|
| **(i) Pure Resistive** | 0 | 1 | **Maximum** power dissipation |
| **(ii) Pure L or Pure C** | π/2 | 0 | **Zero** — current is called **"wattless current"** |
| **(iii) Series LCR (general)** | $\tan^{-1}\frac{X_C-X_L}{R}$, may be non-zero | between 0–1 | Power dissipated **only in R** |
| **(iv) At Resonance** | 0 | 1 | **Maximum**: $P = I^2Z = I^2R$ |

### 📌 Example 7.7 — Power factor & transmission losses (important applied concept)
**(a)** Since $P = IV\cos\phi$: to deliver a fixed power P at fixed V, if $\cos\phi$ is small → current I must be large → larger $I^2R$ loss in transmission lines. **Hence a low power factor is undesirable for power transmission.**

**(b)** **Improving power factor using a capacitor:**
- Resolve current **I** into two components: $I_p$ (in phase with V — the "power component") and $I_q$ (perpendicular to V — the **wattless component**).
- Adding a capacitor in parallel introduces a **leading** wattless current $I'_q$ that **cancels** the original **lagging** wattless current $I_q$.
- Net effect: $I_q$ and $I'_q$ cancel → $P \approx I_pV$ → power factor improves toward 1.
- This is the physics behind **power-factor correction capacitors** used in industrial installations.

---

## 9. Transformers

**Principle:** Mutual induction. Used to step up/down ac voltage.

**Construction:** Two coils (Primary — $N_p$ turns, Secondary — $N_s$ turns) wound on a common **soft-iron core** (either one over the other, or on separate limbs).

### Ideal Transformer Assumptions
1. Primary has **negligible resistance**.
2. **All flux** in the core links both windings (no leakage).
3. Secondary current/load draw is small (near open-circuit) — or 100% efficient.

**Derivation:**

Induced emf in secondary: $\varepsilon_s = -N_s\dfrac{d\phi}{dt}$ (7.31)

Back-emf in primary: $\varepsilon_p = -N_p\dfrac{d\phi}{dt} = v_p$ (7.32) *(equals applied voltage since primary resistance ≈ 0)*

Dividing:
$$\boxed{\dfrac{v_s}{v_p} = \dfrac{N_s}{N_p}} \tag{7.33}$$

**Assuming 100% efficiency** (power input = power output, since $p = iv$):
$$i_pv_p = i_sv_s \tag{7.34}$$

Combining (7.33) & (7.34):
$$\boxed{\dfrac{i_p}{i_s} = \dfrac{v_s}{v_p} = \dfrac{N_s}{N_p}} \tag{7.35}$$

So: 
$$V_s = \left(\dfrac{N_s}{N_p}\right)V_p \qquad I_s = \left(\dfrac{N_p}{N_s}\right)I_p \tag{7.36}$$

### Step-Up vs Step-Down

| Type | Turns ratio | Voltage | Current |
|---|---|---|---|
| **Step-up** | $N_s > N_p$ | $V_s > V_p$ (stepped up) | $I_s < I_p$ (reduced) |
| **Step-down** | $N_s < N_p$ | $V_s < V_p$ (stepped down) | $I_s > I_p$ (increased) |

> Example from NCERT: Primary 100 turns, secondary 200 turns → $N_s/N_p = 2$. A 220 V, 10 A input steps up to **440 V, 5.0 A** output. (Power in = Power out = 2200 W)

### Energy Losses in Real Transformers

| Loss | Cause | Reduction Method |
|---|---|---|
| **Flux leakage** | Not all flux from primary links secondary | Wind primary & secondary coils one over the other |
| **Resistance of windings** ($I^2R$) | Copper wire has resistance | Use thick wire, especially for high-current windings |
| **Eddy currents** | Alternating flux induces eddy currents in iron core | Use a **laminated** core |
| **Hysteresis** | Repeated magnetization reversal of core dissipates energy as heat | Use magnetic material with **low hysteresis loss** (e.g., soft iron) |

### Application: Power Transmission Chain
Generator voltage → **stepped up** (reduces current → cuts $I^2R$ loss) → transmitted over long distance → **stepped down** at area sub-station → further stepped down at distributing sub-stations/utility poles → ~230–240 V reaches homes.

---

## 10. Master Formula & Dimensions Table

| Quantity | Symbol | Formula | Dimension | SI Unit |
|---|---|---|---|---|
| RMS Voltage | V | $v_m/\sqrt2$ | $[ML^2T^{-3}A^{-1}]$ | V |
| RMS Current | I | $i_m/\sqrt2$ | $[A]$ | A |
| Inductive Reactance | $X_L$ | $\omega L$ | $[ML^2T^{-3}A^{-2}]$ | Ω |
| Capacitive Reactance | $X_C$ | $1/\omega C$ | $[ML^2T^{-3}A^{-2}]$ | Ω |
| Impedance | Z | $\sqrt{R^2+(X_C-X_L)^2}$ | $[ML^2T^{-3}A^{-2}]$ | Ω |
| Resonant frequency | $\omega_0$ | $1/\sqrt{LC}$ | $[T^{-1}]$ | Hz (rad/s) |
| Quality factor | Q | $\omega_0L/R = 1/(\omega_0CR)$ | Dimensionless | — |
| Power factor | $\cos\phi$ | R/Z | Dimensionless | — |

*(Note: Q-factor formula appears in the NCERT summary table but is **not derived** in the running text of this reduced chapter — see Section 14.)*

---

## 11. Points to Ponder (Conceptual Traps)

*(NCERT's own list — high-yield for Assertion-Reason & 1-mark conceptual MCQs)*

1. Quoted ac values (e.g., "220 V", "5 A") are, by convention, **RMS values**, not peak.
2. **Power rating** of an ac appliance = its **average power rating**.
3. Power consumed in an ac circuit is **never negative**.
4. AC ampere is defined via **Joule heating equivalence** (same heating effect as 1 A DC), not via the force-between-wires method used for DC.
5. Voltages across different elements **cannot be added algebraically** if out of phase — use phasor (Pythagorean) addition instead. E.g., in RC circuit, $V_{RC} = \sqrt{V_R^2+V_C^2} \ne V_R+V_C$.
6. Phasors represent **scalar** quantities (v, i) using a rotating-vector geometric trick — v and i are **not** actually vectors.
7. **No power loss** in pure L or pure C. Only the **resistive element** dissipates energy in an ac circuit.
8. Resonance ($X_L=X_C$, $\omega_0=1/\sqrt{LC}$) requires **both L and C**; impossible in RL-only or RC-only circuits.
9. Power factor is a measure of **how close the circuit is to delivering maximum possible power**.
10. In **motors**, electrical energy → mechanical energy (input→output); in **generators**, mechanical → electrical. Both merely *transform* energy (no creation).
11. A **step-up transformer does NOT violate energy conservation** — while voltage increases, current decreases proportionally (power stays ~constant).

---

## 12. Worked Examples — Quick Reference

| Ex. | Setup | Key Answer(s) |
|---|---|---|
| 7.1 | Bulb: 100 W, 220 V | R = 484 Ω, $v_m$ = 311 V, I = 0.454 A |
| 7.2 | L = 25 mH, 220 V, 50 Hz | $X_L$ = 7.85 Ω, I = 28 A |
| 7.3 | Lamp + capacitor, dc vs ac | DC → lamp off; AC → lamp glows; ↓C → dimmer |
| 7.4 | C = 15 µF, 220 V, 50 Hz | $X_C$=212 Ω, I=1.04 A, $i_m$=1.47 A; doubling ν halves $X_C$, doubles I |
| 7.5 | Bulb + inductor, iron rod inserted | L↑ → $X_L$↑ → bulb dims |
| 7.6 | R=200Ω, C=15µF, 220V, 50Hz | Z=291.67Ω, I=0.755A, $V_R$=151V, $V_C$=160.3V, Pythagorean sum=220V |
| 7.7 | Power factor theory | Low cosφ → high loss; capacitor cancels wattless current |
| 7.8 | $v_m$=283V, R=3Ω, L=25.48mH, C=796µF, 50Hz | $X_L$=8Ω, $X_C$=4Ω, Z=5Ω, φ=−53.1°, P=4800W, cosφ=0.6 |
| 7.9 | Same circuit as 7.8, at resonance | $\omega_0$=222.1 rad/s, $\nu_r$=35.4Hz, Z=R=3Ω, I=66.7A, P=13.35kW |
| 7.10 | Metal detector | Works on resonance principle |

---

## 13. Practice Problems (Chapter-End Exercises)

1. A 100 Ω resistor is connected to 220 V, 50 Hz ac. Find (a) rms current, (b) net power over a full cycle.
2. (a) Peak voltage = 300 V → find rms voltage. (b) rms current = 10 A → find peak current.
3. A 44 mH inductor connected to 220 V, 50 Hz ac. Find rms current.
4. A 60 µF capacitor connected to 110 V, 60 Hz ac. Find rms current.
5. For Q.3 and Q.4, find net power absorbed over a complete cycle. Explain.
6. A charged 30 µF capacitor connected to a 27 mH inductor. Find angular frequency of free oscillations. *(Uses ω₀=1/√LC even though this is an LC-only circuit — see Section 14.)*
7. Series LCR: R=20Ω, L=1.5H, C=35µF, connected to 200V variable-frequency ac. At resonance, find average power transferred per cycle.
8. Series LCR circuit, 230 V variable-frequency source, L=5.0H, C=80µF, R=40Ω. Find: (a) resonant source frequency, (b) impedance & current amplitude at resonance, (c) rms voltage drops across R, L, C — show $V_{LC}$ combination = 0 at resonance.

> 💡 Try solving these using the boxed formulas above before checking against Examples 7.1–7.9 for method.

---

## 14. ⚠️ NOT in this reduced NCERT chapter but relevant for JEE Main

The current (rationalized) NCERT chapter has **removed** a few classic sub-topics that used to be part of the full "Alternating Current" chapter. **CBSE boards will NOT test these**, but **JEE Main syllabus still nominally includes AC as a full topic**, and these ideas occasionally appear in JEE Main/similar competitive exams, so know them at a basic level:

### (a) LC Oscillations
- A charged capacitor connected to an inductor (no resistor) undergoes **electrical oscillations**: energy shuttles between the capacitor's electric field and the inductor's magnetic field.
- Governing equation: $L\dfrac{di}{dt}+\dfrac{q}{C}=0$, analogous to SHM.
- Natural (angular) frequency of these **undamped free oscillations**:
$$\omega_0 = \dfrac{1}{\sqrt{LC}}$$
- This is exactly the *resonant frequency* formula of the LCR circuit (Eq. 7.28) — the LC circuit is the "natural oscillator," and driving an LCR circuit at this same frequency is what produces resonance.
- Total energy $\left(\frac{1}{2}Li^2 + \frac{q^2}{2C}\right)$ remains constant (ideal, resistanceless case) — in a real LC circuit, resistance causes **damped oscillations**.
- ⚠️ **Chapter-end Exercise 7.6** ("charged 30 µF capacitor connected to 27 mH inductor — find angular frequency of free oscillations") is actually **based on this removed topic**, even though it appears in this reduced chapter's exercise list!

### (b) AC Generator (Dynamo) — now taught under Ch. 6 (EMI)
- A coil of N turns, area A, rotating with angular velocity ω in uniform magnetic field B generates:
$$e = NBA\omega\sin\omega t = e_0\sin\omega t, \quad e_0 = NBA\omega$$
- This is the physical origin of the sinusoidal EMF assumed throughout this chapter ($v=v_m\sin\omega t$).
- Based on **electromagnetic induction / motional emf**, energy conversion: mechanical → electrical.

### (c) Sharpness of Resonance, Q-Factor, and Bandwidth
- **Quality factor**: $Q = \dfrac{\omega_0L}{R} = \dfrac{1}{\omega_0CR}$ (appears in NCERT's own summary table but is undeveloped in text).
- **Bandwidth** (range of ω over which power ≥ half of max power, i.e., "half-power points"): $\Delta\omega = \dfrac{R}{L}$
- Relation: $Q = \dfrac{\omega_0}{\Delta\omega}$
- **Higher Q → sharper/narrower resonance peak → smaller R → more selective circuit** (important for radio tuning quality).

### (d) Choke Coil
- A **high-inductance, low-resistance** coil (ideally pure L) used in series with ac appliances (e.g., old-style fluorescent tube ballasts) to **limit/reduce current without dissipating power** (since pure L has cosφ ≈ 0 → near-zero power loss), unlike using a resistor which would waste power as heat.

### (e) Analytical (Calculus-based) Solution of the LCR Differential Equation
- NCERT's own text (§7.6) explicitly promises "we solve this problem by two methods... second method solve Eq. (7.20) analytically" — but **only the phasor method is actually presented** in this reduced edition. The full analytical (differential equation) solution has been dropped. JEE numericals rarely need this method directly since the phasor-derived formulas suffice, but conceptually be aware the impedance/phase results can also be derived by directly solving the LCR differential equation.

> 🎯 **JEE Main takeaway:** Master formulas $\omega_0=1/\sqrt{LC}$, $Q=\omega_0L/R$, $\Delta\omega = R/L$, and the AC generator EMF equation $e=e_0\sin\omega t$ (with $e_0=NBA\omega$) in addition to everything in Sections 1–9 above — these bridge the gap between the trimmed NCERT chapter and the fuller JEE Main syllabus.

---

## 15. One-Page Formula Cheat Sheet

```
GENERAL:            v = vm sin ωt,  ω = 2πν = 2π/T

RESISTOR:            i = im sin ωt         [in phase]
                     im = vm/R
                     P̄ = (1/2)im²R = I²R

RMS VALUES:           I = im/√2  = 0.707 im
                     V = vm/√2  = 0.707 vm
                     P = VI = I²R

INDUCTOR:            i = im sin(ωt − π/2)   [I lags V by 90°]
                     XL = ωL
                     im = vm/XL
                     P̄L = 0

CAPACITOR:           i = im sin(ωt + π/2)   [I leads V by 90°]
                     XC = 1/ωC
                     im = vm/XC
                     P̄C = 0

SERIES LCR:           i = im sin(ωt + φ)
                     Z  = √[R² + (XC − XL)²]
                     im = vm/Z
                     tanφ = (XC − XL)/R
                     XC>XL → φ>0 → capacitive, I leads V
                     XC<XL → φ<0 → inductive, I lags V

RESONANCE:            ω0 = 1/√(LC)   (Xc = XL)
                     Zmin = R,   im(max) = vm/R,   φ = 0
                     Needs BOTH L & C present

POWER:               P = VI cosφ = I²Z cosφ
                     cosφ = power factor = R/Z
                     Pure R: cosφ=1 (max)
                     Pure L/C: cosφ=0 (wattless current)
                     Resonance: cosφ=1, P=I²R (max)

TRANSFORMER:          Vs/Vp = Ns/Np           (voltage ratio)
                     Is/Ip = Np/Ns           (current ratio, inverse)
                     Step-up:  Ns>Np → Vs>Vp, Is<Ip
                     Step-down: Ns<Np → Vs<Vp, Is>Ip
                     Ideal: ip vp = is vs  (power conserved)

[JEE EXTRA]  LC oscillation ω0 = 1/√LC | AC generator e = NBAω sinωt
             Q = ω0L/R = 1/(ω0CR)     | Bandwidth Δω = R/L
```

---

*End of Chapter 7 notes. Upload the next chapter's PDF and I'll prepare a separate, matching notes file for it.*
