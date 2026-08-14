# Nuclei - Class 12 Physics

> NCERT-aligned board notes with a JEE Main problem-solving layer  
> Source chapter: `leph205.pdf` (Chapter 13)  
> Syllabus basis checked: CBSE 2026-27 and JEE Main 2026, on 13 July 2026

## How to use these notes

| Tag | Meaning |
|---|---|
| **[B+J]** | Required for CBSE boards and explicitly relevant to JEE Main |
| **[B]** | Explicit CBSE or board-answer emphasis |
| **[J]** | JEE Main extension or fast numerical result |
| **[OUT]** | Printed/contextual material outside current official CBSE and JEE Main Physics scope |

**Important:** The official JEE Main 2027 syllabus was not available on the preparation date. JEE tags use the latest official NTA syllabus, JEE Main 2026, provisionally.

## Navigation

- [1. Exam scope and the radioactivity trap](#1-exam-scope-and-the-radioactivity-trap)
- [2. Nuclear composition and notation](#2-nuclear-composition-and-notation)
- [3. Atomic and nuclear masses](#3-atomic-and-nuclear-masses)
- [4. Nuclear size and density](#4-nuclear-size-and-density)
- [5. Mass-energy equivalence](#5-mass-energy-equivalence)
- [6. Mass defect and binding energy](#6-mass-defect-and-binding-energy)
- [7. Binding-energy curve](#7-binding-energy-curve)
- [8. Nuclear force](#8-nuclear-force)
- [9. Radioactivity section in the PDF](#9-radioactivity-section-in-the-pdf)
- [10. Nuclear fission](#10-nuclear-fission)
- [11. Nuclear fusion](#11-nuclear-fusion)
- [12. Formula sheet](#12-formula-sheet)
- [13. Numerical playbook](#13-numerical-playbook)
- [14. Board answer map](#14-board-answer-map)
- [15. Common traps](#15-common-traps)
- [16. Last-minute checklist](#16-last-minute-checklist)

---

## 1. Exam scope and the radioactivity trap

### CBSE 2026-27

Explicit scope:

- composition and size of nucleus;
- nuclear force;
- mass-energy relation and mass defect;
- binding energy per nucleon and its variation with mass number;
- nuclear fission and fusion.

CBSE groups Dual Nature, Atoms, and Nuclei into a shared **12-mark block**, without a fixed chapter-wise split.

### JEE Main 2026

Explicit scope:

- composition and size;
- atomic masses;
- mass-energy relation and mass defect;
- binding energy per nucleon and its variation;
- fission and fusion.

Nuclear force is not separately named in the NTA line, but it is explicit for CBSE and is needed for conceptual coherence.

### The important mismatch

> **[OUT] Radioactivity is briefly printed as Section 13.6 in the uploaded NCERT PDF, but radioactivity, decay law, decay constant, activity, and half-life are absent from both the official CBSE 2026-27 Nuclei syllabus and the official JEE Main 2026 Physics syllabus.**

These notes preserve a tiny labelled record of what the PDF says, but do not mix radioactivity formulas into the assessed formula sheet. This is exactly the sort of reduced-syllabus ambush that wastes revision time.

---

## 2. Nuclear composition and notation

### 2.1 Nucleons **[B+J]**

The nucleus contains:

- protons: charge $+e$, number $Z$;
- neutrons: charge $0$, number $N$.

Protons and neutrons together are nucleons.

Mass number:

$$
A=Z+N
$$

Nuclide notation:

$$
{}^A_ZX
$$

### 2.2 Classification **[B+J]**

| Term | Same | Different |
|---|---|---|
| Isotopes | $Z$ | $N$, hence $A$ |
| Isobars | $A$ | $Z$ |
| Isotones | $N$ | $Z$, hence $A$ |

Chemical behaviour is governed mainly by electron arrangement and hence $Z$; isotopes therefore have nearly identical chemistry but different nuclear properties/masses.

### 2.3 Nuclear charge and approximate mass

$$
Q_{\mathrm{nucleus}}=+Ze
$$

Nuclear mass is roughly $A$ atomic mass units, but accurate binding calculations must use tabulated masses rather than $A\,u$.

---

## 3. Atomic and nuclear masses

### 3.1 Atomic mass unit **[B+J]**

One unified atomic mass unit is defined as one-twelfth of the mass of a neutral carbon-12 atom in its ground state:

$$
1\,u=1.66054\times10^{-27}\ \mathrm{kg}
$$

Energy equivalent:

$$
1\,u\,c^2\approx931.5\ \mathrm{MeV}
$$

### 3.2 Useful masses

Approximate standard values:

| Particle/atom | Mass in $u$ |
|---|---:|
| Proton $m_p$ | $1.007276$ |
| Neutron $m_n$ | $1.008665$ |
| Electron $m_e$ | $0.0005486$ |
| Hydrogen atom $m_H$ | $1.007825$ |

Use the masses supplied in the question when given; small tabulation differences affect final MeV values.

### 3.3 Atomic mass versus nuclear mass **[B+J]**

- **Atomic mass** includes $Z$ electrons.
- **Nuclear mass** excludes electrons.

Electron binding energies are tiny on the MeV nuclear scale and are usually neglected in Class 12 calculations, but electron masses must be cancelled consistently.

---

## 4. Nuclear size and density

### 4.1 Radius relation **[B+J]**

Experimental nuclear radii follow:

$$
\boxed{R=R_0A^{1/3}}
$$

with:

$$
R_0\approx1.2\ \mathrm{fm},
\qquad
1\ \mathrm{fm}=10^{-15}\ \mathrm m
$$

Consequences:

- Nuclear volume $\propto R^3\propto A$.
- Nuclear volume per nucleon is nearly constant.

### 4.2 Nearly constant nuclear density **[B+J]**

Approximating nuclear mass as $Am_N$:

$$
\rho=\frac{Am_N}{\frac43\pi R_0^3A}
$$

$$
\boxed{\rho=\frac{3m_N}{4\pi R_0^3}}
$$

Thus $A$ cancels: nuclei have approximately the same mean density, of order:

$$
10^{17}\ \mathrm{kg\,m^{-3}}
$$

### 4.3 Radius ratios **[J]**

For two nuclei:

$$
\frac{R_1}{R_2}=\left(\frac{A_1}{A_2}\right)^{1/3}
$$

If mass number increases by a factor of 8, radius only doubles.

---

## 5. Mass-energy equivalence

### 5.1 Einstein relation **[B+J]**

$$
E=mc^2
$$

A change in rest mass corresponds to energy change:

$$
\Delta E=\Delta m\,c^2
$$

Nuclear energies are commonly expressed in electron volts:

$$
1\ \mathrm{eV}=1.602\times10^{-19}\ \mathrm J
$$

$$
1\ \mathrm{MeV}=10^6\ \mathrm{eV}
$$

### 5.2 Q-value of a reaction **[B+J]**

For a nuclear reaction:

$$
Q=(\text{total initial rest mass}-\text{total final rest mass})c^2
$$

- $Q>0$: energy is released.
- $Q<0$: at least $|Q|$ plus any momentum-related threshold requirement must be supplied.

If masses are in $u$:

$$
Q(\mathrm{MeV})=\Delta m(u)\times931.5
$$

Conserve electric charge, nucleon number, total energy, and momentum.

---

## 6. Mass defect and binding energy

### 6.1 Why nuclear mass is smaller **[B+J]**

A bound nucleus has lower total energy than separated free nucleons. Its mass is therefore smaller than the sum of the free-nucleon masses.

### 6.2 Using nuclear masses **[B+J]**

$$
\boxed{\Delta m=Zm_p+Nm_n-M_{\mathrm{nucleus}}}
$$

### 6.3 Using atomic masses **[B+J]**

Use hydrogen-atom mass so electron masses cancel:

$$
\boxed{\Delta m=Zm_H+Nm_n-M_{\mathrm{atom}}}
$$

Do not mix $m_p$ with a neutral atomic mass unless you separately account for the $Z$ electrons.

### 6.4 Binding energy **[B+J]**

Energy required to separate a nucleus completely into free nucleons:

$$
\boxed{B=\Delta m\,c^2}
$$

If $\Delta m$ is in $u$:

$$
\boxed{B(\mathrm{MeV})=\Delta m(u)\times931.5}
$$

### 6.5 Binding energy per nucleon **[B+J]**

$$
\boxed{\frac BA=\frac{\Delta m\,c^2}{A}}
$$

It is a useful average measure of nuclear stability. Comparing total binding energy alone can be misleading when $A$ differs greatly.

### 6.6 Separation energy **[J support]**

Energy required to remove one neutron:

$$
S_n=[M(A-1,Z)+m_n-M(A,Z)]c^2
$$

Analogous proton separation must handle atomic/nuclear masses consistently. This is an application of mass defect, not a separate official heading.

---

## 7. Binding-energy curve

### 7.1 Shape **[B+J]**

For a graph of $B/A$ against mass number $A$:

1. It rises rapidly for very light nuclei.
2. It reaches about $8\ \mathrm{MeV}$ by moderate $A$.
3. It is broad and nearly flat through medium-mass nuclei.
4. It peaks near the iron/nickel region at roughly $8.8\ \mathrm{MeV}$ per nucleon.
5. It slowly decreases for very heavy nuclei.

### 7.2 Stability interpretation **[B+J]**

Higher $B/A$ generally means nucleons are more tightly bound and the nucleus is more stable against breakup into free nucleons.

### 7.3 Why fission releases energy

Very heavy nuclei have lower $B/A$ than medium-mass products. Splitting moves nucleons upward on the $B/A$ curve, increasing total binding energy. The corresponding mass decrease appears as released energy.

### 7.4 Why fusion releases energy

Very light nuclei have low $B/A$. Combining them into a heavier light/medium nucleus increases $B/A$, so total binding energy rises and energy is released.

### 7.5 Saturation clue

The roughly constant $B/A$ for a broad range of $A$ indicates that each nucleon interacts strongly only with nearby nucleons, not equally with every other nucleon. This reflects the short-range, saturating nature of nuclear force.

---

## 8. Nuclear force

### 8.1 Properties **[B]**

1. Extremely strong at nuclear distances.
2. Short ranged, effective over a few femtometres.
3. Approximately charge independent: proton-proton, neutron-neutron, and proton-neutron nuclear interactions are broadly similar after separating electromagnetic effects.
4. Attractive over normal nucleon separations.
5. Strongly repulsive at very small separation, preventing collapse.
6. Shows saturation: a nucleon interacts mainly with close neighbours.

### 8.2 Nuclear versus Coulomb force

- Coulomb proton-proton repulsion is long-ranged and depends on charge.
- Nuclear attraction is much stronger at short range and binds protons and neutrons.
- In very heavy nuclei, accumulated Coulomb repulsion contributes to reduced stability and makes fission energetically favourable.

No simple school-level inverse-power formula describes nuclear force across all distances.

---

## 9. Radioactivity section in the PDF

### 9.1 What the uploaded PDF briefly contains **[OUT]**

The chapter states that an unstable nucleus may undergo spontaneous radioactive change and qualitatively names alpha, beta, and gamma emission.

### 9.2 What not to add to current board/JEE Physics revision **[OUT]**

Do not treat the following as part of the official 2026-27 CBSE or JEE Main 2026 Physics unit unless a later syllabus explicitly restores them:

- decay law $N=N_0e^{-\lambda t}$;
- activity and decay constant;
- half-life/mean-life relations;
- detailed alpha/beta/gamma decay equations and displacement laws.

First-order kinetics in Chemistry is a separate assessed topic and should not be confused with this Physics syllabus deletion.

---

## 10. Nuclear fission

### 10.1 Definition **[B+J]**

Fission is the splitting of a heavy nucleus into two medium-mass fragments, usually with neutrons and energy released.

A representative balanced pattern is:

$$
{}^{235}_{92}\mathrm U+{}^1_0\mathrm n
\rightarrow{}^{141}_{56}\mathrm{Ba}+{}^{92}_{36}\mathrm{Kr}
+3{}^1_0\mathrm n+Q
$$

Actual fragment pairs can vary; the essential checks are conservation of $A$ and $Z$ and positive $Q$.

### 10.2 Chain reaction concept **[B context]**

Neutrons released by one fission can trigger further fissions. In a controlled energy system the multiplication is regulated; an uncontrolled growth releases energy too rapidly. Detailed reactor engineering is outside this chapter's official scope.

### 10.3 Energy calculation **[B+J]**

Use either:

1. initial-final mass difference; or
2. difference between total binding energies of products and reactants.

$$
Q=B_{\mathrm{products}}-B_{\mathrm{reactants}}
$$

when free-particle rest masses cancel consistently.

---

## 11. Nuclear fusion

### 11.1 Definition **[B+J]**

Fusion is the combination of light nuclei into a heavier nucleus with greater binding energy per nucleon, releasing energy.

Representative deuterium-tritium reaction:

$$
{}^2_1\mathrm H+{}^3_1\mathrm H
\rightarrow{}^4_2\mathrm{He}+{}^1_0\mathrm n+17.6\ \mathrm{MeV}
$$

### 11.2 Why high temperature is needed **[B+J]**

Both nuclei are positively charged and repel electrically. Very high kinetic energy and suitable confinement increase the probability of reaching separations where the short-range nuclear force can bind them.

Fusion powers stars. Its energy origin is increased total binding energy, not destruction of nucleons.

### 11.3 Fission versus fusion

| Feature | Fission | Fusion |
|---|---|---|
| Starting nuclei | Heavy | Light |
| Process | Split | Combine |
| Energy reason | Products have higher $B/A$ | Product has higher $B/A$ |
| Initiation issue | Neutron capture/instability can initiate | Coulomb barrier requires very high energies/temperatures |

---

## 12. Formula sheet

| Concept | Formula |
|---|---|
| Nucleon count | $A=Z+N$ |
| Nuclear radius | $R=R_0A^{1/3}$ |
| Mean density | $\rho=3m_N/(4\pi R_0^3)$ |
| Nuclear-mass defect | $\Delta m=Zm_p+Nm_n-M_{\rm nuc}$ |
| Atomic-mass defect | $\Delta m=Zm_H+Nm_n-M_{\rm atom}$ |
| Binding energy | $B=\Delta mc^2$ |
| MeV conversion | $B(\mathrm{MeV})=\Delta m(u)\times931.5$ |
| Binding per nucleon | $B/A$ |
| Reaction Q | $Q=(M_i-M_f)c^2$ |

Constants:

- $R_0\approx1.2\ \mathrm{fm}$.
- $1\ \mathrm{fm}=10^{-15}\ \mathrm m$.
- $1u=1.66054\times10^{-27}\ \mathrm{kg}$.
- $1u\,c^2=931.5\ \mathrm{MeV}$.

Radioactive-decay formulas are intentionally absent because they are **[OUT]** for the referenced official Physics syllabi.

---

## 13. Numerical playbook

### 13.1 Radius/density

- Use ratios to avoid constants: $R_1/R_2=(A_1/A_2)^{1/3}$.
- For density, show $A$ cancellation explicitly.
- Convert fm to m only at the final SI step.

### 13.2 Binding energy from atomic mass

1. Calculate $N=A-Z$.
2. Use $Zm_H+Nm_n-M_{\rm atom}$.
3. Confirm $\Delta m>0$ for a bound nucleus.
4. Multiply by $931.5$ MeV/u.
5. Divide by $A$ only if $B/A$ is asked.

### 13.3 Binding energy from nuclear mass

Use $Zm_p+Nm_n-M_{\rm nucleus}$. Never swap between atomic and nuclear formulas halfway through.

### 13.4 Q-value

1. Balance $A$ and $Z$ first.
2. Add all initial masses and all final masses.
3. Electron masses may cancel if neutral atomic masses appear with equal total $Z$ on both sides.
4. Compute $Q=(M_i-M_f)931.5$ MeV.
5. Positive $Q$ means released kinetic/radiative energy while total energy remains conserved.

### 13.5 Binding-energy-per-nucleon data

If only $B/A$ and $A$ are given:

$$
B=A(B/A)
$$

Find reaction energy from final total binding energy minus initial total binding energy.

---

## 14. Board answer map

Prepare:

1. Nuclide notation, isotopes/isobars/isotones.
2. Derivation that nuclear density is nearly independent of $A$.
3. Mass defect and binding energy using both atomic and nuclear masses.
4. A labelled $B/A$ versus $A$ curve with four regions and stability interpretation.
5. Properties of nuclear force.
6. Conceptual explanations of energy release in fission and fusion using the binding-energy curve.

Do not include a long radioactivity answer unless the actual exam's updated official syllabus or question explicitly restores it.

---

## 15. Common traps

1. Writing $A=Z-N$ instead of $Z+N$.
2. Confusing isotopes, isobars, and isotones.
3. Assuming radius is proportional to $A$ rather than $A^{1/3}$.
4. Saying heavier nuclei necessarily have higher density; mean nuclear density is nearly constant.
5. Mixing atomic mass with proton mass without handling electron masses.
6. Subtracting masses in the wrong order and obtaining negative binding energy.
7. Comparing stability using total $B$ instead of $B/A$.
8. Saying iron-region nuclei have the largest total binding energy; the key maximum is binding **per nucleon**.
9. Claiming fission/fusion releases energy because mass disappears; mass-energy is conserved and rest mass becomes other energy forms.
10. Forgetting to conserve both $A$ and $Z$ in a nuclear equation.
11. Treating nuclear force as long-range or simply inverse-square.
12. Revising decay-law/half-life formulas for this Physics chapter despite their current official exclusion.

---

## 16. Last-minute checklist

- [ ] I can find $Z$, $N$, and $A$ and classify nuclides.
- [ ] I know $R=R_0A^{1/3}$ and can prove density is nearly constant.
- [ ] I know when to use $m_H$ versus $m_p$ in mass defect.
- [ ] I can convert $u$ to MeV and calculate $B$ and $B/A$.
- [ ] I can sketch and explain the binding-energy curve.
- [ ] I know all key nuclear-force properties.
- [ ] I can calculate a reaction Q-value.
- [ ] I can explain fission and fusion energy using increased binding energy.
- [ ] I remember that radioactivity is printed but outside current CBSE/JEE Main Physics scope.

## Official syllabus references

- [CBSE Physics syllabus 2026-27](https://cbseacademic.nic.in/web_material/CurriculumMain27/SecPart2/Physics_SecP2_2026-27.pdf)
- [NTA JEE Main 2026 syllabus page](https://jeemain.nta.nic.in/document/syllabus-2026/)

