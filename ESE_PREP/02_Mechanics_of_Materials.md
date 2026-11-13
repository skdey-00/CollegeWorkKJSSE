# 02 · Mechanics of Materials (316U43C302) — ESE Question Bank

50 marks · 2 hrs · Q1 any-two ×5 · Q2 any-one ×10 · Q3 any-one ×10 · Q4 both ×5 · Q5 both/any ×5

Real RAI paper analysed: Nov–Dec 2025 (filed as "Strength of Materials", programme code 43 = RAI). Reinforced with Mech KT papers (SVU2020/2023) and SOM Dec 2020/Nov 2021, which share the same question factory.

---

## CHEAT SHEET — what repeats

| # | Recurring item | Evidence |
|---|----------------|----------|
| 1 | **Mohr's circle: principal stresses + directions + max shear** | RAI ND25 Q3, KT25 Q4(iii), Dec20 Q3(a) |
| 2 | **Macaulay's method: deflection/slope of beam** (answer in EI terms) | RAI ND25 Q4, KT25 Q4(ii), Dec20 Q3(b) |
| 3 | **Bending stress numerical** (simply supported, given cross-section; find max stress or safe load W) | RAI ND25 Q3(ii), KT25 Q2B, Dec20 Q2, ND21 Q3(a) |
| 4 | **Torsion numerical: power transmitted / shear stress / angle of twist** | KT25 Q4(i), Dec20 Q3(c), ND21 Q4(a) & Q1B(b) |
| 5 | **Composite/two-material bar, thermal stress** | RAI ND25 Q2 (copper+steel rod), ND21 Q2(b),(c), Dec20 objective |
| 6 | **Fatigue + S-N curve** (theory) | RAI ND25 Q5 |
| 7 | **Stress-strain graph terms / elastic constants / factor of safety** (Q1 short-theory bank) | KT25 Q1, Dec20 obj |
| 8 | **Shear stress distribution across rectangular vs circular section** | KT25 Q5, ND21 Q3(b) |

RAI ND25 full breakdown: Q1 = composite materials / corrosion types / stacking fault (module 1+5 theory). Q2 = composite bar numerical + thermal(?) / inclined-plane→Mohr setup. Q3 = Mohr's circle 10-marker + bending stress 10-marker. Q4 = Macaulay. Q5 = fatigue + S-N curve.

---

## MODULE 1 — Materials & Deformation (theory goldmine)

### Possible questions
1. Classification of materials: metals/polymers/ceramics/composites — definition, properties, applications. *(RAI ND25 asked composites specifically)*
2. Lattice imperfections: point defects (vacancy, interstitial, impurity) — formation & effects.
3. Edge vs screw dislocation, Burgers vector; motion of dislocations; Frank-Read source.
4. Surface defects: grain boundary, sub-angle boundary, **stacking faults** *(asked ND25 as short note)*.
5. Deformation mechanism in single vs polycrystal; slip systems; critical resolved shear stress (numerical possible: σ_y = τ_crss / (cosφ cosλ)).
6. Strain hardening: definition, dislocation theory, effect on material behaviour.
7. Recrystallization annealing: stages, factors affecting it.
8. Short notes: Schottky defect, atomic packing factor, ductility, endurance limit, creep (these were the Material-Sci paper's Q1 bank — same BoS examiners).

### Notes to remember
- APF: FCC & HCP = 0.74, BCC = 0.68, SC = 0.52.
- Edge dislocation: Burgers vector ⊥ dislocation line; screw: parallel.
- Frank-Read source: pinned dislocation segment bows and multiplies under stress.
- Recrystallization stages: recovery → recrystallization → grain growth.
- Hume-Rothery / Griffith questions came in the Mech Material-Sci paper — Griffith's theory is in YOUR module 5 too (see below).

## MODULE 2 — Stress, Strain, Deformation

### Possible questions
1. Stress-strain diagram for ductile material: label yield, ultimate, elastic/plastic zones. *(KT25 Q1)*
2. Elastic constants E, G, K, μ and relations: E=2G(1+μ)=3K(1−2μ). Derive E–G relation *(KT25 Q5)*.
3. Hooke's law, factor of safety, Poisson's ratio definitions *(KT25 Q1 v)*.
4. **Axial numericals**: rod under pull → stress, strain, elongation *(KT25 Q2 & Q1)*; strain energy stored *(KT25, Dec20 obj, ND21)*.
5. **Composite bar numerical**: copper + steel supporting load, find stresses (use ΔL_same for both: σs·L/Es = σc·L/Ec) *(RAI ND25 Q2)*.
6. **Thermal stress**: rod fixed both ends, ΔT given → σ = EαΔT (ND21 asked twice with yielding supports).
7. Principal stresses on inclined planes; analytical + graphical (feeds Mohr's Q3).
8. Volumetric strain: e = εx+εy+εz; relation with μ.
9. Modes of failure; eccentric loading & core/limit of eccentricity (square: S/6 middle-third rule — ND21 MCQ).

### Notes to remember
- Elongation δ = PL/AE. Strain energy U = P²L/2AE = σ²V/2E (gradual load); sudden load ×4... 
- Thermal: if fully restrained σ = αEΔT; partial yielding δ_support → subtract.
- Strain energy scales with 1/d² at fixed P... diameter +10% → U changes by 1/1.1² ≈ −17.4% (Dec20 asked exactly this).
- Composite bar: same extension ⇒ σ₁/E₁ = σ₂/E₂; load shared P = σ₁A₁+σ₂A₂.

## MODULE 3 — Stresses in Beams

### Possible questions
1. SF/BM due to point load, UDL, UVL (no SFD/BMD diagrams per syllabus — but KT asked "explain with figures", so know shapes). Max BM formulas: SS+central point W → WL/4; SS+UDL → wL²/8; cantilever+UDL → wL²/2.
2. **Bending stress numerical**: SS beam with rectangular/T-section, find max bending stress or safe W. *(RAI ND25: 150 wide × 300 deep; Dec20: T-section 80×10 flange)*
3. Derive flexural formula M/I = σ/y = E/R *(RAI ND25 Q3 short)*.
4. Shear stress distribution: τ = VAȳ/(Ib); rectangular max = 1.5×avg; circular max = 4/3×avg. Draw distributions *(KT25 Q5)*.
5. I-section shear: three plates 50×200 forming I, same max shear redesign question *(ND21 Q3(c))*.
6. Eccentric loading: stress at points of section under eccentric compressive loads (pier with P1..P5 at points A,B,C,D,O *(ND21 Q3(c))*); T-section eccentric P *(ND21 Q3(c) variant)*.
7. Area moment of inertia computation for given section (rectangle, circle — feeding Q3 numericals).

### Notes to remember
- σ_max = M·y_max/I. For rectangle bh³/12, y=b/2 → Z = bh²/6. Circle: I = πd⁴/64, Z = πd³/32.
- Rect shear: parabolic, max at NA = 1.5 V/A. Circle: 4/3·V/A.
- Eccentric: σ = P/A ± M·y/I combined at corner points; "core/middle third" for no tension: e ≤ S/6.
- Hollow box section shear stress (ND21 asked) — same formula with b = 2×wall thickness at NA.

## MODULE 4 — Torsion + Deflection

### Possible questions
1. **Torsion numerical family**: shaft d, T or power+rpm → τ_max, θ, or find T_max safe. *(KT25 Q4: hollow shaft 200 od, 25 thick, 200 rpm, 0.5°/2m; Dec20: 300 kW 180 rpm, T_max=1.25 T_mean)*
2. Compare hollow vs solid shaft (same strength / same weight) — theory short.
3. Torsional rigidity GJ, polar modulus Zp — definitions & formula.
4. Compound shaft steel+aluminium with two torques → max permissible T₀ *(ND21 Q4(a))*.
5. Principal stresses from pure torsion: σ₁,₂ = ±τ → "torsion induces 40 MPa shear, find principal stresses" *(ND21 Q1B(d))*.
6. **Macaulay's method**: cantilever / SS / overhanging beam, point load + UDL, slope & deflection at a point in terms of EI. *(RAI ND25 Q4 with "find W" twist; KT25: slope+deflection at C; Dec20: cantilever UDL)*
7. Cantilever with end couple: slope at free end = ML/EI *(ND21 Q4(c))*.

### Notes to remember
- T/J = τ/r = Gθ/L. Power P = 2πNT/60 (N rpm, T in Nm → W). τ_max = 16T/πd³ (solid); hollow: J = π(D⁴−d⁴)/32.
- T_max for given τ: T = τ·Zp.
- Macaulay steps: reactions → write bending moment with (x−a) brackets → integrate twice, constants from boundary → substitute target x. Terms with negative bracket value = 0.
- Standard checks: SS + central W: δ = WL³/48EI. Cantilever + UDL: δ = wL⁴/8EI.

## MODULE 5 — Failure (RAI ND25 dedicated Q5 here — don't skip theory)

### Possible questions
1. **Fatigue: definition, cyclic stress, mechanism, fatigue testing, S-N curve, factors affecting fatigue** *(RAI ND25 Q5 — a guaranteed-style repeat topic)*.
2. **Creep: definition, classical creep curve stages, mechanism/types, creep testing, creep-resistant materials**.
3. Brittle fracture: **Griffith's theory + derivation**; Orowan's modification; crack propagation. *(Asked in Mech MSM ND25 paper — same examiner pool)*
4. Ductile fracture, notch effect, fracture toughness; ductile-brittle transition & factors.
5. Corrosion basics + **stress-corrosion cracking**; types of corrosion *(RAI ND25 Q1)*.
6. Strain hardening / dislocation theory of fracture (bridge from module 1).

### Notes to remember
- S-N curve: stress amplitude vs log(cycles to failure). Steel shows endurance limit (horizontal asymptote); aluminium doesn't.
- Fatigue factors: surface finish, size, temperature, stress concentration, residual stresses.
- Creep curve: primary (decreasing rate), secondary (steady), tertiary (accelerating → rupture).
- Griffith: σ_f = √(2Eγ_s/πa) for thin plate; Orowan added plastic work γ_p ≫ γ_s.
- SCC needs: susceptible material + corrosive environment + tensile stress.

---

## PRACTICE PRIORITY
Numericals: (1) Mohr's circle, (2) Macaulay, (3) bending stress with section, (4) torsion power problem, (5) composite/thermal bar. Theory: fatigue+S-N, creep, Griffith, dislocations — one full 10-mark theory answer is near-certain.
