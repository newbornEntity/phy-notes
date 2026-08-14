# Electrostatic Potential and Capacitance - Class 12 Physics

> NCERT-aligned board notes with a JEE Main problem-solving layer  
> Source chapter: `leph102.pdf` (Chapter 2)  
> Syllabus basis checked: CBSE 2026-27 and JEE Main 2026, on 13 July 2026

## How to use these notes

| Tag | Meaning |
|---|---|
| **[B+J]** | Required for CBSE boards and explicitly relevant to JEE Main |
| **[B]** | Board-answer or derivation emphasis |
| **[J]** | JEE Main extension or problem-solving result |
| **[Scope note]** | Current reduced-syllabus boundary |

**Important:** JEE Main 2027 had not published its official syllabus by the preparation date. JEE tags provisionally use the latest official NTA syllabus, JEE Main 2026.

## Navigation

- [1. Exam scope](#1-exam-scope)
- [2. Potential and potential difference](#2-potential-and-potential-difference)
- [3. Potential due to common charge systems](#3-potential-due-to-common-charge-systems)
- [4. Relation between electric field and potential](#4-relation-between-electric-field-and-potential)
- [5. Equipotential surfaces](#5-equipotential-surfaces)
- [6. Electrostatic potential energy](#6-electrostatic-potential-energy)
- [7. Electrostatics of conductors](#7-electrostatics-of-conductors)
- [8. Dielectrics and polarisation](#8-dielectrics-and-polarisation)
- [9. Capacitors and capacitance](#9-capacitors-and-capacitance)
- [10. Parallel-plate capacitor and dielectrics](#10-parallel-plate-capacitor-and-dielectrics)
- [11. Capacitor combinations](#11-capacitor-combinations)
- [12. Energy stored in a capacitor](#12-energy-stored-in-a-capacitor)
- [13. Connected versus isolated capacitor](#13-connected-versus-isolated-capacitor)
- [14. Formula sheet](#14-formula-sheet)
- [15. Problem-solving playbook](#15-problem-solving-playbook)
- [16. Board derivation map](#16-board-derivation-map)
- [17. Common traps](#17-common-traps)
- [18. Last-minute checklist](#18-last-minute-checklist)

---

## 1. Exam scope

### CBSE 2026-27

Explicit scope:

- potential and potential difference;
- potential due to a point charge, dipole, and system of charges;
- equipotential surfaces;
- potential energy of two point charges and an electric dipole in a field;
- conductors, insulators, free and bound charges;
- dielectrics and polarisation;
- capacitors, series/parallel combinations;
- parallel-plate capacitance with and without dielectric;
- energy stored in a capacitor.

**Major reduced-syllabus instruction:** CBSE states **"energy stored in a capacitor - no derivation, formulae only."** Use the formulas in board numericals, but do not spend board-revision time memorising that derivation.

Electrostatics and Current Electricity form a shared 16-mark block in the course structure; no fixed chapter-wise split is promised.

### JEE Main 2026

The official electrostatics unit covers the same core ideas but does not impose CBSE's "no derivation" wording. JEE may combine energy, mechanical force, dielectric insertion, and capacitor networks.

### Scope exclusions

- Van de Graaff generator is not in the current official CBSE/JEE Main unit wording.
- Detailed microscopic dielectric theory is unnecessary; know polarisation and macroscopic effects.

---

## 2. Potential and potential difference

### 2.1 Electrostatic field is conservative **[B+J]**

Work done by an electrostatic field between two points is path-independent:

$$
\oint\vec E\cdot d\vec l=0
$$

Therefore a scalar potential can be defined.

### 2.2 Potential difference **[B+J]**

Potential difference between final point $B$ and initial point $A$ is work done per unit positive test charge by an external agent in slow transfer, with no kinetic-energy change:

$$
V_B-V_A=-\int_A^B\vec E\cdot d\vec l
$$

Equivalently, work done by the electric field is:

$$
W_{\text{field},A\to B}=q(V_A-V_B)
$$

### 2.3 Potential **[B+J]**

Taking $V(\infty)=0$ for a localised charge distribution:

$$
V(\vec r)=-\int_\infty^{\vec r}\vec E\cdot d\vec l
$$

Potential is scalar. SI unit:

$$
1\ \mathrm V=1\ \mathrm{J\,C^{-1}}
$$

Absolute potential depends on a chosen reference; physically measurable potential differences do not.

---

## 3. Potential due to common charge systems

### 3.1 Point charge **[B+J]**

$$
V(r)=\frac1{4\pi\varepsilon_0}\frac{q}{r}
$$

Potential has the sign of $q$. Unlike field, it is added algebraically.

### 3.2 System of point charges **[B+J]**

$$
V(\vec r)=\frac1{4\pi\varepsilon_0}
\sum_i\frac{q_i}{|\vec r-\vec r_i|}
$$

A zero potential point can have non-zero field because scalar cancellation does not imply vector cancellation.

### 3.3 Continuous charge distribution **[J support]**

$$
V=\frac1{4\pi\varepsilon_0}\int\frac{dq}{R}
$$

Potential integration is often easier than direct field integration because it has no vector components. Obtain field afterward from $\vec E=-\nabla V$.

### 3.4 Electric dipole **[B+J]**

Exact potential:

$$
V=\frac1{4\pi\varepsilon_0}
\left(\frac{q}{r_+}-\frac{q}{r_-}\right)
$$

where $r_+$ and $r_-$ are distances from $+q$ and $-q$.

For a short dipole at $r\gg$ separation:

$$
\boxed{V=\frac1{4\pi\varepsilon_0}\frac{\vec p\cdot\hat r}{r^2}}
$$

$$
V=\frac1{4\pi\varepsilon_0}\frac{p\cos\theta}{r^2}
$$

Special cases:

- Positive axial side, $\theta=0$: $V=+k_ep/r^2$.
- Negative axial side, $\theta=\pi$: $V=-k_ep/r^2$.
- Equatorial plane, $\theta=90^\circ$: $V=0$, even though $E\neq0$.

### 3.5 Uniformly charged ring on its axis **[J]**

For ring radius $R$, total charge $Q$, and axial distance $x$:

$$
V(x)=\frac1{4\pi\varepsilon_0}
\frac{Q}{\sqrt{x^2+R^2}}
$$

Then:

$$
E_x=-\frac{dV}{dx}=\frac1{4\pi\varepsilon_0}
\frac{Qx}{(x^2+R^2)^{3/2}}
$$

This is a standard continuous-distribution application, not a separate named CBSE derivation.

### 3.6 Thin spherical shell **[B+J application]**

For radius $R$ and total charge $Q$:

$$
V(r)=
\begin{cases}
k_eQ/r,&r\ge R\\
k_eQ/R,&r\le R
\end{cases}
$$

Potential is continuous at the surface, while its radial derivative and hence field change discontinuously for an ideal charged surface.

---

## 4. Relation between electric field and potential

### 4.1 One dimension/radial form **[B+J]**

$$
E_x=-\frac{dV}{dx}
$$

For radial symmetry:

$$
E_r=-\frac{dV}{dr}
$$

### 4.2 Vector form **[J]**

$$
\vec E=-\nabla V
$$

In Cartesian coordinates:

$$
\vec E=-\left(
\frac{\partial V}{\partial x}\hat i+
\frac{\partial V}{\partial y}\hat j+
\frac{\partial V}{\partial z}\hat k
\right)
$$

Meaning of the minus sign: electric field points toward the steepest decrease of potential.

### 4.3 Reading a $V$-position graph **[J]**

- Slope $dV/dx=0$ $\Rightarrow E_x=0$.
- Steeper magnitude of slope $\Rightarrow$ larger $|E_x|$.
- A potential maximum or minimum gives zero field at that point, but stability depends on the sign of the test charge and curvature of potential energy $U=qV$.

---

## 5. Equipotential surfaces

### 5.1 Definition and properties **[B+J]**

An equipotential surface has the same potential at every point.

1. Work moving a charge along it is zero:

$$
W=-q\Delta V=0
$$

2. Electric field is perpendicular to an equipotential surface.
3. Two equipotential surfaces cannot intersect.
4. Closer spacing means a stronger field for comparable potential intervals.
5. A conductor in electrostatic equilibrium is an equipotential body.

Examples:

- Point charge: concentric spherical surfaces.
- Uniform field: parallel planes perpendicular to $\vec E$.

---

## 6. Electrostatic potential energy

### 6.1 One charge in an external field **[B+J]**

$$
U=qV_{\mathrm{ext}}
$$

Only external-source potential is used; do not include a point charge's self-potential.

Change in potential energy:

$$
\Delta U=q(V_B-V_A)
$$

For slow movement:

$$
W_{\mathrm{external}}=\Delta U,
\qquad
W_{\mathrm{field}}=-\Delta U
$$

### 6.2 Two point charges **[B+J]**

Taking zero energy at infinite separation:

$$
U=\frac1{4\pi\varepsilon_0}\frac{q_1q_2}{r_{12}}
$$

- Like charges: $U>0$.
- Unlike charges: $U<0$.

### 6.3 System of point charges **[B+J]**

$$
U=\frac1{4\pi\varepsilon_0}
\sum_{i<j}\frac{q_iq_j}{r_{ij}}
$$

Each unordered pair is counted once.

Equivalent assembly expression:

$$
U=\frac12\sum_iq_iV_i
$$

where $V_i$ is potential at $q_i$ due to all the **other** charges.

### 6.4 Dipole in a uniform external field **[B+J]**

$$
\boxed{U=-\vec p\cdot\vec E=-pE\cos\theta}
$$

- Minimum $U=-pE$ at $\theta=0$: stable.
- Maximum $U=+pE$ at $\theta=\pi$: unstable.

Work by an external agent in slow rotation from $\theta_1$ to $\theta_2$:

$$
W_{\mathrm{ext}}=pE(\cos\theta_1-\cos\theta_2)
$$

Work by field is its negative.

---

## 7. Electrostatics of conductors

### 7.1 Properties in electrostatic equilibrium **[B+J]**

1. Electric field inside conducting material is zero.
2. Potential is constant throughout the conductor and on its surface.
3. Excess charge resides on the surface.
4. Electric field just outside is normal to the surface; no tangential component can remain.
5. Just outside a conductor in vacuum:

$$
E_n=\frac{\sigma}{\varepsilon_0}
$$

6. Surface charge density is greater at regions of smaller radius of curvature, producing stronger nearby fields.

### 7.2 Cavity and electrostatic shielding **[B+J]**

- An empty cavity inside a conductor, with no internal charge and no time-varying fields, has zero electrostatic field.
- External electrostatic fields do not penetrate the closed conducting enclosure under equilibrium conditions.
- If a charge $q$ is placed inside an isolated cavity without touching the conductor, total induced charge on the inner surface is $-q$. The outer-surface charge adjusts to conserve the conductor's total charge.

### 7.3 Electrostatic pressure **[J]**

Outward pressure on a conductor surface in vacuum:

$$
P=\frac{\sigma^2}{2\varepsilon_0}
=\frac12\varepsilon_0E^2
$$

Use the field just outside and remember the surface charge does not exert force on itself; the relevant average/other-charge field produces the factor $1/2$.

---

## 8. Dielectrics and polarisation

### 8.1 Free and bound charge **[B+J]**

- **Free charges:** can move over macroscopic distances, as in conductors.
- **Bound charges:** tied to atoms/molecules; they can shift slightly, producing polarisation.

### 8.2 Non-polar and polar molecules

- Non-polar molecules have no permanent dipole moment; an applied field induces one.
- Polar molecules have permanent dipole moments but are randomly oriented without a field; an applied field gives partial alignment against thermal disorder.

### 8.3 Polarisation vector **[B+J]**

Polarisation $\vec P$ is dipole moment per unit volume.

For a linear isotropic dielectric:

$$
\vec P=\varepsilon_0\chi_e\vec E
$$

$$
K=\varepsilon_r=1+\chi_e
$$

The dielectric's bound charges create a field opposing the applied field, reducing the net field for a fixed free charge.

### 8.4 Dielectric strength

Dielectric strength is the maximum field a dielectric can withstand without electrical breakdown. It is not the same as dielectric constant $K$.

---

## 9. Capacitors and capacitance

### 9.1 Capacitor **[B+J]**

A capacitor consists of two conductors separated by an insulator, arranged to store equal and opposite charges.

$$
C=\frac{Q}{V}
$$

- $Q$ is magnitude of charge on either conductor.
- $V$ is potential difference.
- SI unit: farad (F).

For a fixed linear dielectric geometry, $C$ depends on geometry and medium, not on instantaneous $Q$ or $V$.

### 9.2 Isolated spherical conductor **[J support]**

For sphere radius $R$ in vacuum:

$$
C=4\pi\varepsilon_0R
$$

This follows from $V=k_eQ/R$.

---

## 10. Parallel-plate capacitor and dielectrics

Ignore edge/fringing effects unless stated; this requires plate size much larger than separation.

### 10.1 Vacuum/air **[B+J]**

For plate area $A$ and separation $d$:

$$
E=\frac{\sigma}{\varepsilon_0}
$$

$$
V=Ed=\frac{Qd}{\varepsilon_0A}
$$

$$
\boxed{C_0=\frac{\varepsilon_0A}{d}}
$$

### 10.2 Completely filled dielectric **[B+J]**

$$
\boxed{C=K\frac{\varepsilon_0A}{d}=KC_0}
$$

### 10.3 Dielectric slab of thickness $t$ **[J]**

If slab covers full area but only thickness $t<d$:

$$
C=\frac{\varepsilon_0A}{(d-t)+t/K}
$$

Interpretation: air layer and dielectric layer behave like capacitors in series.

If a conducting slab of thickness $t$ is inserted without touching plates, field inside the slab is zero and effective gap is $d-t$:

$$
C=\frac{\varepsilon_0A}{d-t}
$$

### 10.4 Dielectric covering part of plate area **[J]**

If different regions share the same plate separation and potential difference, treat them as parallel capacitors:

$$
C=\sum_i\frac{\varepsilon_iA_i}{d}
$$

---

## 11. Capacitor combinations

### 11.1 Parallel **[B+J]**

Same potential across each; charges add:

$$
C_{\mathrm{eq}}=C_1+C_2+\cdots
$$

$$
Q_i=C_iV
$$

Equivalent capacitance exceeds the largest branch capacitance.

### 11.2 Series **[B+J]**

For initially uncharged capacitors connected in series, magnitude of charge is the same on each; voltages add:

$$
\frac1{C_{\mathrm{eq}}}=
\frac1{C_1}+\frac1{C_2}+\cdots
$$

$$
V_i=\frac{Q}{C_i}
$$

Smaller capacitance gets larger voltage. Equivalent capacitance is smaller than the smallest individual capacitance.

For two capacitors:

$$
C_{\mathrm{eq}}=\frac{C_1C_2}{C_1+C_2}
$$

### 11.3 Symmetric networks **[J]**

If symmetry guarantees two nodes have equal potential, no current/charge transfer is driven through a capacitor between those nodes; it can sometimes be ignored for equivalent-capacitance calculation. Establish symmetry before deleting anything.

---

## 12. Energy stored in a capacitor

### 12.1 Required formulas **[B+J]**

$$
\boxed{U=\frac12QV=\frac{Q^2}{2C}=\frac12CV^2}
$$

**CBSE scope note:** know and apply these formulas; derivation is explicitly not assessable for boards in 2026-27.

### 12.2 Energy density **[J; formula useful for boards]**

For a linear medium:

$$
u=\frac12\varepsilon E^2
$$

In vacuum:

$$
u=\frac12\varepsilon_0E^2
$$

The energy is regarded as stored in the electric field throughout the space between/around conductors.

### 12.3 Force between parallel plates **[J]**

At fixed charge in a uniform dielectric:

$$
F=\frac{Q^2}{2\varepsilon A}
=\frac12\varepsilon E^2A
$$

At fixed voltage:

$$
F=\frac12\frac{\varepsilon AV^2}{d^2}
$$

Force is attractive. Use an energy method only after identifying whether $Q$ or $V$ is held constant and whether a battery exchanges energy.

---

## 13. Connected versus isolated capacitor

Suppose a dielectric $K$ completely fills a capacitor initially having $C_0,Q_0,V_0,E_0,U_0$.

### 13.1 Battery disconnected: $Q$ constant **[B+J]**

| Quantity | Final value |
|---|---:|
| $C$ | $KC_0$ |
| $Q$ | $Q_0$ |
| $V$ | $V_0/K$ |
| $E$ | $E_0/K$ |
| $U$ | $U_0/K$ |

### 13.2 Battery connected: $V$ constant **[B+J]**

| Quantity | Final value |
|---|---:|
| $C$ | $KC_0$ |
| $V$ | $V_0$ |
| $Q$ | $KQ_0$ |
| $E=V/d$ | $E_0$ |
| $U$ | $KU_0$ |

The extra energy comes from the battery. A dielectric is pulled into a capacitor because the complete system tends toward lower appropriate energy; do not look only at capacitor field energy while ignoring battery work.

### 13.3 Changing plate separation **[J]**

For $C=\varepsilon A/d$:

- Isolated ($Q$ fixed), increasing $d$: $C\downarrow$, $V\uparrow$, $E=Q/(\varepsilon A)$ unchanged, $U\uparrow$.
- Connected ($V$ fixed), increasing $d$: $C\downarrow$, $Q\downarrow$, $E=V/d\downarrow$, capacitor energy $U\downarrow$.

---

## 14. Formula sheet

| Concept | Formula |
|---|---|
| Potential difference | $V_B-V_A=-\int_A^B\vec E\cdot d\vec l$ |
| Point potential | $V=k_eq/r$ |
| System potential | $V=k_e\sum q_i/r_i$ |
| Far dipole potential | $V=k_ep\cos\theta/r^2$ |
| Field-potential relation | $\vec E=-\nabla V$ |
| Two-charge energy | $U=k_eq_1q_2/r$ |
| Many-charge energy | $U=k_e\sum_{i<j}q_iq_j/r_{ij}$ |
| Dipole energy | $U=-\vec p\cdot\vec E$ |
| Capacitance | $C=Q/V$ |
| Parallel plate | $C=\varepsilon A/d$ |
| Series | $1/C_{\rm eq}=\sum1/C_i$ |
| Parallel | $C_{\rm eq}=\sum C_i$ |
| Capacitor energy | $U=Q^2/(2C)=QV/2=CV^2/2$ |
| Energy density | $u=\varepsilon E^2/2$ |
| Dielectric slab | $C=\varepsilon_0A/(d-t+t/K)$ |

---

## 15. Problem-solving playbook

### 15.1 Potential from charges

1. Choose the zero reference, normally infinity.
2. Find distance from observation point to every charge.
3. Add $k_eq_i/r_i$ algebraically.
4. Do not resolve potential into components.

### 15.2 Field from a given potential

1. Identify coordinate dependence.
2. Differentiate with respect to each coordinate.
3. Add the minus sign.
4. At discontinuities, use one-sided slopes/physical boundary conditions.

### 15.3 Energy of assembling charges

Count each pair exactly once. A safe method is to bring charges one at a time from infinity and sum the work; the first costs zero, the second interacts with the first, and so on.

### 15.4 Capacitor network

1. Mark nodes, not just visual shapes.
2. Identify elements with the same two nodes as parallel.
3. Identify true end-to-end branches with an otherwise isolated intermediate node as series.
4. Reduce stepwise.
5. Reconstruct charges/voltages from the source backward.

### 15.5 Dielectric or moving-plate question

Write at the top:

- battery connected $\Rightarrow V$ fixed;
- battery disconnected $\Rightarrow Q$ fixed.

Then choose $U=CV^2/2$ or $U=Q^2/(2C)$ accordingly.

### 15.6 Charge sharing **[J]**

When charged capacitors are connected with like plates together and no battery:

$$
Q_{\mathrm{total}}=\text{constant}
$$

Final common voltage:

$$
V_f=\frac{\sum C_iV_i\ \text{with algebraic plate signs}}{\sum C_i}
$$

Final electrostatic energy is usually smaller; the difference becomes heat/radiation during redistribution.

---

## 16. Board derivation map

Prepare:

1. Potential due to a point charge from line integration.
2. Potential due to a dipole and far-field form.
3. Potential energy of a two-charge/system configuration.
4. Potential energy of a dipole in a uniform field.
5. Capacitance of a parallel-plate capacitor without and with dielectric.
6. Series and parallel capacitor combinations.

Do **not** memorise the derivation of capacitor energy for CBSE 2026-27; the official syllabus says formulae only. Understanding the derivation can still help JEE reasoning.

---

## 17. Common traps

1. Treating potential as a vector.
2. Assuming $V=0$ implies $E=0$.
3. Forgetting the minus sign in $\vec E=-\nabla V$.
4. Using a charge's own potential in $U=qV_{\rm ext}$.
5. Double-counting pairs in system energy.
6. Reversing work done by field and external agent.
7. Taking dipole energy as $+pE\cos\theta$.
8. Saying field inside a conductor is zero because there are no charges anywhere; surface charges may exist.
9. Confusing dielectric constant with dielectric strength.
10. Saying capacitance changes merely because $Q$ or $V$ changes for fixed geometry/medium.
11. Treating a slab covering full area as a parallel combination; layers along field are series.
12. Assuming visual adjacency means capacitors are in series without checking nodes.
13. Forgetting that series capacitors carry equal charge magnitude, not equal voltage.
14. Forgetting the connected/disconnected condition during dielectric insertion.
15. Deriving capacitor energy in a CBSE answer when the question only asks the current syllabus's formula-level result.

---

## 18. Last-minute checklist

- [ ] I can calculate potential by scalar superposition.
- [ ] I know point, dipole, ring-axis, and shell potential results.
- [ ] I can obtain field from potential and read $V-x$ graphs.
- [ ] I know equipotential-surface properties.
- [ ] I can calculate energy of charges and a dipole.
- [ ] I can state all conductor properties and shielding facts.
- [ ] I understand polarisation and dielectric response.
- [ ] I can derive $C=\varepsilon A/d$ and reduce networks.
- [ ] I know all three equivalent capacitor-energy formulas.
- [ ] I distinguish fixed $Q$ from fixed $V$ before changing geometry/dielectric.
- [ ] I remember that CBSE requires energy formulas only, not their derivation.

## Official syllabus references

- [CBSE Physics syllabus 2026-27](https://cbseacademic.nic.in/web_material/CurriculumMain27/SecPart2/Physics_SecP2_2026-27.pdf)
- [NTA JEE Main 2026 syllabus page](https://jeemain.nta.nic.in/document/syllabus-2026/)
