# Semiconductor Electronics: Materials, Devices and Simple Circuits - Class 12 Physics

> Reduced-NCERT board notes plus the additional JEE Main material that CBSE removed  
> Source chapter: `leph206(2).pdf` (Chapter 14)  
> Syllabus basis checked: CBSE 2026-27 and JEE Main 2026, on 13 July 2026

## How to use these notes

| Tag | Meaning |
|---|---|
| **[B+J]** | In CBSE 2026-27 and JEE Main 2026 |
| **[B]** | Board-answer/practical emphasis |
| **[J-ONLY]** | Explicitly in JEE Main 2026 but absent from CBSE 2026-27 theory scope and the reduced NCERT PDF |
| **[J]** | JEE problem extension around a shared topic |
| **[OUT]** | Not in either referenced official theory syllabus |

**Important:** The official JEE Main 2027 syllabus was not available on the preparation date. The latest official NTA syllabus, JEE Main 2026, is used provisionally. Recheck this chapter when NTA publishes 2027 because this is the chapter where CBSE and JEE diverge the hardest.

## Navigation

- [1. Exam scope: read this first](#1-exam-scope-read-this-first)
- [2. Energy bands](#2-energy-bands)
- [3. Intrinsic semiconductors](#3-intrinsic-semiconductors)
- [4. Extrinsic semiconductors](#4-extrinsic-semiconductors)
- [5. Formation of a p-n junction](#5-formation-of-a-p-n-junction)
- [6. Junction diode under bias](#6-junction-diode-under-bias)
- [7. Diode I-V characteristics](#7-diode-i-v-characteristics)
- [8. Diode as a rectifier](#8-diode-as-a-rectifier)
- [9. LED](#9-led-j-only)
- [10. Photodiode](#10-photodiode-j-only)
- [11. Solar cell](#11-solar-cell-j-only)
- [12. Zener diode and voltage regulation](#12-zener-diode-and-voltage-regulation-j-only)
- [13. Logic gates](#13-logic-gates-j-only)
- [14. Formula and comparison sheet](#14-formula-and-comparison-sheet)
- [15. Problem-solving playbook](#15-problem-solving-playbook)
- [16. Practical and graph checklist](#16-practical-and-graph-checklist)
- [17. Common traps](#17-common-traps)
- [18. Last-minute checklists](#18-last-minute-checklists)

---

## 1. Exam scope: read this first

### CBSE 2026-27 theory

Electronic Devices is shown as a **7-mark unit**. It includes only:

- energy bands in conductors, semiconductors, and insulators - qualitative;
- intrinsic and extrinsic $p$- and $n$-type semiconductors;
- $p$-$n$ junction;
- diode I-V characteristics in forward and reverse bias;
- junction diode as a rectifier.

That matches the reduced uploaded NCERT chapter, which stops after rectification.

### JEE Main 2026 theory

JEE includes the shared diode content **plus**:

- LED I-V characteristics;
- photodiode;
- solar cell and its I-V characteristics;
- Zener diode and Zener voltage regulator;
- OR, AND, NOT, NAND, and NOR gates.

These JEE-only topics are fully included below and marked **[J-ONLY]**.

### Outside both referenced theory syllabi **[OUT]**

- Bipolar-junction transistor, transistor characteristics/amplifier, oscillator.
- Detailed digital electronics beyond the five named gates; XOR/XNOR are not explicitly listed.
- Communication systems.

Do not resurrect old unreduced-chapter content just because an ancient notes PDF on the internet refuses to move on.

---

## 2. Energy bands

### 2.1 From atomic levels to bands **[B+J]**

When many atoms form a solid, interactions split closely spaced atomic levels into large collections of allowed energy levels called bands.

- **Valence band (VB):** highest occupied band at low temperature; associated mainly with bonding electrons.
- **Conduction band (CB):** higher allowed band in which electrons can move through the crystal and conduct.
- **Forbidden energy gap $E_g$:** energy interval with no allowed electron states between VB and CB.

### 2.2 Classification **[B+J]**

| Material | Band picture | Conductivity behaviour |
|---|---|---|
| Conductor/metal | Partly filled band or overlap of VB and CB | Many mobile electrons even at low temperature |
| Semiconductor | Filled VB and empty CB at $0$ K, separated by small $E_g$ | Thermal/light/doping excitation creates carriers |
| Insulator | Large forbidden gap | Negligible ordinary carrier excitation |

Typical room-temperature band gaps:

- Germanium: about $0.7\ \mathrm{eV}$.
- Silicon: about $1.1\ \mathrm{eV}$.

Exact values depend on temperature and material condition.

### 2.3 Temperature coefficient **[B+J]**

- Metals generally have a positive temperature coefficient of resistance: lattice scattering rises with temperature.
- Semiconductors generally have a negative temperature coefficient: carrier concentration rises strongly with temperature, so resistance decreases.

---

## 3. Intrinsic semiconductors

### 3.1 Covalent-bond picture **[B+J]**

Silicon and germanium are tetravalent. Each atom forms four covalent bonds. At $0$ K in an ideal crystal, bonds are complete, VB is full, CB is empty, and conduction is absent in the simplified picture.

At higher temperature, some bond electrons gain enough energy to enter the conduction band.

### 3.2 Electron-hole pair **[B+J]**

An excited conduction electron leaves an empty state in the valence band called a **hole**.

- Electron behaves as charge $-e$ carrier in CB.
- Hole behaves as effective charge $+e$ carrier in VB.
- Thermal generation creates electrons and holes in pairs.
- Recombination annihilates a conduction electron-hole pair and releases energy.

For an intrinsic semiconductor:

$$
n=p=n_i
$$

where $n$ is electron concentration, $p$ hole concentration, and $n_i$ intrinsic carrier concentration.

### 3.3 Conductivity **[J support]**

$$
\sigma=e(n\mu_e+p\mu_h)
$$

For intrinsic material:

$$
\sigma_i=en_i(\mu_e+\mu_h)
$$

$\mu_e$ and $\mu_h$ are electron and hole mobilities. Usually electron mobility exceeds hole mobility.

### 3.4 Hole motion

A hole is not a separate fundamental particle inside the crystal. Repeated valence-electron hopping into neighbouring vacancies makes the vacancy appear to move opposite to electron motion and in the direction of conventional current.

---

## 4. Extrinsic semiconductors

Doping deliberately adds a very small controlled concentration of impurity atoms to an intrinsic semiconductor.

### 4.1 $n$-type **[B+J]**

Dope Si/Ge with a pentavalent impurity such as P, As, or Sb.

- Four impurity electrons form covalent bonds.
- The fifth is weakly bound and easily enters the conduction band.
- Impurity is a **donor**.
- Electrons are majority carriers; holes are minority carriers.
- Ionised donor atoms are fixed positive ions.

The crystal remains electrically neutral overall. "$n$-type" does not mean the material has a net negative charge.

### 4.2 $p$-type **[B+J]**

Dope with a trivalent impurity such as B, Al, Ga, or In.

- Only three covalent bonds are completed.
- The missing bond electron behaves as a hole.
- Impurity is an **acceptor**.
- Holes are majority carriers; electrons are minority carriers.
- Ionised acceptors are fixed negative ions.

The crystal remains electrically neutral overall.

### 4.3 Comparison

| Feature | $n$-type | $p$-type |
|---|---|---|
| Dopant valency for Si/Ge | 5 | 3 |
| Impurity role | Donor | Acceptor |
| Majority carrier | Electron | Hole |
| Minority carrier | Hole | Electron |
| Fixed ion after ionisation | Positive donor ion | Negative acceptor ion |

### 4.4 Mass-action relation **[J]**

At thermal equilibrium for a non-degenerate semiconductor:

$$
np=n_i^2
$$

Thus increasing majority-carrier concentration reduces minority-carrier concentration.

### 4.5 Energy levels **[B+J qualitative]**

- Donor level lies slightly below conduction band, so donor electrons need little energy to enter CB.
- Acceptor level lies slightly above valence band, so it readily accepts a valence electron and leaves a hole.

---

## 5. Formation of a p-n junction

### 5.1 Why it must be fabricated as one crystal **[B]**

A proper junction is produced by controlled doping within one continuous crystal. Merely pressing separate $p$- and $n$-type slabs together does not make an atomic-scale junction of the required quality.

### 5.2 Diffusion **[B+J]**

Immediately after junction formation:

- Electrons diffuse from high-concentration $n$ side to $p$ side.
- Holes diffuse from $p$ side to $n$ side.
- They recombine near the boundary.

This leaves immobile ions:

- positive donor ions on the $n$ side;
- negative acceptor ions on the $p$ side.

### 5.3 Depletion region **[B+J]**

The junction region depleted of mobile majority carriers is the depletion/space-charge region.

Fixed charges create an electric field directed:

$$
n\text{ side}\rightarrow p\text{ side}
$$

and a built-in barrier potential opposing further majority-carrier diffusion.

### 5.4 Drift-diffusion equilibrium **[B+J]**

- Concentration gradient drives diffusion current.
- Built-in electric field drives drift current in the opposite direction.
- At equilibrium:

$$
I_{\mathrm{diffusion}}=I_{\mathrm{drift}}
$$

so net current is zero.

---

## 6. Junction diode under bias

A semiconductor diode is a $p$-$n$ junction with metallic contacts and two terminals.

### 6.1 Forward bias **[B+J]**

Connection:

$$
p\rightarrow+,
\qquad
n\rightarrow-
$$

Effects:

- Applied field opposes junction field.
- Barrier height decreases.
- Depletion width decreases.
- Majority carriers cross junction readily.
- Current becomes large after the knee/cut-in region.

Forward current is mainly diffusion current and is ordinarily measured in mA.

### 6.2 Reverse bias **[B+J]**

Connection:

$$
p\rightarrow-,
\qquad
n\rightarrow+
$$

Effects:

- Applied field reinforces junction field.
- Barrier height increases.
- Depletion width increases.
- Majority-carrier diffusion is strongly suppressed.
- A small minority-carrier drift current remains.

Reverse current is ordinarily measured in $\mu$A for an ordinary small diode.

### 6.3 Breakdown **[B+J]**

At sufficiently large reverse voltage, reverse current rises sharply. An ordinary diode can be damaged if current is not externally limited. A Zener diode is specially designed to operate safely in a specified reverse-breakdown range.

---

## 7. Diode I-V characteristics

### 7.1 Forward characteristic **[B+J]**

- Very small current at low forward voltage.
- Rapid increase after cut-in/knee voltage.
- Typical approximate cut-in values:
  - Ge: $0.2$-$0.3\ \mathrm V$;
  - Si: about $0.7\ \mathrm V$.

These are useful models, not universal exact constants.

### 7.2 Reverse characteristic **[B+J]**

- Small reverse saturation current, nearly independent of reverse voltage before breakdown.
- Sharp rise at breakdown voltage.
- Reverse saturation current increases strongly with temperature because minority-carrier population rises.

### 7.3 Static and dynamic resistance **[B+J]**

Static/DC resistance at a point:

$$
R=\frac VI
$$

Dynamic/AC resistance near an operating point:

$$
\boxed{r_d=\frac{\Delta V}{\Delta I}}
$$

Use the local graph slope for dynamic resistance; do not automatically use $V/I$.

### 7.4 Ideal diode model **[J]**

- Forward biased: short circuit/zero voltage drop.
- Reverse biased: open circuit/zero current.

For a constant-drop silicon model, a conducting diode has approximately $0.7\ \mathrm V$ drop. Use whichever model the question specifies or clearly implies.

---

## 8. Diode as a rectifier

Rectification converts alternating voltage/current into unidirectional pulsating output.

### 8.1 Half-wave rectifier **[B+J]**

- One diode conducts during one half-cycle and blocks during the other.
- Output contains pulses once per input cycle.
- Ripple/output pulse frequency:

$$
f_{\mathrm{ripple}}=f_{\mathrm{input}}
$$

For an ideal sinusoidal input with output peak $V_m$:

$$
V_{\mathrm{dc}}=\frac{V_m}{\pi},
\qquad
V_{\mathrm{rms}}=\frac{V_m}{2}
$$

Ideal maximum rectification efficiency is about $40.6\%$ and ripple factor about $1.21$ **[J extension]**.

### 8.2 Full-wave rectifier **[B+J]**

Both half-cycles drive load current in the same direction.

Implementations:

- centre-tapped transformer with two diodes;
- bridge rectifier with four diodes.

Ripple frequency:

$$
f_{\mathrm{ripple}}=2f_{\mathrm{input}}
$$

For an ideal sinusoidal output peak $V_m$:

$$
V_{\mathrm{dc}}=\frac{2V_m}{\pi},
\qquad
V_{\mathrm{rms}}=\frac{V_m}{\sqrt2}
$$

Ideal maximum efficiency is about $81.2\%$ and ripple factor about $0.482$ **[J extension]**.

### 8.3 Peak inverse voltage **[J]**

- Half-wave diode: approximately $V_m$.
- Centre-tapped full-wave diode: approximately $2V_m$ per non-conducting diode.
- Bridge diode: approximately $V_m$ per non-conducting diode.

Use the circuit's definition of $V_m$ carefully; transformer half-winding versus full-secondary conventions differ.

### 8.4 Filtering **[B context/J]**

A capacitor across the load charges near output peaks and discharges through the load between peaks, reducing ripple. Larger $RC$ compared with ripple period generally gives smoother output, subject to component ratings and load behaviour.

---

## 9. LED **[J-ONLY]**

### 9.1 Working

A light-emitting diode is a forward-biased junction made from suitable direct-band-gap semiconductors. Injected electrons and holes recombine and emit photons.

Approximate photon energy:

$$
h\nu\approx E_g
$$

$$
\lambda\approx\frac{hc}{E_g}
$$

Colour depends mainly on band gap, not on the plastic package colour.

### 9.2 Characteristics and use

- Operated in forward bias.
- Requires a current-limiting resistor in ordinary circuits.
- Low power, fast switching, long life.
- Forward voltage depends on material/colour and is not always the silicon-diode $0.7$ V value.

The JEE syllabus explicitly names LED I-V characteristics, so recognise its diode-like forward curve and negligible normal reverse operation.

---

## 10. Photodiode **[J-ONLY]**

### 10.1 Working

A photodiode is generally operated in reverse bias.

Incident photons create electron-hole pairs in/near the depletion region. The junction field separates them, increasing reverse current.

### 10.2 Key facts

- Reverse current increases with light intensity.
- Current in darkness is dark current.
- Reverse bias widens depletion region and improves carrier collection/response.
- Used as a light detector, not as a light source.

Graphically, stronger illumination shifts the reverse I-V characteristic to a larger current magnitude.

---

## 11. Solar cell **[J-ONLY]**

### 11.1 Photovoltaic operation

A solar cell is a large-area junction that converts light energy directly into electrical energy, normally without external bias.

Light-generated carriers are separated by the built-in junction field, creating emf and delivering current to a load.

### 11.2 I-V quantities

- **Short-circuit current $I_{sc}$:** current at $V=0$.
- **Open-circuit voltage $V_{oc}$:** voltage at $I=0$.
- Maximum-power point: $(V_m,I_m)$ where $VI$ is maximum.

Fill factor:

$$
FF=\frac{V_mI_m}{V_{oc}I_{sc}}
$$

Efficiency:

$$
\eta=\frac{P_{\max}}{P_{\mathrm{incident}}}
=\frac{V_mI_m}{P_{\mathrm{incident}}}
$$

In the passive sign convention, the illuminated cell's power-delivering region may appear in the fourth quadrant. Focus on magnitudes and axis convention.

---

## 12. Zener diode and voltage regulation **[J-ONLY]**

### 12.1 Zener diode

- Heavily doped junction.
- Thin depletion layer.
- Designed for a sharp, specified reverse breakdown at $V_Z$.
- Operated in reverse bias with current limiting.

Before breakdown, reverse current is small. In the regulation region, voltage remains approximately $V_Z$ while current changes substantially.

### 12.2 Shunt voltage regulator

A series resistor $R_s$ is connected between input and the parallel combination of reverse-biased Zener and load.

Approximate regulated output:

$$
V_o\approx V_Z
$$

Series current:

$$
I_s=\frac{V_{in}-V_Z}{R_s}
$$

Current split:

$$
I_s=I_Z+I_L
$$

$$
I_Z=\frac{V_{in}-V_Z}{R_s}-I_L
$$

For regulation:

$$
I_{Z,\min}\le I_Z\le I_{Z,\max}
$$

Power check:

$$
P_Z=V_ZI_Z\le P_{Z,\mathrm{rated}}
$$

The resistor is not optional; without current limiting, breakdown current can exceed the diode rating.

---

## 13. Logic gates **[J-ONLY]**

Use positive logic: 1 = high, 0 = low.

### 13.1 NOT gate

$$
Y=\overline A
$$

| $A$ | $Y$ |
|---:|---:|
| 0 | 1 |
| 1 | 0 |

### 13.2 Two-input gates

| $A$ | $B$ | OR $A+B$ | AND $AB$ | NAND $\overline{AB}$ | NOR $\overline{A+B}$ |
|---:|---:|---:|---:|---:|---:|
| 0 | 0 | 0 | 0 | 1 | 1 |
| 0 | 1 | 1 | 0 | 1 | 0 |
| 1 | 0 | 1 | 0 | 1 | 0 |
| 1 | 1 | 1 | 1 | 0 | 0 |

Interpretation:

- OR is 1 if at least one input is 1.
- AND is 1 only if all inputs are 1.
- NAND is NOT of AND.
- NOR is NOT of OR.

### 13.3 Universal gates **[J]**

NAND and NOR are universal: either alone can build NOT, AND, and OR.

Using NAND:

$$
\overline A=A\ \mathrm{NAND}\ A
$$

$$
A\cdot B=\overline{A\ \mathrm{NAND}\ B}
$$

Using NOR:

$$
\overline A=A\ \mathrm{NOR}\ A
$$

### 13.4 Boolean identities useful for simplification **[J]**

$$
\overline{AB}=\overline A+\overline B
$$

$$
\overline{A+B}=\overline A\,\overline B
$$

These are De Morgan's laws.

**Scope note:** XOR/XNOR are useful digital gates but are not explicitly named in the JEE Main 2026 list; prioritise the five listed gates.

---

## 14. Formula and comparison sheet

### Shared board + JEE formulas

| Concept | Formula/result |
|---|---|
| Intrinsic carriers | $n=p=n_i$ |
| Conductivity | $\sigma=e(n\mu_e+p\mu_h)$ |
| Mass action | $np=n_i^2$ **[J]** |
| Dynamic diode resistance | $r_d=\Delta V/\Delta I$ |
| Half-wave pulse frequency | $f_r=f$ |
| Full-wave pulse frequency | $f_r=2f$ |

### Rectifier ideal results **[J extension]**

| Quantity | Half wave | Full wave |
|---|---:|---:|
| $V_{dc}$ | $V_m/\pi$ | $2V_m/\pi$ |
| $V_{rms}$ | $V_m/2$ | $V_m/\sqrt2$ |
| Max efficiency | $40.6\%$ | $81.2\%$ |
| Ripple factor | $1.21$ | $0.482$ |

### JEE-only formulas

| Device | Formula |
|---|---|
| LED photon | $E_\gamma\approx E_g$, $\lambda\approx hc/E_g$ |
| Solar fill factor | $FF=V_mI_m/(V_{oc}I_{sc})$ |
| Solar efficiency | $\eta=V_mI_m/P_{in}$ |
| Zener series current | $I_s=(V_{in}-V_Z)/R_s$ |
| Zener current | $I_Z=I_s-I_L$ |
| Zener power | $P_Z=V_ZI_Z$ |

---

## 15. Problem-solving playbook

### 15.1 Identify diode state **[B+J]**

1. Mark $p$ side/anode and $n$ side/cathode from the symbol/circuit.
2. Compare terminal potentials.
3. Forward bias if $p$ is sufficiently above $n$ potential.
4. Replace diode by the chosen model: ideal short, constant drop, or open.
5. Solve circuit, then verify the assumed state is self-consistent.

### 15.2 I-V graph

- Static resistance: line from origin to operating point.
- Dynamic resistance: reciprocal slope idea locally, $\Delta V/\Delta I$.
- Convert mA or $\mu$A to amperes before reporting ohms.

### 15.3 Rectifier waveform

Trace one half-cycle at a time:

1. Mark transformer polarity.
2. Decide which diode(s) conduct.
3. Draw current direction through load.
4. Repeat after polarity reverses.
5. Confirm load current remains same direction for full-wave rectification.

### 15.4 Zener regulator **[J-ONLY]**

1. Assume regulation: $V_o=V_Z$.
2. Calculate $I_s$.
3. Calculate load current $I_L=V_Z/R_L$.
4. Find $I_Z=I_s-I_L$.
5. Verify $I_Z$ is within regulation/current rating and check $P_Z$.
6. If $I_Z<0$ or below knee current, Zener is not regulating; re-solve without the regulated-voltage assumption.

### 15.5 Logic circuit **[J-ONLY]**

Work from input to output gate by gate. Introduce intermediate labels, apply truth tables or Boolean expressions, then use De Morgan's laws. Do not mentally skip inversion bubbles.

---

## 16. Practical and graph checklist

### CBSE practical overlap **[B]**

CBSE includes drawing the forward- and reverse-bias I-V characteristic of a $p$-$n$ junction diode and identifying basic components.

Know:

- correct bias circuit;
- milliammeter for forward current and microammeter for reverse current;
- voltmeter placement;
- rheostat/current-limiting resistor;
- forward knee and reverse saturation regions;
- basic precautions, including staying within current and reverse-voltage ratings.

### JEE experimental-skills overlap **[J]**

The official JEE experimental-skills list includes:

- $p$-$n$ diode characteristic curves;
- Zener characteristic and breakdown voltage;
- identification of diode, LED, resistor, and capacitor.

### Identification clues

- Ordinary diode: band commonly marks cathode.
- LED: longer lead is commonly anode and flat package side commonly cathode, but verify because leads may have been cut.
- Resistor: colour bands/ohmmeter behaviour.
- Capacitor: capacitance marking and, if electrolytic, polarity marking.

---

## 17. Common traps

1. Saying holes are physical positively charged particles injected into the crystal from nowhere.
2. Saying $n$-type material is negatively charged or $p$-type is positively charged; both are neutral overall.
3. Reversing donor/acceptor fixed-ion signs.
4. Drawing junction electric field from $p$ to $n$; it points from positive donor ions on $n$ side toward negative acceptor ions on $p$ side.
5. Reversing forward-bias connection: $p$ goes positive, $n$ negative.
6. Saying reverse current is exactly zero in a real diode before breakdown.
7. Using $V/I$ when dynamic resistance is asked.
8. Assuming every silicon-based junction device has exactly $0.7$ V forward drop.
9. Drawing a full-wave output with alternating load-current direction.
10. Saying a photodiode is normally forward biased.
11. Saying an LED is used in reverse breakdown.
12. Treating a solar cell as an externally forward-biased LED.
13. Connecting a Zener in forward bias for voltage regulation.
14. Omitting the Zener series resistor/current and power checks.
15. Reversing NAND/NOR truth tables.
16. Studying transistors for this current official theory unit while neglecting JEE's actual LED/Zener/logic-gate additions.

---

## 18. Last-minute checklists

### CBSE board core

- [ ] I can compare conductor, semiconductor, and insulator bands qualitatively.
- [ ] I understand intrinsic electron-hole generation and recombination.
- [ ] I can compare $n$- and $p$-type doping and carriers.
- [ ] I can explain junction formation, depletion region, and barrier potential.
- [ ] I can explain forward/reverse bias and draw the I-V curve.
- [ ] I can trace half-wave and full-wave rectifier waveforms.

### JEE additions

- [ ] I know LED operation and the band-gap/colour link.
- [ ] I know why a photodiode is reverse biased and how light changes current.
- [ ] I know solar-cell $I_{sc}$, $V_{oc}$, fill factor, and efficiency.
- [ ] I can solve a Zener regulator and check current/power limits.
- [ ] I know NOT, OR, AND, NAND, and NOR truth tables.
- [ ] I can simplify simple NAND/NOR networks with De Morgan's laws.
- [ ] I know transistors are outside the referenced current theory syllabi.

## Official syllabus references

- [CBSE Physics syllabus 2026-27](https://cbseacademic.nic.in/web_material/CurriculumMain27/SecPart2/Physics_SecP2_2026-27.pdf)
- [NTA JEE Main 2026 syllabus page](https://jeemain.nta.nic.in/document/syllabus-2026/)

