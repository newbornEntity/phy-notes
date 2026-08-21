# 🧲 Chapter 6 — Electromagnetic Induction
### CBSE Class 12 Boards + JEE Main | Complete Study Notes
*Based on NCERT Physics Part 1, Chapter 6 (2026-27 reprint edition)*

> 📍 **Scope note:** Directly feeds into Ch. 7 (Alternating Current) — the AC generator equation derived here (§6.8) is the very source of the $v=v_m\sin\omega t$ assumed throughout Ch. 7. Expect derivation-based 3-mark questions (Faraday's law, motional emf, self/mutual inductance) and conceptual Assertion-Reason questions (Lenz's law, energy conservation).

---

## 🗂️ Table of Contents
1. [Introduction](#1-introduction)
2. [Experiments of Faraday and Henry](#2-experiments-of-faraday-and-henry)
3. [Magnetic Flux](#3-magnetic-flux)
4. [Faraday's Law of Induction](#4-faradays-law-of-induction)
5. [Lenz's Law and Conservation of Energy](#5-lenzs-law-and-conservation-of-energy)
6. [Motional EMF](#6-motional-emf)
7. [Inductance](#7-inductance)
8. [AC Generator](#8-ac-generator)
9. [Master Formula & Dimensions Table](#9-master-formula--dimensions-table)
10. [NCERT "Points to Ponder"](#10-ncert-points-to-ponder)
11. [Worked Examples — Quick Reference](#11-worked-examples--quick-reference)
12. [Practice Problems (Chapter-End Exercises)](#12-practice-problems-chapter-end-exercises)
13. [⚠️ NOT in this reduced NCERT chapter but relevant for JEE Main](#13-️-not-in-this-reduced-ncert-chapter-but-relevant-for-jee-main)
14. [One-Page Formula Cheat Sheet](#14-one-page-formula-cheat-sheet)

---

## 1. Introduction

- Early 1800s: **Oersted, Ampère** → moving charges (currents) produce a **magnetic field**.
- Natural follow-up question: Can moving **magnets** produce **electric currents**? (the converse effect)
- **~1830 — Michael Faraday (England) & Joseph Henry (USA)**: independently and conclusively showed that electric currents ARE induced in closed coils when subjected to **changing** magnetic fields.
- **Electromagnetic Induction**: the phenomenon of generating electric current (emf) using a **varying magnetic field**.
- This principle underlies **generators** and **transformers** — foundational to modern electrical civilization.

> 📝 Famous quote (occasionally asked in 1-mark GK-style Qs): When asked "What is the use of [this discovery]?", Faraday reportedly replied, **"What is the use of a new born baby?"**

---

## 2. Experiments of Faraday and Henry

*(Board-favorite: describe any one/all experiments with observations & conclusion — common 3-mark question)*

### Experiment 6.1 — Bar magnet + Coil
Coil $C_1$ connected to galvanometer G. A bar magnet's **N-pole** is pushed toward the coil.

| Observation | Conclusion |
|---|---|
| Galvanometer deflects when magnet is in motion | Current is induced |
| No deflection when magnet held stationary | No motion → no induction |
| Deflection reverses when magnet pulled away | Current direction reverses |
| S-pole gives opposite deflection to N-pole (for same motion) | Polarity matters |
| Faster motion → larger deflection | Rate of change matters |
| Same effects if magnet fixed & coil $C_1$ moved instead | **Relative motion** is what counts |

> ⭐ **Conclusion:** It is the **relative motion** between magnet and coil that induces current in the coil.

### Experiment 6.2 — Two coils, one current-carrying
Bar magnet replaced by a second coil $C_2$ (connected to a battery, carrying steady current → produces steady field). Moving $C_2$ toward/away from stationary $C_1$ (or vice-versa) reproduces the same deflection effects as Experiment 6.1.

> ⭐ **Conclusion:** Again, **relative motion between the coils** induces the current.

### Experiment 6.3 — Both coils stationary (key experiment!)
$C_1$ (connected to G) and $C_2$ (connected to battery via tapping key K) are both **held stationary**.

| Action | Observation |
|---|---|
| Key K **pressed** (current in $C_2$ rises 0→max) | **Momentary** deflection in G, returns to zero |
| Key **held pressed** (steady current in $C_2$) | **No** deflection |
| Key **released** (current in $C_2$ falls max→0) | Momentary deflection again, **opposite direction** |
| Iron rod inserted into the coils | Deflection increases dramatically |

> ⭐ **Key insight:** Relative motion is **NOT** an absolute requirement! What actually matters in **all three experiments** is: **the time rate of change of magnetic flux** through the circuit induces an emf. This is the unifying idea that leads to Faraday's Law.

---

## 3. Magnetic Flux

Defined analogously to electric flux. For a plane of area **A** in a uniform field **B**:

$$\Phi_B = \mathbf{B}\cdot\mathbf{A} = BA\cos\theta \tag{6.1}$$

where θ = angle between **B** and the area vector **A**.

For a curved surface / non-uniform field (sum over area elements):
$$\Phi_B = \mathbf{B_1}\cdot d\mathbf{A_1} + \mathbf{B_2}\cdot d\mathbf{A_2}+\cdots = \sum_{all}\mathbf{B_i}\cdot d\mathbf{A_i} \tag{6.2}$$

| Property | Value |
|---|---|
| Nature | **Scalar** quantity |
| SI Unit | **weber (Wb)** or **tesla·metre² (T·m²)** |
| Dimension | $[ML^2T^{-2}A^{-1}]$ |

> Flux can be changed by varying **any** of: **B** (field strength), **A** (area/shape of coil), or **θ** (orientation/angle) — this is the master key to solving every EMI problem: identify *which* of B, A, θ is changing.

---

## 4. Faraday's Law of Induction

> **Statement:** *The magnitude of the induced emf in a circuit is equal to the time rate of change of magnetic flux through the circuit.*

$$\boxed{\varepsilon = -\dfrac{d\Phi_B}{dt}} \tag{6.3}$$

For a **closely wound coil of N turns** (same flux change linked with every turn):

$$\boxed{\varepsilon = -N\dfrac{d\Phi_B}{dt}} \tag{6.4}$$

- The **negative sign** encodes the *direction* of the induced emf — this is **Lenz's Law** (Section 5).
- If the circuit is **closed** with resistance R: induced current $I = \varepsilon/R$.
- Induced emf can be increased by: increasing **N** (turns), increasing rate of change of B, A, or θ.

### 📌 Example 6.2 (numerical template — very testable)
Square loop (side 10 cm, R=0.5Ω) in east-west plane; B=0.10 T at 45° to loop plane (north-east direction), reduced to zero steadily in 0.70 s.
$$\Phi_{initial} = BA\cos45° = \dfrac{0.1\times10^{-2}}{\sqrt2}\text{ Wb} \implies \varepsilon = \dfrac{|\Delta\Phi_B|}{\Delta t} = 1.0\text{ mV}, \quad I = \varepsilon/R = 2\text{ mA}$$
> Note: Earth's magnetic field also threads the loop, but since it's **steady** (unchanging), it contributes **zero** to the induced emf — only *changing* flux matters.

### 📌 Example 6.3 — Coil rotated 180° (θ changes)
Circular coil (r=10cm, N=500, R=2Ω) rotated 180° about vertical diameter in 0.25 s in Earth's horizontal field $H_E=3.0\times10^{-5}$T.
$$\Phi_{initial}=BA\cos0°=+3\pi\times10^{-7}\text{Wb}, \quad \Phi_{final}=BA\cos180°=-3\pi\times10^{-7}\text{Wb}$$
$$\varepsilon = N\dfrac{\Delta\Phi}{\Delta t} = 3.8\times10^{-3}\text{ V}, \quad I=\varepsilon/R=1.9\times10^{-3}\text{A}$$
> ⚠️ Note these are only **average/estimated** values over the interval — the *instantaneous* emf varies with the instantaneous speed of rotation (this becomes the sinusoidal AC generator emf in §6.8!).

---

## 5. Lenz's Law and Conservation of Energy

> **Statement (Heinrich Lenz, 1834):** *The polarity of the induced emf is such that it tends to produce a current which opposes the change in magnetic flux that produced it.*

- This is exactly what the **negative sign** in Eq. (6.3)/(6.4) represents.

### Applying it to Experiment 6.1 (N-pole approaching coil):
- Flux through coil **increases** (as N-pole approaches) → induced current flows in a direction (**counter-clockwise**, viewed from the magnet's side) such that the coil's near face becomes an **effective N-pole** → **repels** the approaching magnet.
- If N-pole is **withdrawn**: flux decreases → induced current reverses (clockwise) → coil's near face becomes **S-pole** → **attracts** the receding magnet (opposing its departure).

> ⭐ Either way: the induced effect always **opposes the change**, never aids it.

### ⭐ Why Lenz's Law MUST be true — the perpetual motion argument (important conceptual/HOTS derivation)
- **Suppose** the induced current direction were *reversed* from Lenz's law (i.e., it *attracted* the approaching magnet instead of repelling it).
- Then the magnet would accelerate toward the coil **on its own**, gaining KE with **no energy input** — a **perpetual motion machine**.
- This **violates the law of conservation of energy** → impossible.
- **Correct picture:** the magnet experiences a **repulsive/opposing force**, so an external agent must **do work** to move the magnet — this work is exactly what gets **dissipated as Joule heating** ($I^2R$) by the induced current. Energy is conserved. ✅

### Open circuit case
Even with an **open** circuit, an emf is still induced across the open ends (just no current flows, since circuit isn't closed). Lenz's law is used to find the *polarity* of this emf.

> 📌 **Example 6.5(d)** — two bar magnets moving toward a capacitor plate arrangement between two coils: polarity is found by determining which plate the induced current would flow toward if the circuit were closed (via Lenz's law reasoning) → **plate 'A' is positive w.r.t. plate 'B'**.

### 📌 Example 6.4 — Direction of induced current in irregular loops (classic Lenz's law application)
Loops of different shapes moving into/out of a magnetic field region (field into the page):

| Loop | Motion | Flux change | Induced current direction |
|---|---|---|---|
| Rectangular abcd | moving **into** field | **increases** | flows along **bcdab** (opposes increase) |
| Triangular abc | moving **out** of field | **decreases** | flows along **bacb** (opposes decrease) |
| Irregular abcd | moving **out** of field | **decreases** | flows along **cdabc** (opposes decrease) |

> ⚠️ **No current is induced** when a loop is entirely **inside** or entirely **outside** the field region — only during the *transition* (when flux is actually changing) is current induced.

### 📌 Example 6.5 — Conceptual traps (VERY frequently recycled as Assertion-Reason / 1-markers)
**(a)** Stationary closed loop between fixed magnet poles (static field): No current, however strong the magnet — **current needs *changing* flux**, not merely the presence of a field.
**(b)** Loop moving through a constant **electric** field region (between capacitor plates): **No current induced** in either case (fully inside or partially outside) — **EMI is about changing magnetic flux, NOT electric flux.**
**(c)** Rectangular loop vs circular loop exiting a field region at constant velocity **v**: only the **rectangular** loop gives a **constant** induced emf (its rate of change of area, and hence flux, is constant as it exits at constant v); the circular loop's rate of area-change is **not** constant during exit → **non-constant (varying) emf**.

---

## 6. Motional EMF

**Setup:** Rectangular conductor PQRS, with rod PQ free to slide, moving with constant velocity **v** in a **uniform, time-independent** field **B** (perpendicular to the plane). Let RQ = x, RS = l.

$$\Phi_B = Blx$$

$$\varepsilon = -\dfrac{d\Phi_B}{dt} = -Bl\dfrac{dx}{dt} = Blv \tag{6.5}$$

$$\boxed{\varepsilon = Blv} \quad \text{— the } \textit{motional emf}$$

### Alternative derivation — via Lorentz Force (important 2nd method, sometimes explicitly asked)
- Any charge q in the moving rod PQ moves with speed v → experiences **Lorentz force** $F = qvB$ (directed along the rod, say toward Q).
- Work done moving charge from P to Q: $W = qvBl$
- $\varepsilon = W/q = Blv$ ✓ — identical to Eq. (6.5).

### ⭐ Deep conceptual point (frequently tested, "Points to Ponder" #3)
- For a **moving** conductor: the force on charges is explained by the **magnetic** part of the Lorentz force, $q(\mathbf v\times\mathbf B)$.
- For a **stationary** conductor in a **time-varying** B: since $\mathbf v=0$, $F=q(\mathbf E+\mathbf v\times\mathbf B)=q\mathbf E$ — the force **must** come from an **electric field E**.
- **Conclusion: a time-varying magnetic field generates an electric field.** (Caution: such induced E fields have different properties than electrostatic fields — e.g., their field lines are closed loops, not radiating from charges.) This is the deep unification underlying Faraday's law, and hints at the relevance of relativity (moving charges in a static field vs. stationary charges in a time-varying field are "symmetric" situations).

### 📌 Example 6.6 — Rotating rod (spoke) — VERY high-yield derivation (rod pivoted at one end)
Metallic rod length R=1m, rotated at ν=50 rev/s about one end (center), other end touching a ring; field B=1T along the axis.

**Method I** (integrate motional emf over each element $dr$ at radius r, speed $v=\omega r$):
$$d\varepsilon = Bv\,dr = B\omega r\,dr \implies \varepsilon = \int_0^R B\omega r\,dr = \dfrac{B\omega R^2}{2}$$

**Method II** (rate of change of swept area of sector, $\text{Area}=\tfrac12 R^2\theta$):
$$\varepsilon = B\dfrac{d}{dt}\left[\tfrac12R^2\theta\right] = \tfrac12BR^2\dfrac{d\theta}{dt} = \dfrac{B\omega R^2}{2}$$

$$\boxed{\varepsilon_{rotating\ rod} = \dfrac{1}{2}B\omega R^2}$$

Both methods agree: $\varepsilon = \tfrac12\times1.0\times(2\pi\times50)\times1^2 = 157\text{ V}$

> 🎯 **This formula ($\varepsilon=\tfrac12B\omega R^2$) is a JEE Main favorite** — appears in rotating rod/disc/wheel-spoke problems repeatedly.

### 📌 Example 6.7 — Wheel with spokes
Same formula applies to **each spoke** individually: $\varepsilon = \tfrac12\omega B R^2$. Since all spokes are effectively **in parallel** (same emf, same two end-points: axle & rim), the **number of spokes doesn't matter** for the emf value.

---

## 7. Inductance

- Flux linked with a coil is proportional to the current: $\Phi_B \propto I$ (for fixed coil geometry).
- For an N-turn coil, **flux linkage** $= N\Phi_B \propto I$; the proportionality constant is called **inductance**.
- Inductance depends only on **geometry** of the coil + **intrinsic material properties** (analogous to how capacitance depends on plate geometry + dielectric constant K).

| Property | Value |
|---|---|
| Nature | Scalar |
| Dimension | $[ML^2T^{-2}A^{-2}]$ |
| SI Unit | **henry (H)** *(named after Joseph Henry)* |

### 7.1 Mutual Inductance

**Setup:** Two long co-axial solenoids $S_1$ (radius $r_1$, turns/length $n_1$) and $S_2$ (radius $r_2$, turns/length $n_2$), both length *l*.

Current $I_2$ in $S_2$ → sets up flux through $S_1$:
$$N_1\Phi_1 = M_{12}I_2 \tag{6.7}$$

**Derivation:** Field due to $I_2$ inside $S_2$ is $B=\mu_0n_2I_2$ (uniform, since solenoid is long). Flux linkage with $S_1$ (only the portion inside $S_2$'s field matters):
$$N_1\Phi_1 = (n_1l)(\pi r_1^2)(\mu_0n_2I_2) = \mu_0n_1n_2\pi r_1^2 l\,I_2$$
$$\boxed{M_{12} = \mu_0n_1n_2\pi r_1^2 l} \tag{6.9}$$

**Reverse case** (current $I_1$ in $S_1$, flux linked with $S_2$ — but flux from $S_1$ is confined within $S_1$ since solenoids are long):
$$\boxed{M_{21} = \mu_0n_1n_2\pi r_1^2 l} \tag{6.11}$$

### ⭐ Reciprocity Theorem
$$\boxed{M_{12} = M_{21} = M} \tag{6.12}$$
> This holds far more generally than just for coaxial solenoids — extremely useful when one direction is easy to compute and the other is not (e.g., Example 6.8 below).

**With a medium of relative permeability $\mu_r$ filling the solenoids:**
$$M = \mu_r\mu_0n_1n_2\pi r_1^2 l$$

> Mutual inductance also depends on the **separation** and **relative orientation** of the two coils (not just their individual geometries).

### 📌 Example 6.8 — Concentric coils (classic JEE-style application of reciprocity)
Small coil (radius $r_1$) and large coil (radius $r_2$), $r_1\ll r_2$, coaxial, centers coinciding.
- Direct calc (current $I_2$ in outer coil, field at center $B_2=\mu_0I_2/2r_2$, assumed uniform over the tiny inner coil):
$$\Phi_1 = \pi r_1^2 B_2 = \dfrac{\mu_0\pi r_1^2}{2r_2}I_2 = M_{12}I_2 \implies M_{12}=\dfrac{\mu_0\pi r_1^2}{2r_2}$$
- By reciprocity: $M_{21}=M_{12}=\dfrac{\mu_0\pi r_1^2}{2r_2}$ — (computing $M_{21}$ directly would have been far harder, since B due to the small coil varies non-uniformly over the large coil!)

**Applying to Experiment 6.3:** varying current $I_2$ in coil $C_2$ induces emf in neighboring coil $C_1$:
$$\varepsilon_1 = -M\dfrac{dI_2}{dt}$$

### 7.2 Self-Inductance

Flux linkage of a coil due to **its own** current:
$$N\Phi_B = LI \tag{6.13}$$

$$\boxed{\varepsilon = -L\dfrac{dI}{dt}} \tag{6.14}$$

> The self-induced emf (also called **back emf**) always **opposes** any change (increase OR decrease) in the coil's own current.

**Self-inductance of a long solenoid** (cross-section area A, length *l*, n turns/unit length, field $B=\mu_0nI$):
$$N\Phi_B = (nl)(\mu_0nI)(A) = \mu_0n^2AlI$$
$$\boxed{L = \mu_0n^2Al} \tag{6.15}$$

**With core of relative permeability $\mu_r$** (e.g., soft iron):
$$\boxed{L = \mu_r\mu_0n^2Al} \tag{6.16}$$

### ⭐ Self-inductance = "Electrical Inertia" (favorite analogy question)
- L is the **electromagnetic analogue of mass (m)** in mechanics — it opposes/resists change (growth or decay) of current, just as mass resists change in velocity.
- Work must be done **against the back emf** to establish a current → this work is stored as **magnetic potential energy**.

**Energy stored derivation:**
$$\dfrac{dW}{dt}=|\varepsilon|I = LI\dfrac{dI}{dt} \implies W=\int_0^I LI\,dI$$
$$\boxed{W = \dfrac12LI^2} \tag{6.17}$$
*(Directly analogous to $\tfrac12mv^2$ — mechanical KE.)*

### General case — two coils with both self & mutual effects
$$N_1\Phi_1 = M_{11}I_1 + M_{12}I_2, \quad \text{where } M_{11}=L_1 \text{ (self-inductance)}$$
$$\varepsilon_1 = -L_1\dfrac{dI_1}{dt} - M_{12}\dfrac{dI_2}{dt}$$

### 📌 Example 6.9 — Magnetic energy density (important derivation, parallels electrostatics)
$$U_B = \tfrac12LI^2 = \tfrac12(\mu_0n^2Al)\left(\dfrac{B}{\mu_0n}\right)^2 = \dfrac{B^2Al}{2\mu_0}$$
$$\boxed{u_B = \dfrac{U_B}{\text{Volume}} = \dfrac{B^2}{2\mu_0}} \tag{6.18}$$

> **Compare with electrostatic energy density** (Ch. 2, Eq. 2.73): $u_E = \tfrac12\varepsilon_0E^2$.
> **Both energy densities are proportional to the square of the respective field strength** — and although each was derived for a special case (solenoid / parallel-plate capacitor), **both results are completely general**, valid in *any* region of space containing a magnetic and/or electric field. *(High-value conceptual comparison — commonly asked.)*

---

## 8. AC Generator

**Principle:** Mechanical energy → Electrical energy, via electromagnetic induction — specifically, by continuously changing a coil's **effective area** (i.e., changing **θ**, the angle between **A** and **B**) by **rotating** the coil in a magnetic field.

**Construction:** Coil (**armature**) mounted on a rotor shaft, rotated mechanically inside a uniform field **B**; ends connected to external circuit via **slip rings** and **brushes**.

**Derivation:**
At constant angular speed ω, with θ = ωt (θ=0 at t=0):
$$\Phi_B = BA\cos\theta = BA\cos\omega t$$

By Faraday's law, for N turns:
$$\varepsilon = -N\dfrac{d\Phi_B}{dt} = -NBA\dfrac{d}{dt}(\cos\omega t)$$

$$\boxed{\varepsilon = NBA\,\omega\sin\omega t} \tag{6.19}$$

Denoting the peak/maximum value $\varepsilon_0 = NBA\omega$:
$$\boxed{\varepsilon = \varepsilon_0\sin\omega t} \tag{6.20} \qquad = \varepsilon_0\sin(2\pi\nu t) \tag{6.21}$$

*(This is exactly the $v=v_m\sin\omega t$ ansatz used throughout Chapter 7 — AC generator is the **physical source** of sinusoidal ac voltage!)*

- The emf reaches its **maximum magnitude when θ=90° or 270°**, i.e., when the coil plane is **parallel** to B (rate of flux change is greatest there) — and is **zero when θ=0° or 180°** (coil plane ⊥ B, flux is at an extremum, momentarily not changing).
- Since current direction reverses periodically, this is called **alternating current (ac)**.

### Types of commercial generators
| Type | Mechanical energy source |
|---|---|
| **Hydro-electric** | Falling water (dams) |
| **Thermal** | Steam (from coal/other fuel) |
| **Nuclear power** | Steam from nuclear fuel |

- Modern generators: output up to **500 MW**.
- In most real generators, the **coil is held stationary** and the **electromagnets are rotated** instead (practically easier for high-power output).
- **Frequency of rotation:** **50 Hz in India**; **60 Hz** in USA and some other countries.

### 📌 Example 6.10 — Kamla's bicycle generator
N=100 turns, A=0.10 m², ν=0.5 Hz (half a revolution/sec), B=0.01 T:
$$\varepsilon_0 = NBA(2\pi\nu) = 100\times0.01\times0.1\times2\pi\times0.5 = 0.314\text{ V}$$

---

## 9. Master Formula & Dimensions Table

| Quantity | Symbol | Unit | Dimension | Key Equation |
|---|---|---|---|---|
| Magnetic Flux | $\Phi_B$ | Wb (weber) | $[ML^2T^{-2}A^{-1}]$ | $\Phi_B=\mathbf B\cdot\mathbf A$ |
| EMF | ε | V (volt) | $[ML^2T^{-3}A^{-1}]$ | $\varepsilon=-d(N\Phi_B)/dt$ |
| Mutual Inductance | M | H (henry) | $[ML^2T^{-2}A^{-2}]$ | $\varepsilon_1=-M_{12}(dI_2/dt)$ |
| Self Inductance | L | H (henry) | $[ML^2T^{-2}A^{-2}]$ | $\varepsilon=-L(dI/dt)$ |

---

## 10. NCERT "Points to Ponder"

1. Electricity & magnetism are intimately related: **Oersted/Ampère** (moving charges → magnetic field) and **Faraday/Henry** (moving/changing magnet → induced current) are two sides of the same coin.
2. In a **closed circuit**, induced current opposes the changing flux (law of conservation of energy). In an **open circuit**, an emf is still induced across the ends — NCERT poses this as an open conceptual question about how it relates to the flux change (answer: same $\varepsilon=-d\Phi/dt$ relation, simply no current flows since circuit isn't complete).
3. Motional emf can be derived two ways: (i) **Lorentz force** on moving charges (for a **moving** conductor in a static field), or (ii) assuming a **time-varying B field generates an E field** (for a **stationary** conductor in a changing field). These appear to be **symmetric situations**, hinting at a deep connection with the **principle of relativity**.

---

## 11. Worked Examples — Quick Reference

| Ex. | Setup | Key Answer(s) |
|---|---|---|
| 6.1 | Increasing deflection / detecting induced current without galvanometer | Soft iron core + powerful battery + faster motion; use a small bulb instead of galvanometer |
| 6.2 | Square loop (10cm, R=0.5Ω), B=0.10T at 45°, →0 in 0.70s | ε = 1.0 mV, I = 2 mA |
| 6.3 | Circular coil (r=10cm,N=500,R=2Ω) rotated 180° in 0.25s, $H_E=3.0\times10^{-5}$T | ε = 3.8×10⁻³ V, I = 1.9×10⁻³ A |
| 6.4 | Lenz's law direction — 3 loop shapes | bcdab / bacb / cdabc (opposing flux change in each case) |
| 6.5 | Conceptual: static field, electric flux, loop shapes, capacitor polarity | (a) No current (b) No current in either case (c) only rectangular loop → constant emf (d) plate A positive |
| 6.6 | Rotating rod, L=1m, ν=50 rev/s, B=1T | ε = ½BωR² = 157 V (2 methods) |
| 6.7 | Wheel, 10 spokes×0.5m, 120 rev/min, $H_E$=0.4G | ε = 6.28×10⁻⁵ V (spoke count irrelevant) |
| 6.8 | Concentric coils $r_1\ll r_2$ | $M_{12}=M_{21}=\mu_0\pi r_1^2/2r_2$ |
| 6.9 | Magnetic energy density in solenoid | $u_B = B^2/2\mu_0$; compare $u_E=\tfrac12\varepsilon_0E^2$ |
| 6.10 | Kamla's bicycle: N=100, A=0.1m², ν=0.5Hz, B=0.01T | $\varepsilon_0$ = 0.314 V |

---

## 12. Practice Problems (Chapter-End Exercises)

1. Predict the direction of induced current for six given figures (a)–(f) — coil/magnet motion, tapping key just closed/released, rheostat setting changed, current decreasing at steady rate. *(Practice applying Lenz's law systematically.)*
2. Use Lenz's law: (a) irregular wire loop turning into a circular shape (b) circular loop deformed into a narrow straight wire — predict induced current direction.
3. Long solenoid (15 turns/cm) with a small loop (area 2.0 cm²) inside, normal to axis. Solenoid current changes steadily 2.0 A → 4.0 A in 0.1 s. Find induced emf in the loop.
4. Rectangular wire loop (8 cm × 2 cm, with a small cut) moving out of a field region (B=0.3 T normal to loop) at 1 cm/s. Find emf across the cut when velocity is normal to (a) longer side (b) shorter side. How long does induced voltage last in each case?
5. 1.0 m metallic rod rotated at ω=400 rad/s about an axis through one end, other end touching a metallic ring; B=0.5 T along axis. Find emf between center and ring.
6. 10 m horizontal wire (east-west) falls at 5.0 m/s, ⊥ to Earth's horizontal field component (0.30×10⁻⁴ Wb/m²). Find: (a) instantaneous emf (b) direction of emf (c) which end is at higher potential.
7. Current falls 5.0 A → 0.0 A in 0.1 s, inducing average emf of 200 V. Estimate self-inductance of the circuit.
8. Pair of adjacent coils, M=1.5 H. Current in one changes 0→20 A in 0.5 s. Find change of flux linkage with the other coil.

> 💡 Tip: For Q.3–Q.8, directly apply the boxed formulas from Sections 4, 6, and 7 above.

---

## 13. ⚠️ NOT in this reduced NCERT chapter but relevant for JEE Main

This edition (2026-27 reprint) ends at §6.8 (AC Generator). A few classic EMI sub-topics that used to appear in the fuller NCERT chapter — or that are standard JEE Main extensions — are **not** covered here:

### (a) Eddy Currents *(fully removed from this edition — used to be §6.9)*
- **Definition:** When a **changing magnetic flux** links a **bulk piece of conductor** (not just a thin wire loop), induced currents circulate within the body of the conductor itself in closed loops resembling eddies in water — hence "eddy currents."
- Direction (by Lenz's law) always **opposes** the change causing them → results in a **retarding/damping force** and dissipates energy as heat.
- **Key applications (very commonly asked in JEE Main / NEET-style MCQs):**
  | Application | How eddy currents are used |
  |---|---|
  | **Electromagnetic braking** | Used in trains — strong eddy currents in a rotating drum/rail oppose motion, providing smooth braking without mechanical contact |
  | **Induction furnace** | High-frequency alternating field induces large eddy currents in a metal → heats and melts it |
  | **Electric/induction motors** | Eddy currents in the rotor are exploited to produce rotational torque |
  | **Magnetic damping (galvanometers)** | Aluminium/copper frame in moving-coil galvanometers uses eddy currents to quickly damp needle oscillations |
  | **Energy meters (electricity meters)** | Eddy currents in an aluminium disc used for speed regulation |
- **Reduction of eddy currents** (undesirable in transformer cores, motors): achieved using a **laminated core** *(cross-reference: this exact point survives in Ch. 7's transformer-losses section!)*.

### (b) Growth & Decay of Current in an LR Circuit
- Never explicitly derived in NCERT, but a standard JEE numerical topic:
$$\text{Growth: } I(t) = I_0\left(1-e^{-t/\tau}\right), \qquad \text{Decay: } I(t) = I_0\,e^{-t/\tau}$$
where the **time constant** $\tau = L/R$ (analogous to $\tau=RC$ for a capacitor charging/discharging).

### (c) Combination of Inductors
- **Series** (no mutual coupling): $L_{eq} = L_1+L_2+\cdots$
- **Parallel** (no mutual coupling): $\dfrac{1}{L_{eq}} = \dfrac{1}{L_1}+\dfrac{1}{L_2}+\cdots$
- **Series, with mutual inductance M**: $L_{eq} = L_1+L_2\pm2M$ (+ if fluxes aid, − if they oppose)
- **Coupling coefficient**: $k = \dfrac{M}{\sqrt{L_1L_2}}$ (0 ≤ k ≤ 1; k=1 for perfect/ideal coupling)

### (d) Extended Motional EMF Problems
- Rod sliding on frictionless horizontal/inclined **rails** connected by a resistor R at one end: induced current $I=Blv/R$, retarding force on rod $F=BIl=B^2l^2v/R$, leading to **terminal velocity** concepts (for a rod falling under gravity on vertical rails) and **power dissipated = power delivered by the external/gravitational force** (energy conservation check — good check-work for numericals).

> 🎯 **JEE Main takeaway:** Along with everything in Sections 1–8 above, make sure you're comfortable with **eddy current applications** (conceptual MCQs), the **LR circuit** growth/decay equations, and **rod-on-rails** motional emf numericals with retarding force/terminal velocity — these regularly appear in JEE Main despite being trimmed from (or never formally derived in) this NCERT edition.

---

## 14. One-Page Formula Cheat Sheet

```
MAGNETIC FLUX:        ΦB = B·A = BA cos θ                [Wb]

FARADAY'S LAW:         ε = −dΦB/dt          (single turn)
                      ε = −N dΦB/dt         (N turns)
                      I = ε/R                (closed circuit)

LENZ'S LAW:            Induced effects always OPPOSE the change in flux
                      (⇒ conservation of energy; − sign in Faraday's law)

MOTIONAL EMF:          ε = Blv          (rod of length l, speed v, field B ⊥ v,l)
                      Lorentz-force derivation: ε = W/q = Blv
                      Rotating rod (pivoted at one end): ε = ½ B ω R²

STATIONARY CHARGE
+ CHANGING B:          F = qE  (time-varying B induces an E field)

INDUCTANCE (general):   NΦB ∝ I  →  NΦB = (constant) × I

MUTUAL INDUCTANCE:      N1Φ1 = M12 I2 ;  N2Φ2 = M21 I1
                      M12 = M21 = M                (reciprocity)
                      Coaxial solenoids: M = μ0 n1 n2 π r1² l
                      (with core, permeability μr: M = μr μ0 n1 n2 π r1² l)
                      ε1 = −M (dI2/dt)

SELF INDUCTANCE:        NΦB = LI
                      ε = −L (dI/dt)                  (back emf)
                      Long solenoid: L = μ0 n² A l
                      (with core: L = μr μ0 n² A l)

ENERGY STORED:          W = ½ L I²          (analogous to ½mv²)
                      Energy density: uB = B² / 2μ0
                      (compare: uE = ½ ε0 E²  — electrostatic)

AC GENERATOR:           ΦB = BA cos ωt
                      ε = NBAω sin ωt = ε0 sin ωt = ε0 sin(2πνt)
                      ε0 = NBAω  (peak emf)
                      Max emf at θ=90°,270°;  Zero emf at θ=0°,180°
                      India: 50 Hz   |   USA: 60 Hz

[JEE EXTRA]  Eddy currents → braking, induction furnace, damping, energy meters
             LR circuit: I(t)=I0(1−e^(−t/τ)) growth, I0 e^(−t/τ) decay, τ=L/R
             L_series = L1+L2(±2M) | 1/L_parallel = 1/L1+1/L2
             Rod on rails: I=Blv/R, F=B²l²v/R (retarding), terminal velocity
```

---

*End of Chapter 6 notes. This pairs directly with the Chapter 7 (Alternating Current) notes already prepared — upload the next chapter's PDF whenever you're ready for a matching file.*
