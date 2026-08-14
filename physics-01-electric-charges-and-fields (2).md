# Electric Charges and Fields - Class 12 Physics

> NCERT-aligned board notes with a JEE Main problem-solving layer  
> Source chapter: `leph101(1).pdf` (Chapter 1)  
> Syllabus basis checked: CBSE 2026-27 and JEE Main 2026, on 13 July 2026

## How to use these notes

| Tag | Meaning |
|---|---|
| **[B+J]** | Required for CBSE boards and explicitly relevant to JEE Main |
| **[B]** | Board-answer or derivation emphasis |
| **[J]** | JEE Main extension or fast problem result |
| **[Scope note]** | Current reduced-syllabus boundary |

**Important:** JEE Main 2027 had not published its official syllabus by the preparation date. The latest official NTA syllabus, JEE Main 2026, is used provisionally.

## Navigation

- [1. Exam scope](#1-exam-scope)
- [2. Electric charge and its properties](#2-electric-charge-and-its-properties)
- [3. Conductors, insulators, and charging](#3-conductors-insulators-and-charging)
- [4. Coulomb's law](#4-coulombs-law)
- [5. Superposition principle](#5-superposition-principle)
- [6. Electric field](#6-electric-field)
- [7. Electric field lines](#7-electric-field-lines)
- [8. Electric dipole](#8-electric-dipole)
- [9. Electric flux](#9-electric-flux)
- [10. Continuous charge distributions](#10-continuous-charge-distributions)
- [11. Gauss's law](#11-gausss-law)
- [12. Standard Gaussian-law results](#12-standard-gaussian-law-results)
- [13. Formula sheet](#13-formula-sheet)
- [14. Problem-solving playbook](#14-problem-solving-playbook)
- [15. Board derivations](#15-board-derivations)
- [16. Common traps](#16-common-traps)
- [17. Last-minute checklist](#17-last-minute-checklist)

---

## 1. Exam scope

### CBSE 2026-27

The official scope explicitly includes charge and its conservation, Coulomb's law, multiple and continuous charge distributions, electric field and field lines, dipole field and torque, electric flux, Gauss's theorem, and applications to:

- an infinitely long uniformly charged wire;
- a uniformly charged infinite plane sheet;
- a uniformly charged thin spherical shell, inside and outside.

CBSE places Electrostatics and Current Electricity in a **shared 16-mark block** in the course structure; it does not promise a fixed chapter-wise mark split.

### JEE Main 2026

The electrostatics wording for this chapter is effectively the same. JEE questions more often combine symmetry, vector addition, equilibrium, and graphs in one problem.

### Scope note

Every major section in this uploaded reduced NCERT chapter is in current scope. Results for finite rods/rings or non-uniform distributions are useful JEE applications of the stated continuous-distribution syllabus, even when not separate CBSE headings.

---

## 2. Electric charge and its properties

### 2.1 Two kinds of charge **[B+J]**

- Like charges repel; unlike charges attract.
- Charge is a scalar, even though the force it produces is a vector.
- SI unit: coulomb (C).
- Elementary charge magnitude:

$$
e=1.602176634\times10^{-19}\ \mathrm C
$$

Electron has charge $-e$ and proton has charge $+e$.

### 2.2 Additivity **[B+J]**

Total charge is the algebraic sum:

$$
Q=\sum_i q_i
$$

No vector addition is involved for charge.

### 2.3 Conservation **[B+J]**

The net electric charge of an isolated system remains constant. Charging transfers charge; it does not create net charge from nothing.

### 2.4 Quantisation **[B+J]**

$$
q=ne,\qquad n\in\mathbb Z
$$

At macroscopic scales, $e$ is so small that charge often appears continuous.

**JEE check:** if an isolated body is stated to carry a charge not equal to an integer multiple of $e$, the data are physically inconsistent at the elementary level.

### 2.5 Charge invariance

Electric charge does not depend on the observer's inertial frame. This differs from quantities such as length or time interval in relativity.

---

## 3. Conductors, insulators, and charging

### 3.1 Conductors and insulators **[B+J]**

- **Conductor:** contains mobile charge carriers; in metals these are mainly electrons.
- **Insulator/dielectric:** charges are bound and cannot move freely through the material, though polarisation can occur.
- **Semiconductor:** intermediate, controllable conductivity; treated in detail in Chapter 14.

### 3.2 Charging methods

- **Friction:** electrons transfer between unlike materials.
- **Conduction/contact:** charge transfers through direct contact.
- **Induction:** a conductor is charged without contact by redistribution, grounding, and removal in the correct sequence.

Earthing provides a path to a huge charge reservoir whose potential is taken approximately as zero.

### 3.3 Basic induction sequence **[B]**

To leave a neutral conductor with charge opposite to a nearby charged rod:

1. Bring rod near without touching.
2. Ground the conductor while rod remains.
3. Remove ground first.
4. Remove rod afterward.

Reversing steps 3 and 4 ruins the intended net charge.

---

## 4. Coulomb's law

### 4.1 Magnitude **[B+J]**

For two stationary point charges separated by distance $r$ in vacuum:

$$
F=\frac{1}{4\pi\varepsilon_0}\frac{|q_1q_2|}{r^2}
$$

where:

$$
\frac1{4\pi\varepsilon_0}=k_e\approx8.99\times10^9\ \mathrm{N\,m^2C^{-2}}
$$

and

$$
\varepsilon_0=8.854\times10^{-12}\ \mathrm{C^2N^{-1}m^{-2}}
$$

### 4.2 Vector form **[B+J]**

Force on $q_2$ due to $q_1$:

$$
\vec F_{21}=\frac1{4\pi\varepsilon_0}
\frac{q_1q_2}{r_{21}^2}\,\hat r_{21}
$$

where $\hat r_{21}$ points from $q_1$ to $q_2$.

Equivalent coordinate-safe form:

$$
\vec F_{21}=\frac1{4\pi\varepsilon_0}
\frac{q_1q_2(\vec r_2-\vec r_1)}{|\vec r_2-\vec r_1|^3}
$$

Newton's third law:

$$
\vec F_{12}=-\vec F_{21}
$$

### 4.3 Medium **[B+J]**

In a homogeneous isotropic dielectric with relative permittivity $K=\varepsilon_r$:

$$
\varepsilon=K\varepsilon_0
$$

$$
F_{\text{medium}}=\frac{F_{\text{vacuum}}}{K}
$$

This simple division assumes the entire relevant field region is filled uniformly by the dielectric.

---

## 5. Superposition principle

### 5.1 Discrete charges **[B+J]**

The net force on charge $q$ is the vector sum of forces from all other charges:

$$
\vec F=\sum_i\vec F_i
$$

Each pairwise force is calculated as if the other charges were absent.

### 5.2 Symmetry tricks **[J]**

- Resolve forces into components before adding.
- In symmetric arrangements, transverse components often cancel.
- At the centre of a regular polygon carrying identical charges at all vertices, net field is zero.
- If one charge is removed from a configuration whose complete field was zero, field due to the remaining charges is the negative of the removed charge's field.

### 5.3 Equilibrium of a charge

For equilibrium:

$$
\sum\vec F=0
$$

Zero net force does not automatically imply stable equilibrium. Stability requires the force after a small displacement to restore the body toward equilibrium.

---

## 6. Electric field

### 6.1 Definition **[B+J]**

Electric field at a point is force per unit positive test charge in the limit that the test charge does not disturb the source distribution:

$$
\vec E=\lim_{q_0\to0}\frac{\vec F}{q_0}
$$

Units:

$$
\mathrm{N\,C^{-1}}=\mathrm{V\,m^{-1}}
$$

Force on any charge placed there:

$$
\vec F=q\vec E
$$

For negative $q$, force is opposite to $\vec E$.

### 6.2 Point charge **[B+J]**

$$
\vec E=\frac1{4\pi\varepsilon_0}\frac{q}{r^2}\hat r
$$

- Outward for $q>0$.
- Inward for $q<0$.

### 6.3 System of point charges

$$
\vec E(\vec r)=\frac1{4\pi\varepsilon_0}
\sum_i q_i\frac{\vec r-\vec r_i}{|\vec r-\vec r_i|^3}
$$

### 6.4 Continuous distribution

$$
d\vec E=\frac1{4\pi\varepsilon_0}\frac{dq}{R^2}\hat R
$$

$$
\vec E=\int d\vec E
$$

Choose coordinates so symmetry cancels as many components as possible before integrating.

---

## 7. Electric field lines

### 7.1 Properties **[B+J]**

1. Tangent at a point gives field direction.
2. Line density represents relative field strength.
3. Lines originate on positive charge and terminate on negative charge, or extend to/from infinity.
4. They never intersect; intersection would imply two field directions at one point.
5. Electrostatic field lines do not form closed loops.
6. Lines meet an electrostatic conductor's surface normally.
7. No field lines exist inside the material of a conductor in electrostatic equilibrium because $\vec E=0$ there.

Field lines are a visual representation, not physical threads or particle trajectories in general.

### 7.2 Uniform field

A uniform field is represented by straight, parallel, equally spaced lines.

---

## 8. Electric dipole

### 8.1 Definition and dipole moment **[B+J]**

An electric dipole consists of charges $+q$ and $-q$ separated by displacement vector from negative to positive charge.

If separation is $2a$:

$$
\vec p=q(2\vec a)
$$

Magnitude:

$$
p=q(2a)
$$

Unit: $\mathrm{C\,m}$.

### 8.2 Field on axial line **[B+J]**

At distance $r>a$ from the centre on the positive axial side:

$$
E_{\mathrm{axial}}=\frac1{4\pi\varepsilon_0}
\frac{2pr}{(r^2-a^2)^2}
$$

For $r\gg a$:

$$
\vec E_{\mathrm{axial}}\approx
\frac1{4\pi\varepsilon_0}\frac{2\vec p}{r^3}
$$

On either axial side, determine direction from the actual charges; the far-field vector expression along the axis points in the direction of $\vec p$.

### 8.3 Field on equatorial line **[B+J]**

At perpendicular distance $r$ from the centre:

$$
\vec E_{\mathrm{equatorial}}=
-\frac1{4\pi\varepsilon_0}
\frac{\vec p}{(r^2+a^2)^{3/2}}
$$

For $r\gg a$:

$$
\vec E_{\mathrm{equatorial}}\approx
-\frac1{4\pi\varepsilon_0}\frac{\vec p}{r^3}
$$

Thus at the same large $r$:

$$
|E_{\mathrm{axial}}|=2|E_{\mathrm{equatorial}}|
$$

and directions are opposite relative to $\vec p$ as shown above.

### 8.4 General far-field expression **[J]**

$$
\vec E(\vec r)=\frac1{4\pi\varepsilon_0r^3}
\left[3(\vec p\cdot\hat r)\hat r-\vec p\right]
$$

valid for $r\gg$ dipole size.

### 8.5 Dipole in a uniform electric field **[B+J]**

Net force is zero, but forces form a couple.

$$
\vec\tau=\vec p\times\vec E
$$

$$
\tau=pE\sin\theta
$$

- $\theta=0$: stable equilibrium.
- $\theta=\pi$: unstable equilibrium.
- Torque is maximum at $90^\circ$.

In a non-uniform field, a dipole can also experience a net force; this is a JEE application, not a separate CBSE derivation requirement.

---

## 9. Electric flux

### 9.1 Area vector **[B+J]**

For a small surface element:

$$
d\vec S=\hat n\,dS
$$

For a closed surface, the area vector points outward.

### 9.2 Flux **[B+J]**

$$
d\Phi_E=\vec E\cdot d\vec S
$$

For a uniform field through a flat area:

$$
\Phi_E=EA\cos\theta
$$

where $\theta$ is between $\vec E$ and the area normal, not between the field and the plane.

For a general surface:

$$
\Phi_E=\int_S\vec E\cdot d\vec S
$$

Unit: $\mathrm{N\,m^2C^{-1}}$.

Flux may be positive, negative, or zero. Zero net flux does not necessarily mean zero field everywhere on the surface.

---

## 10. Continuous charge distributions

### 10.1 Charge densities **[B+J]**

| Distribution | Density | Element |
|---|---|---|
| Line | $\lambda=dq/dl$ | $dq=\lambda\,dl$ |
| Surface | $\sigma=dq/dS$ | $dq=\sigma\,dS$ |
| Volume | $\rho=dq/dV$ | $dq=\rho\,dV$ |

Units:

- $\lambda$: $\mathrm{C\,m^{-1}}$.
- $\sigma$: $\mathrm{C\,m^{-2}}$.
- $\rho$: $\mathrm{C\,m^{-3}}$.

For non-uniform density, keep the density inside the integral as a position-dependent function.

### 10.2 Integration template **[J]**

1. Choose an element $dq$.
2. Write its distance and direction to the observation point.
3. Express $d\vec E$.
4. Cancel components by symmetry.
5. Integrate surviving components over the complete source.

---

## 11. Gauss's law

### 11.1 Statement **[B+J]**

The net electric flux through any closed surface is $1/\varepsilon_0$ times the net charge enclosed:

$$
\oint_S\vec E\cdot d\vec S=
\frac{Q_{\mathrm{enclosed}}}{\varepsilon_0}
$$

### 11.2 What it does and does not say

- It is valid for every closed surface, not only symmetric ones.
- Only enclosed charge appears on the right side.
- Charges outside can contribute to $\vec E$ locally, but their net flux through the closed surface is zero.
- A charge exactly on an ideal Gaussian surface creates ambiguity; choose a slightly shifted surface or treat the limiting geometry carefully.
- Gauss's law gives $E$ easily only when symmetry lets $E$ be taken constant or zero over selected parts of the surface.

### 11.3 Choosing a Gaussian surface **[B+J]**

Match source symmetry:

- Spherical symmetry $\rightarrow$ concentric sphere.
- Cylindrical symmetry $\rightarrow$ coaxial cylinder.
- Planar symmetry $\rightarrow$ pillbox.

The Gaussian surface is imaginary; it need not coincide with a physical object.

---

## 12. Standard Gaussian-law results

### 12.1 Infinitely long uniformly charged straight wire **[B+J]**

For linear density $\lambda$, at perpendicular distance $r$:

$$
E(2\pi rl)=\frac{\lambda l}{\varepsilon_0}
$$

$$
\boxed{E=\frac{\lambda}{2\pi\varepsilon_0r}}
$$

Direction is radially outward for $\lambda>0$ and inward for $\lambda<0$.

### 12.2 Uniformly charged infinite plane sheet **[B+J]**

For surface density $\sigma$:

$$
2EA=\frac{\sigma A}{\varepsilon_0}
$$

$$
\boxed{E=\frac{\sigma}{2\varepsilon_0}}
$$

The magnitude is independent of distance.

Two oppositely charged infinite sheets $+\sigma$ and $-\sigma$:

$$
E_{\text{between}}=\frac{\sigma}{\varepsilon_0},
\qquad
E_{\text{outside}}=0
$$

by superposition.

### 12.3 Uniformly charged thin spherical shell **[B+J]**

For radius $R$ and total charge $Q$:

Outside, $r>R$:

$$
\boxed{E=\frac1{4\pi\varepsilon_0}\frac{Q}{r^2}}
$$

The shell acts as if all charge were concentrated at its centre for external points.

Inside, $r<R$:

$$
\boxed{E=0}
$$

At the surface:

$$
E_{\mathrm{just\ outside}}=
\frac1{4\pi\varepsilon_0}\frac{Q}{R^2}
=\frac{\sigma}{\varepsilon_0}
$$

while just inside an ideal conducting shell $E=0$. The normal component jumps by $\sigma/\varepsilon_0$.

---

## 13. Formula sheet

| Concept | Formula |
|---|---|
| Quantisation | $q=ne$ |
| Coulomb force | $F=k_e|q_1q_2|/r^2$ |
| Field of point charge | $\vec E=k_eq\hat r/r^2$ |
| Force in field | $\vec F=q\vec E$ |
| Dipole moment | $\vec p=q\,\vec d$ from $-q$ to $+q$ |
| Far axial dipole field | $E=2k_ep/r^3$ |
| Far equatorial field | $\vec E=-k_e\vec p/r^3$ |
| Dipole torque | $\vec\tau=\vec p\times\vec E$ |
| Flux | $\Phi=\int\vec E\cdot d\vec S$ |
| Gauss law | $\oint\vec E\cdot d\vec S=Q_{\rm enc}/\varepsilon_0$ |
| Infinite line | $E=\lambda/(2\pi\varepsilon_0r)$ |
| Infinite sheet | $E=\sigma/(2\varepsilon_0)$ |
| Spherical shell outside | $E=k_eQ/r^2$ |
| Spherical shell inside | $E=0$ |

---

## 14. Problem-solving playbook

### 14.1 Point-charge configuration

1. Draw coordinates and force/field arrows.
2. Calculate each contribution with its own distance.
3. Resolve into $x$ and $y$ components.
4. Add components, then find magnitude and direction.
5. Use symmetry before arithmetic.

### 14.2 Zero-field point on a line **[J]**

- For like charges, cancellation point lies between them and closer to the smaller magnitude.
- For unlike charges, fields between them point in the same direction, so cancellation must lie outside, on the side of the smaller magnitude.
- These location rules assume only two charges; always verify directions.

### 14.3 Dipole questions

1. Check whether the point is axial or equatorial.
2. Check whether $r\gg a$ before using short-dipole formulas.
3. Keep the direction of $\vec p$ from negative to positive.
4. For torque, use the angle between $\vec p$ and $\vec E$.

### 14.4 Gauss-law questions

Ask three questions:

1. What symmetry does the **source** have?
2. On which surface is $E$ constant in magnitude?
3. Where is $\vec E$ parallel or perpendicular to $d\vec S$?

If these cannot be answered cleanly, Gauss's law remains true but may not directly calculate $E$.

### 14.5 Dimensional checks

- Point-charge field must scale as $1/r^2$.
- Dipole far field must scale as $1/r^3$.
- Infinite-line field scales as $1/r$.
- Infinite-sheet field is distance-independent.

---

## 15. Board derivations

Prepare clean, labelled derivations for:

1. Electric field on axial line of a dipole; give exact and $r\gg a$ form.
2. Electric field on equatorial line; show component cancellation and direction opposite $\vec p$.
3. Torque on a dipole in uniform field.
4. Gauss-law field of an infinite line charge.
5. Gauss-law field of an infinite plane sheet.
6. Field inside and outside a uniformly charged thin spherical shell.

For every Gaussian derivation: state symmetry, draw surface, identify zero-flux parts, calculate enclosed charge, and then apply Gauss's law.

---

## 16. Common traps

1. Adding charges as vectors.
2. Using a negative magnitude for force instead of handling direction separately.
3. Choosing an inconsistent unit vector in Coulomb's vector law.
4. Including the test charge in the source field.
5. Saying field points opposite the force without checking the sign of the placed charge.
6. Drawing intersecting or closed electrostatic field lines.
7. Taking dipole moment from positive to negative; it points negative to positive.
8. Using far-dipole formulas when $r$ is not much greater than separation.
9. Forgetting that equatorial dipole field is opposite $\vec p$.
10. Taking flux angle with the surface rather than its normal.
11. Assuming zero net flux means zero field.
12. Putting external charge into $Q_{\rm enclosed}$.
13. Using Gauss's law to solve $E$ without sufficient symmetry.
14. Writing $\sigma/\varepsilon_0$ for a non-conducting isolated infinite sheet; its field on either side is $\sigma/(2\varepsilon_0)$.

---

## 17. Last-minute checklist

- [ ] I know charge additivity, conservation, and quantisation.
- [ ] I can use scalar and vector forms of Coulomb's law.
- [ ] I can add fields/forces using components and symmetry.
- [ ] I can explain all electric-field-line rules.
- [ ] I know exact and far axial/equatorial dipole results and directions.
- [ ] I can calculate torque and identify stable/unstable orientation.
- [ ] I can calculate flux using the area normal.
- [ ] I know $dq=\lambda dl$, $\sigma dS$, and $\rho dV$.
- [ ] I know when Gauss's law is computationally useful.
- [ ] I can derive line, sheet, and spherical-shell field results.

## Official syllabus references

- [CBSE Physics syllabus 2026-27](https://cbseacademic.nic.in/web_material/CurriculumMain27/SecPart2/Physics_SecP2_2026-27.pdf)
- [NTA JEE Main 2026 syllabus page](https://jeemain.nta.nic.in/document/syllabus-2026/)
