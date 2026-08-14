# Dual Nature of Radiation and Matter - Class 12 Physics

> NCERT-aligned board notes with a JEE Main problem-solving layer  
> Source chapter: `leph203.pdf` (Chapter 11)  
> Syllabus basis checked: CBSE 2026-27 and JEE Main 2026, on 13 July 2026

## How to use these notes

| Tag | Meaning |
|---|---|
| **[B+J]** | Required for CBSE boards and explicitly relevant to JEE Main |
| **[B]** | Board-explanation or derivation emphasis |
| **[J]** | JEE Main extension or fast numerical result |
| **[Scope note]** | Current reduced-syllabus boundary |

**Important:** The official JEE Main 2027 syllabus was not available on the preparation date. JEE tags use the latest official NTA syllabus, JEE Main 2026, provisionally.

## Navigation

- [1. Exam scope](#1-exam-scope)
- [2. Why dual nature is needed](#2-why-dual-nature-is-needed)
- [3. Electron emission](#3-electron-emission)
- [4. Photoelectric effect and observations](#4-photoelectric-effect-and-observations)
- [5. Failure of classical wave theory](#5-failure-of-classical-wave-theory)
- [6. Einstein's photoelectric equation](#6-einsteins-photoelectric-equation)
- [7. Photon model](#7-photon-model)
- [8. Matter waves and de Broglie relation](#8-matter-waves-and-de-broglie-relation)
- [9. Formula and graph sheet](#9-formula-and-graph-sheet)
- [10. Numerical playbook](#10-numerical-playbook)
- [11. Board answer map](#11-board-answer-map)
- [12. Common traps](#12-common-traps)
- [13. Last-minute checklist](#13-last-minute-checklist)

---

## 1. Exam scope

### CBSE 2026-27

Explicit scope:

- dual nature of radiation;
- photoelectric effect;
- Hertz and Lenard observations;
- Einstein's photoelectric equation and particle nature of light;
- experimental study of photoelectric effect;
- matter waves and de Broglie relation.

CBSE groups Dual Nature, Atoms, and Nuclei into a **shared 12-mark block**; there is no fixed chapter-wise mark guarantee.

### JEE Main 2026

The official scope matches the same core. JEE commonly tests graphs, threshold wavelength/frequency, stopping potential, photon counting, and de Broglie wavelength after acceleration.

### Reduced-syllabus boundary

- The uploaded chapter ends with wave nature of matter and does not include a Davisson-Germer section.
- Davisson-Germer experiment is not named in the official CBSE 2026-27 or JEE Main 2026 unit wording. Know it only if your teacher separately requires historical evidence; do not prioritise it here.

---

## 2. Why dual nature is needed

Light shows:

- **Wave behaviour:** interference, diffraction, polarisation.
- **Particle behaviour:** emission and absorption in discrete packets in the photoelectric effect.

Matter normally appears particulate but moving particles possess an associated wavelength. "Dual nature" does not mean a classical wave and classical particle are literally present simultaneously; the quantum object produces different observable behaviour in different experimental arrangements.

---

## 3. Electron emission

### 3.1 Work function **[B+J]**

Electrons in a metal are bound by a surface energy barrier. The minimum energy needed to eject an electron is the work function:

$$
\phi=W_0
$$

Unit commonly used: electron volt.

$$
1\ \mathrm{eV}=1.602\times10^{-19}\ \mathrm J
$$

Work function depends on material and surface condition.

### 3.2 Methods of electron emission **[B context]**

- **Thermionic emission:** heating supplies energy.
- **Field emission:** very strong electric field extracts electrons.
- **Photoelectric emission:** incident radiation supplies energy.

These are useful context; current exam emphasis is photoelectric emission.

---

## 4. Photoelectric effect and observations

### 4.1 Definition **[B+J]**

Emission of electrons from a suitable material when electromagnetic radiation of adequate frequency falls on it is the photoelectric effect. Emitted electrons are photoelectrons.

### 4.2 Experimental arrangement **[B]**

A photosensitive emitter and a collector are enclosed in an evacuated tube. Variable potential controls collection/retardation, while a microammeter measures photocurrent. Radiation frequency and intensity can be varied.

### 4.3 Photocurrent versus applied potential **[B+J]**

- Positive collector potential attracts more emitted electrons.
- At sufficiently positive voltage, nearly all emitted electrons are collected and current reaches **saturation current**.
- A negative collector retards electrons.
- At a particular reverse voltage magnitude $V_0$, even the fastest photoelectrons fail to reach the collector and current becomes zero. This is **stopping potential**.

$$
K_{\max}=eV_0
$$

### 4.4 Effect of intensity **[B+J]**

At fixed frequency above threshold:

- greater intensity $\Rightarrow$ more incident photons per second;
- more photoelectrons per second $\Rightarrow$ larger photocurrent and saturation current;
- stopping potential and maximum kinetic energy remain unchanged.

### 4.5 Effect of frequency **[B+J]**

At fixed intensity and for $\nu>\nu_0$:

- higher frequency $\Rightarrow$ larger maximum kinetic energy;
- stopping-potential magnitude rises.

The photocurrent need not rise merely because frequency rises; current primarily depends on photon arrival rate and collection conditions.

### 4.6 Threshold frequency **[B+J]**

For each material, emission occurs only when:

$$
\nu\ge\nu_0
$$

Equivalently:

$$
\lambda\le\lambda_0
$$

No increase in intensity can cause photoemission below threshold frequency.

### 4.7 Negligible time lag **[B+J]**

Photoemission begins essentially immediately when suitable radiation arrives, even at low intensity. Energy transfer occurs photon by photon, not by gradual accumulation from a classical wave.

---

## 5. Failure of classical wave theory

Classical wave theory would suggest:

1. Electron energy should increase with light intensity.
2. Sufficiently intense radiation of any frequency should eventually eject electrons.
3. At low intensity, a measurable delay might occur while an electron accumulates energy.

Experiments instead show:

- $K_{\max}$ depends on frequency, not intensity;
- a definite threshold frequency exists;
- emission has no observable accumulation delay.

This motivates quantised energy transfer.

---

## 6. Einstein's photoelectric equation

### 6.1 Photon energy **[B+J]**

Planck's quantum relation:

$$
E_\gamma=h\nu=\frac{hc}{\lambda}
$$

One photon transfers its energy to one electron in the elementary Einstein picture.

### 6.2 Energy conservation **[B+J]**

Part of photon energy overcomes the work function; the rest becomes maximum electron kinetic energy:

$$
\boxed{h\nu=\phi+K_{\max}}
$$

$$
\boxed{K_{\max}=h\nu-\phi}
$$

Using stopping potential:

$$
\boxed{eV_0=h\nu-\phi}
$$

At threshold, $K_{\max}=0$:

$$
\boxed{\phi=h\nu_0=\frac{hc}{\lambda_0}}
$$

Therefore:

$$
eV_0=h(\nu-\nu_0)
$$

and

$$
K_{\max}=hc\left(\frac1\lambda-\frac1{\lambda_0}\right)
$$

### 6.3 Fast eV-nm form **[J]**

Using $hc\approx1240\ \mathrm{eV\,nm}$:

$$
E_\gamma(\mathrm{eV})=\frac{1240}{\lambda(\mathrm{nm})}
$$

$$
K_{\max}(\mathrm{eV})=E_\gamma(\mathrm{eV})-\phi(\mathrm{eV})
$$

For an electron, the numerical value of $K_{\max}$ in eV equals the stopping-potential magnitude in volts.

### 6.4 Einstein equation explains all main observations

- Threshold: photon must have $h\nu\ge\phi$.
- Frequency dependence: excess photon energy becomes $K_{\max}$.
- Intensity dependence: intensity controls number of photons and hence number of emitted electrons, not energy per photon at fixed $\nu$.
- Immediate emission: one photon transfers energy in a single interaction.

---

## 7. Photon model

### 7.1 Photon properties **[B+J]**

$$
E=h\nu=\frac{hc}{\lambda}
$$

$$
p_\gamma=\frac{E}{c}=\frac{h}{\lambda}
$$

- Rest mass: zero.
- Electric charge: zero.
- Travels at $c$ in vacuum.
- Energy and momentum depend on frequency/wavelength.
- In interactions, total energy and momentum are conserved.

### 7.2 Photon flux and optical power **[J]**

For monochromatic light power $P$:

$$
N_\gamma=\frac{P}{h\nu}=\frac{P\lambda}{hc}
$$

photons per second.

If quantum efficiency $\eta$ means emitted electrons per incident photon:

$$
I_{\text{photo}}=\eta eN_\gamma
$$

under full collection/saturation conditions.

---

## 8. Matter waves and de Broglie relation

### 8.1 de Broglie hypothesis **[B+J]**

Every moving material particle has an associated wavelength:

$$
\boxed{\lambda=\frac{h}{p}}
$$

For a non-relativistic particle:

$$
\lambda=\frac{h}{mv}
$$

Matter-wave wavelength depends on momentum, not merely velocity.

### 8.2 Particle accelerated through potential difference **[B+J]**

For charge magnitude $q$ starting from rest:

$$
qV=\frac{p^2}{2m}
$$

$$
\boxed{\lambda=\frac{h}{\sqrt{2mqV}}}
$$

For an electron:

$$
\boxed{\lambda(\text{\AA})=\frac{12.27}{\sqrt{V(\mathrm V)}}}
$$

or

$$
\lambda(\mathrm{nm})=\frac{1.227}{\sqrt{V(\mathrm V)}}
$$

This shortcut is non-relativistic and is excellent for ordinary Class 12/JEE Main voltages.

### 8.3 Using kinetic energy **[J]**

$$
\lambda=\frac{h}{\sqrt{2mK}}
$$

At equal kinetic energy, the lighter particle has the larger wavelength. At equal speed, the lighter particle also has the larger wavelength. At equal momentum, all particles have the same de Broglie wavelength.

### 8.4 Why matter waves are not obvious for macroscopic objects

Macroscopic momentum is enormous compared with $h$, so $\lambda=h/p$ is far too small to observe ordinary diffraction.

### 8.5 Matter-wave interpretation

Matter waves are not ordinary mechanical waves requiring a material medium. Their measurable significance appears through quantum probability and interference/diffraction behaviour.

---

## 9. Formula and graph sheet

### Formula table

| Concept | Formula |
|---|---|
| Photon energy | $E=h\nu=hc/\lambda$ |
| Photon momentum | $p=h/\lambda=E/c$ |
| Work function | $\phi=h\nu_0=hc/\lambda_0$ |
| Photoelectric equation | $K_{\max}=h\nu-\phi$ |
| Stopping potential | $eV_0=K_{\max}$ |
| Wavelength form | $K_{\max}=hc(1/\lambda-1/\lambda_0)$ |
| Photon rate | $N=P/(h\nu)=P\lambda/(hc)$ |
| de Broglie | $\lambda=h/p$ |
| Non-relativistic | $\lambda=h/\sqrt{2mK}$ |
| Accelerating voltage | $\lambda=h/\sqrt{2mqV}$ |
| Electron shortcut | $\lambda(\text{\AA})=12.27/\sqrt V$ |

Constants:

- $h=6.626\times10^{-34}\ \mathrm{J\,s}$.
- $c=3.00\times10^8\ \mathrm{m\,s^{-1}}$.
- $e=1.602\times10^{-19}\ \mathrm C$.
- $m_e=9.11\times10^{-31}\ \mathrm{kg}$.
- $hc\approx1240\ \mathrm{eV\,nm}$.

### Graphs to master

1. Photocurrent vs anode potential for two intensities: higher intensity gives higher saturation current; same stopping potential.
2. Photocurrent vs potential for two frequencies: higher frequency gives larger stopping-potential magnitude; saturation-current comparison depends on photon flux/intensity conditions.
3. $K_{\max}$ vs $\nu$: straight line, slope $h$, frequency-axis intercept $\nu_0$, energy-axis intercept $-\phi$ on extrapolation.
4. $V_0$ vs $\nu$: slope $h/e$, frequency-axis intercept $\nu_0$.

---

## 10. Numerical playbook

### 10.1 Photoelectric equation

1. Convert wavelength/frequency to photon energy.
2. Compare with $\phi$ before calculating emission.
3. If $E_\gamma<\phi$, there is no photoemission in the ideal model.
4. Otherwise calculate $K_{\max}=E_\gamma-\phi$.
5. Convert $K_{\max}$ in eV directly to $V_0$ in volts for electrons.

### 10.2 Changing intensity or frequency

- Intensity change at fixed frequency $\Rightarrow$ change in photon rate/current, not $K_{\max}$.
- Frequency change $\Rightarrow$ change in energy per photon and $V_0$.
- If optical **power** is fixed rather than intensity/photon rate, changing frequency also changes the number of photons per second.

### 10.3 de Broglie comparison

Write $\lambda=h/p$ first. Then translate the stated equal condition:

- equal velocity $\Rightarrow p=mv$;
- equal kinetic energy $\Rightarrow p=\sqrt{2mK}$;
- same accelerating voltage and equal charge $\Rightarrow p=\sqrt{2mqV}$.

Do not compare wavelengths from mass alone without identifying what is held constant.

---

## 11. Board answer map

Prepare clear explanations for:

1. Experimental photoelectric arrangement and meanings of saturation current/stopping potential.
2. Effect of intensity and frequency, with labelled $I-V$ graphs.
3. Failure of classical wave theory.
4. Einstein equation and how it explains threshold, instantaneous emission, and frequency dependence.
5. Photon properties.
6. Derivation of de Broglie wavelength for a charged particle accelerated through $V$.

In graph questions, label retarding potential, $-V_0$ if the horizontal axis uses signed collector voltage, and saturation current.

---

## 12. Common traps

1. Saying higher intensity increases photoelectron maximum kinetic energy.
2. Saying sufficiently intense low-frequency light always ejects electrons.
3. Confusing threshold frequency with stopping potential.
4. Using wavelength above $\lambda_0$ as if emission occurs; photoemission requires $\lambda\le\lambda_0$.
5. Treating every emitted electron as having $K_{\max}$; emitted electrons have a distribution up to the maximum.
6. Calling stopping potential the potential that stops emission; it stops collected photocurrent.
7. Losing the electron charge in $K_{\max}=eV_0$ when using joules.
8. Mixing eV and joules.
9. Using $\lambda=h/mv$ relativistically at very high speed.
10. Thinking a stationary massive particle has a finite de Broglie wavelength from the non-relativistic formula; as $p\to0$, wavelength tends to infinity/plane-wave description becomes subtle.
11. Assuming equal velocities or equal energies when a comparison question never states that.
12. Prioritising Davisson-Germer despite its absence from the current official unit wording.

---

## 13. Last-minute checklist

- [ ] I can explain intensity, frequency, saturation current, and stopping potential separately.
- [ ] I know all four major experimental observations.
- [ ] I can explain why classical wave theory fails.
- [ ] I can use $h\nu=\phi+K_{\max}$ in J, eV, frequency, or wavelength form.
- [ ] I can read all standard photoelectric graphs.
- [ ] I know photon energy, momentum, and photon-rate formulas.
- [ ] I can use $\lambda=h/p$ under different equal-condition comparisons.
- [ ] I can derive and use the accelerating-voltage formula.
- [ ] I know the current Davisson-Germer scope warning.

## Official syllabus references

- [CBSE Physics syllabus 2026-27](https://cbseacademic.nic.in/web_material/CurriculumMain27/SecPart2/Physics_SecP2_2026-27.pdf)
- [NTA JEE Main 2026 syllabus page](https://jeemain.nta.nic.in/document/syllabus-2026/)

