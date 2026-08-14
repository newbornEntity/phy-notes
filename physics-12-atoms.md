# Atoms - Class 12 Physics

> NCERT-aligned board notes with a JEE Main problem-solving layer  
> Source chapter: `leph204.pdf` (Chapter 12)  
> Syllabus basis checked: CBSE 2026-27 and JEE Main 2026, on 13 July 2026

## How to use these notes

| Tag | Meaning |
|---|---|
| **[B+J]** | Required for CBSE boards and explicitly relevant to JEE Main |
| **[B]** | Board-answer or derivation emphasis |
| **[J]** | JEE Main extension or fast result |
| **[Scope note]** | Current reduced-syllabus boundary |

**Important:** The official JEE Main 2027 syllabus was not available on the preparation date. JEE tags provisionally use JEE Main 2026, the latest official NTA syllabus.

## Navigation

- [1. Exam scope](#1-exam-scope)
- [2. Rutherford alpha-scattering experiment](#2-rutherford-alpha-scattering-experiment)
- [3. Rutherford atomic model and limitations](#3-rutherford-atomic-model-and-limitations)
- [4. Atomic spectra](#4-atomic-spectra)
- [5. Bohr model](#5-bohr-model)
- [6. Hydrogen-like orbit formulas](#6-hydrogen-like-orbit-formulas)
- [7. Transitions and hydrogen spectrum](#7-transitions-and-hydrogen-spectrum)
- [8. de Broglie explanation of Bohr quantisation](#8-de-broglie-explanation-of-bohr-quantisation)
- [9. Formula sheet](#9-formula-sheet)
- [10. Numerical playbook](#10-numerical-playbook)
- [11. Board answer map](#11-board-answer-map)
- [12. Common traps](#12-common-traps)
- [13. Last-minute checklist](#13-last-minute-checklist)

---

## 1. Exam scope

### CBSE 2026-27

Explicit scope:

- alpha-particle scattering experiment;
- Rutherford model;
- Bohr model of hydrogen;
- expressions for radius, velocity, and electron energy in the $n$th orbit;
- hydrogen line spectra, **qualitative treatment only**.

CBSE groups Dual Nature, Atoms, and Nuclei into a shared **12-mark block**, with no fixed chapter-wise split.

### JEE Main 2026

Explicit scope: alpha scattering, Rutherford model, Bohr model, energy levels, and hydrogen spectrum. JEE commonly adds closest approach, excitation/ionisation, transition counting, and hydrogen-like ion scaling.

### Scope notes

- Detailed quantum-mechanical orbitals are not part of this Physics chapter.
- Hydrogen spectrum is qualitative for CBSE, but the Bohr transition/Rydberg formulas remain essential for numericals and JEE.

---

## 2. Rutherford alpha-scattering experiment

### 2.1 Setup **[B+J]**

- A narrow beam of energetic alpha particles was directed at a very thin gold foil.
- A surrounding fluorescent screen detected scattered particles through tiny flashes.
- Alpha particles are positively charged and much heavier than electrons, making them useful probes of positive charge distribution.

### 2.2 Observations **[B+J]**

1. Most alpha particles passed almost undeflected.
2. A small fraction suffered moderate deflections.
3. A very tiny fraction scattered through large angles or nearly backward.

### 2.3 Conclusions **[B+J]**

1. Most of the atom is empty space.
2. Nearly all positive charge and mass are concentrated in a tiny central nucleus.
3. The nucleus is much smaller than the atom.
4. Large-angle deflection results from close approach to the concentrated positive nuclear charge.

### 2.4 Distance of closest approach **[J]**

For a head-on alpha particle approaching a nucleus of charge $+Ze$, initial kinetic energy is converted into electrostatic potential energy at the turning point:

$$
K=\frac1{4\pi\varepsilon_0}\frac{(2e)(Ze)}{r_0}
$$

$$
\boxed{r_0=\frac1{4\pi\varepsilon_0}\frac{2Ze^2}{K}}
$$

For a projectile of charge $+ze$:

$$
r_0=\frac1{4\pi\varepsilon_0}\frac{zZe^2}{K}
$$

This classical turning distance is not nuclear radius; it is an upper-bound style probe distance for the stated energy.

### 2.5 Impact parameter and scattering angle **[J]**

Impact parameter $b$ is the perpendicular distance between the initial straight-line path and the nucleus centre if no deflection occurred.

For Rutherford scattering with projectile charge $ze$ and kinetic energy $K$:

$$
b=\frac1{4\pi\varepsilon_0}\frac{zZe^2}{2K}
\cot\frac\theta2
$$

- Small $b$ $\Rightarrow$ close approach $\Rightarrow$ large scattering angle $\theta$.
- Head-on approach $b=0$ corresponds to $\theta=180^\circ$.

The detailed differential cross-section formula is not named in the current CBSE/JEE Main unit and is not a priority here.

---

## 3. Rutherford atomic model and limitations

### 3.1 Model **[B+J]**

- Tiny positive nucleus at the centre.
- Electrons move around it under electrostatic attraction.
- Atomic dimensions are much larger than nuclear dimensions.

### 3.2 Classical orbital frequency **[context]**

For a circular electron orbit, electrostatic attraction provides centripetal force:

$$
\frac{mv^2}{r}=\frac1{4\pi\varepsilon_0}\frac{Ze^2}{r^2}
$$

### 3.3 Failures **[B+J]**

1. An orbiting electron is an accelerating charge.
2. Classical electrodynamics predicts it should radiate energy continuously.
3. It should lose energy and spiral into the nucleus, making atoms unstable.
4. Continuous energy loss should produce a continuous spectrum, not observed discrete line spectra.

Rutherford's model explained scattering and nuclear concentration but not stability or spectra.

---

## 4. Atomic spectra

### 4.1 Emission and absorption spectra **[B+J]**

- **Emission spectrum:** bright lines at specific wavelengths emitted by excited atoms.
- **Absorption spectrum:** dark lines missing from a continuous background because atoms absorb selected wavelengths.

Each element has a characteristic line spectrum, showing that atomic energies are discrete.

### 4.2 Hydrogen spectrum

Hydrogen lines follow the empirical Rydberg relation:

$$
\frac1\lambda=R_H\left(\frac1{n_f^2}-\frac1{n_i^2}\right),
\qquad n_i>n_f
$$

For hydrogen-like ions of nuclear charge $Z$:

$$
\frac1\lambda=RZ^2\left(\frac1{n_f^2}-\frac1{n_i^2}\right)
$$

Main series:

| Final level $n_f$ | Series | Region |
|---:|---|---|
| 1 | Lyman | Ultraviolet |
| 2 | Balmer | Mainly visible/near-UV |
| 3 | Paschen | Infrared |
| 4 | Brackett | Infrared |
| 5 | Pfund | Infrared |

**CBSE note:** line spectra are prescribed qualitatively. Know what each series represents and use final formulas; a long spectral derivation is not the board priority.

---

## 5. Bohr model

### 5.1 Postulates **[B+J]**

1. Electrons can move only in certain permitted stable circular orbits called stationary states, without continuous radiation.
2. Orbital angular momentum is quantised:

$$
mvr=n\hbar=\frac{nh}{2\pi},
\qquad n=1,2,3,\ldots
$$

3. Radiation is emitted or absorbed only when an electron changes between stationary states:

$$
h\nu=|E_i-E_f|
$$

The integer $n$ is the principal quantum number in this model.

### 5.2 Ground and excited states

- Ground state: $n=1$, minimum energy.
- Excited states: $n=2,3,\ldots$.
- Ionised state: electron at infinity, conventionally $E=0$.

### 5.3 Scope and limitations

Bohr's model works well for one-electron systems such as $\ce{H}$, $\ce{He+}$, $\ce{Li^{2+}}$, but not accurately for multi-electron atoms, fine structure, line intensities, Zeeman/Stark details, or full quantum behaviour.

---

## 6. Hydrogen-like orbit formulas

For a nucleus of charge $+Ze$ and one electron.

### 6.1 Radius **[B+J]**

Combining Coulomb force with $mvr=n\hbar$:

$$
\boxed{r_n=\frac{4\pi\varepsilon_0\hbar^2}{me^2}\frac{n^2}{Z}}
$$

$$
\boxed{r_n=a_0\frac{n^2}{Z}}
$$

where:

$$
a_0=5.29\times10^{-11}\ \mathrm m=0.529\ \text{\AA}
$$

Scaling:

$$
r_n\propto\frac{n^2}{Z}
$$

### 6.2 Orbital speed **[B+J]**

$$
\boxed{v_n=\frac{Ze^2}{4\pi\varepsilon_0n\hbar}}
$$

$$
\boxed{v_n\approx2.19\times10^6\frac{Z}{n}\ \mathrm{m\,s^{-1}}}
$$

Scaling:

$$
v_n\propto\frac{Z}{n}
$$

### 6.3 Kinetic, potential, and total energy **[B+J]**

From the circular-orbit force equation:

$$
K=\frac12mv^2=\frac1{8\pi\varepsilon_0}\frac{Ze^2}{r}
$$

$$
U=-\frac1{4\pi\varepsilon_0}\frac{Ze^2}{r}=-2K
$$

$$
E=K+U=-K=\frac U2
$$

Quantised total energy:

$$
\boxed{E_n=-13.6\frac{Z^2}{n^2}\ \mathrm{eV}}
$$

Therefore:

$$
K_n=+13.6\frac{Z^2}{n^2}\ \mathrm{eV}
$$

$$
U_n=-27.2\frac{Z^2}{n^2}\ \mathrm{eV}
$$

Negative total energy means the electron is bound relative to $E=0$ at infinite separation.

### 6.4 Orbital period and frequency **[J]**

$$
T_n=\frac{2\pi r_n}{v_n}
\propto\frac{n^3}{Z^2}
$$

$$
f_n\propto\frac{Z^2}{n^3}
$$

Do not equate this classical orbital frequency directly to every emitted photon frequency; radiation arises from energy differences between levels.

---

## 7. Transitions and hydrogen spectrum

### 7.1 Photon energy **[B+J]**

For emission from $n_i$ to $n_f<n_i$:

$$
h\nu=E_{n_i}-E_{n_f}
$$

Magnitude:

$$
\boxed{h\nu=13.6Z^2
\left(\frac1{n_f^2}-\frac1{n_i^2}\right)\ \mathrm{eV}}
$$

$$
\lambda=\frac{hc}{\Delta E}
$$

Absorption uses the same positive energy difference but moves the electron upward.

### 7.2 Excitation energy **[B+J]**

Energy to move from $n_1$ to a higher finite $n_2$:

$$
E_{\mathrm{exc}}=E_{n_2}-E_{n_1}>0
$$

### 7.3 Ionisation energy **[B+J]**

From level $n$ to infinity:

$$
E_{\mathrm{ion},n}=0-E_n
=13.6\frac{Z^2}{n^2}\ \mathrm{eV}
$$

Ionisation potential has the same numerical value in volts for one electron.

### 7.4 Number of possible spectral lines **[J]**

If an atom is excited to level $n$ and all downward transitions among levels $1$ through $n$ occur in an ensemble:

$$
N_{\max}=\frac{n(n-1)}2
$$

Number of lines ending at a particular lower level $n_f$:

$$
N=n-n_f
$$

One individual atom follows one cascade path at a time; the complete set refers to many atoms or repeated events.

### 7.5 Longest and shortest wavelengths **[J]**

Because $\lambda=hc/\Delta E$:

- Largest energy gap $\Rightarrow$ shortest wavelength.
- Smallest energy gap $\Rightarrow$ longest wavelength.

Within a series ending at fixed $n_f$:

- series limit $n_i\to\infty$ gives shortest wavelength;
- first line $n_i=n_f+1$ gives longest wavelength.

---

## 8. de Broglie explanation of Bohr quantisation

### 8.1 Standing matter wave **[B+J]**

For a stable circular orbit, an integer number of de Broglie wavelengths fits around the circumference:

$$
2\pi r=n\lambda
$$

Using $\lambda=h/(mv)$:

$$
2\pi r=n\frac{h}{mv}
$$

$$
\boxed{mvr=\frac{nh}{2\pi}=n\hbar}
$$

Thus Bohr's angular-momentum condition corresponds to a standing matter-wave condition.

---

## 9. Formula sheet

| Concept | Formula |
|---|---|
| Closest approach, alpha | $r_0=k_e(2Ze^2)/K$ |
| Bohr quantisation | $mvr=n\hbar$ |
| Radius | $r_n=a_0n^2/Z$ |
| Speed | $v_n=2.19\times10^6(Z/n)\ \mathrm{m\,s^{-1}}$ |
| Total energy | $E_n=-13.6Z^2/n^2\ \mathrm{eV}$ |
| Kinetic energy | $K_n=+13.6Z^2/n^2\ \mathrm{eV}$ |
| Potential energy | $U_n=-27.2Z^2/n^2\ \mathrm{eV}$ |
| Energy relations | $U=-2K$, $E=-K=U/2$ |
| Transition | $h\nu=|E_i-E_f|$ |
| Spectrum | $1/\lambda=RZ^2(1/n_f^2-1/n_i^2)$ |
| Ionisation from $n$ | $13.6Z^2/n^2\ \mathrm{eV}$ |
| Maximum lines | $n(n-1)/2$ |
| Matter-wave orbit | $2\pi r=n\lambda$ |

Constants:

- $a_0=0.529\ \text{\AA}$.
- $R\approx1.097\times10^7\ \mathrm{m^{-1}}$.
- $hc\approx1240\ \mathrm{eV\,nm}$.

---

## 10. Numerical playbook

### 10.1 Hydrogen-like ions

First identify $Z$ and confirm there is only one electron. Then use scaling:

- $r\propto n^2/Z$;
- $v\propto Z/n$;
- $|E|\propto Z^2/n^2$.

Ratios are often faster and safer than inserting constants.

### 10.2 Transition question

1. Write both level energies with signs.
2. Take positive photon energy $|E_i-E_f|$.
3. Decide emission or absorption from direction.
4. Convert using $\lambda=hc/\Delta E$.
5. Check spectral region/series from the final level.

### 10.3 Closest approach

Use energy conservation for head-on motion. Convert MeV to eV/J consistently. A larger projectile energy gives a smaller closest approach; a larger nuclear $Z$ gives a larger turning distance for the same projectile energy.

### 10.4 Excitation versus ionisation

- Excitation ends at a finite higher $n$.
- Ionisation ends at $n=\infty$, $E=0$.
- Ionisation energy from an already excited state is smaller than from ground state.

---

## 11. Board answer map

Prepare:

1. Rutherford setup, three observations, and corresponding conclusions.
2. Rutherford model and its two major failures: stability and spectra.
3. Bohr postulates.
4. Derivations of $r_n$, $v_n$, and $E_n$ for hydrogen-like atoms.
5. Energy-level diagram and qualitative explanation of hydrogen line series.
6. de Broglie standing-wave explanation of angular-momentum quantisation.

For CBSE's qualitative spectrum treatment, prioritise a correct level diagram, transition direction, series name/region, and energy relation over a long Rydberg derivation.

---

## 12. Common traps

1. Saying Rutherford found that most of the atom is occupied by the nucleus.
2. Treating distance of closest approach as the exact nuclear radius.
3. Using alpha charge $+e$ instead of $+2e$.
4. Forgetting that Bohr formulas with $Z$ apply only to one-electron species.
5. Writing $r_n\propto n/Z$ instead of $n^2/Z$.
6. Making bound-state energy positive.
7. Confusing total, kinetic, and potential energies: $U=-2K$, $E=-K$.
8. Using $E_i-E_f$ with a negative photon energy; use the positive magnitude and direction separately.
9. Calling Lyman visible or Balmer entirely infrared.
10. Reversing series-limit wavelength: the limit has the largest energy gap and shortest wavelength in that series.
11. Counting $n(n-1)/2$ lines from one single atom in one uninterrupted cascade rather than the possible ensemble spectrum.
12. Equating classical orbital frequency with emitted photon frequency.

---

## 13. Last-minute checklist

- [ ] I know Rutherford's setup, observations, conclusions, and limitations.
- [ ] I can calculate alpha-particle closest approach.
- [ ] I can state all Bohr postulates.
- [ ] I can derive and scale radius, speed, and energy.
- [ ] I know $K$, $U$, and $E$ relations without sign confusion.
- [ ] I can calculate excitation, ionisation, wavelength, and frequency.
- [ ] I know Lyman, Balmer, Paschen, Brackett, and Pfund final levels.
- [ ] I can find the maximum possible number of lines.
- [ ] I can explain Bohr quantisation using $2\pi r=n\lambda$.
- [ ] I remember CBSE requires qualitative treatment of hydrogen line spectra.

## Official syllabus references

- [CBSE Physics syllabus 2026-27](https://cbseacademic.nic.in/web_material/CurriculumMain27/SecPart2/Physics_SecP2_2026-27.pdf)
- [NTA JEE Main 2026 syllabus page](https://jeemain.nta.nic.in/document/syllabus-2026/)
