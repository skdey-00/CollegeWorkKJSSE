# MoM — DEMO PAPERS (3 papers, exam format: 50 marks · 2 hrs)

Format cloned from RAI ND-2025 (filed as Strength of Materials 216U43C302): Q1 any-two ×5 · Q2 any-one ×10 · Q3 any-one ×10 · Q4 both ×5 · Q5 both ×5.

---

# =================== DEMO PAPER 1 ===================

**Q1. Attempt any two:** *(2×5=10)*
(i) What are metallic materials, polymers, ceramics and composites? Give two applications of composites in robotics.
(ii) Differentiate edge dislocation and screw dislocation. What is Burgers vector?
(iii) Write a short note on **fracture toughness** and its significance.

**Q2. Attempt any one:** *(10)*
(i) A copper rod (d = 25 mm, E = 1×10⁵ MPa) and steel rod (d = 20 mm, E = 2×10⁵ MPa) rigidly support a load of 25 kN between them, both 1.5 m long. Find the stress in each and the extension. (Both shorten equally... equal deformation.)
(ii) A steel bar 40 mm × 40 mm, 2 m long carries an axial pull of 128 kN. E = 200 GPa. Find elongation and strain energy stored.

**Q3. Attempt any one:** *(10)*
(i) At a point in a strained material σx = 80 MPa (tension), σy = 40 MPa (compression), τ = 30 MPa. Determine principal stresses and their directions, and max shear stress — **analytically and by Mohr's circle** (draw the circle to scale).
(ii) A simply supported beam of span 5 m carries a UDL of 10 kN/m. Section: 150 mm wide × 300 mm deep rectangle. Determine max bending stress and the section modulus.

**Q4. Attempt the following:** *(5+5=10)*
(a) A shaft transmits 30 kW at 200 rpm. Diameter 60 mm. Find max torsional shear stress and angle of twist over 2 m. G = 84 GPa.
(b) Differentiate hollow and solid shafts (same torque capacity) — which is more efficient and why?

**Q5. Attempt the following:** *(5+5=10)*
(a) Define fatigue. Explain fatigue testing and the S-N curve. State factors that influence fatigue life.
(b) Write a short note on stress-corrosion cracking (SCC) with an example.

---KEY (Demo 1)---
Q2(i): equal deformation: σs/σc = Es/Ec = 2. σc(Ac+2As) = 25 kN with Ac = 490.9, As = 314.2 mm² → σc = 25000/1119.2 = 22.3 MPa, σs = 44.7 MPa. δ = σcL/Ec = 22.3·1500/1e5 = 0.335 mm (steel gives same: 44.7·1500/2e5 = 0.335 ✓). (verified)
Q2(ii): δ = PL/AE = 128000·2000/(1600·200000) = 0.8 mm; U = P²L/2AE = (128000²·2000)/(2·1600·200000) = 51.2 kN·mm = 51.2 J.
Q3(i): σ_avg = (80−40)/2 = 20; R = √(60²+30²) = √4500 = 67.08 → σ1 = 87.08, σ2 = −47.08 MPa; τmax = 67.08; θp = ½tan⁻¹(2·30/120) = 13.28°; Mohr circle: centre (20,0), radius 67.
Q3(ii): Mmax = wL²/8 = 10·25/8 = 31.25 kNm; I = 150·300³/12 = 3.375×10⁸ mm⁴; σ = M·y/I = 31.25×10⁶·150/3.375×10⁸ = 13.89 MPa; Z = 150·300²/6 = 2.25×10⁶ mm³ (check σ = M/Z = 13.89 ✓).
Q4(a): T = 60P/2πN = 60000·30/(2π·200) = 1432.4 Nm; τ = 16T/πd³ = 16·1432.4×10³/(π·60000) = 33.8 MPa; θ = TL/GJ = 1432.4×10³·2000/(84000·(π·60⁴/32)) = 0.0268 rad = 1.54°. (verified)
Q4(b): Hollow saves material for same J — weight-efficient; for same weight, hollow J much larger.
Q5: standard theory (see 5.2/5.4 notes).

---

# =================== DEMO PAPER 2 ===================

**Q1. Attempt any two:** *(2×5=10)*
(i) Classify lattice imperfections. Explain vacancy & interstitial defects.
(ii) Define creep. Draw the classical creep curve and name its stages.
(i) — third item: Differentiate brittle and ductile fracture.

**Q1(bis) note:** keep numbering clean in exam: (i), (ii), (iii).

**Q2. Attempt any one:** *(10)*
(i) A steel rod 30 mm dia, 4 m long, fixed between rigid supports, temperature rises 60°C. α = 12×10⁻⁶/°C, E = 210 GPa. Find force and stress developed. If supports yield 0.5 mm total, recompute stress.
(ii) At a point, stresses on two mutually perpendicular planes are 60 MPa tensile and 20 MPa compressive with τxy = 25 MPa... find principal stresses and max shear. (Numerical variant of Mohr.)

**Q3. Attempt any one:** *(10)*
(i) A cantilever 2 m long carries 20 kN at free end. Section 100×200 mm. Determine max bending stress & compare if section is rotated (200 wide × 100 deep) — which orientation is better and why?
(ii) Three plates 50 mm × 200 mm form an I-section carrying shear force 14 kN. Determine max shear stress and suggest a rectangular alternative (b = 2/3 depth) with same τmax.

**Q4. Attempt the following:** *(5+5=10)*
(a) Using **Macaulay's method**, find slope & deflection at the free end of a cantilever of length L with UDL w over the entire span (answer in w, L, EI).
(b) A hollow shaft (OD 100, ID 50) transmits power with τmax = 60 MPa at 240 rpm. Find power transmitted.

**Q5. Attempt the following:** *(5+5=10)*
(a) Explain Griffith's theory of brittle fracture. How did Orowan modify it?
(b) Explain strain hardening: dislocation theory and its effect on material behaviour. What is recrystallization annealing?

---KEY (Demo 2)---
Q2(i): free expansion = αΔTL = 12e−6·60·4000 = 2.88 mm fully restrained → σ = EαΔT = 210000·12e−6·60 = 151.2 MPa (compressive), force = σA = 151.2·706.86 = 106.9 kN. With 0.5 mm yielding: net restrained = 2.38 mm → σ = 151.2·(2.38/2.88) = 124.95 MPa.
Q2(ii): σavg = 20, R = √(40²+25²) = 47.17 → 67.17 & −27.17; τmax = 47.17.
Q3(i): M = 20·2 = 40 kNm; upright (100 wide × 200 deep): I = 6.667×10⁷, y = 100 → σ = 60 MPa. Rotated flat (200 wide × 100 deep): I = 1.667×10⁷ but y = 50 → σ = 120 MPa — 2× worse (I drops 4×, y also halves). Depth in the bending plane matters. (verified)
Q3(ii): I-section NA shear via τ = VAȳ/Ib; target rectangle b×d, d = 1.5b, same τmax → solve.
Q4(a): y = −wL⁴/8EI at free end; θ = wL³/6EI.
Q4(b): J = π(100⁴−50⁴)/32 = 9.204×10⁶ mm⁴; T = τJ/r = 60·9.204e6/50 = 11.04 kNm; P = 2πNT/60 = 2π·240·11045/60 = 277.6 kW.
Q5: theory (5.1, 1.4 notes).

---

# =================== DEMO PAPER 3 — PREDICTED DEC-2026 MOCK ===================

**Q1. Attempt any two:** *(2×5=10)*
(i) Explain classification of materials — define ceramics & composites with robotics-relevant applications.
(ii) Write a short note on **stacking faults** (surface defects) and grain boundaries.
(iii) Explain the significance of the **core (kernel) of a section** under eccentric loading.

**Q2. Attempt any one:** *(10)*
(i) Copper + steel composite bar numerical (ND-2025 style — your scanned "Principal Stresses" handout + this pattern): two materials, shared load, equal strains → stresses & extension.
(ii) Thermal stress with yielding supports (Demo 2 type): rod fixed both ends, ΔT given, support yield given.

**Q3. Attempt any one:** *(10)*
(i) **Mohr's circle** — given σx, σy, τxy: principal stresses, directions, max shear, planes; sketch showing plane directions. (The never-missed archetype: asked in ND25, KT25, Dec20, ND21.)
(ii) Bending + eccentric numerical: T-section or rectangle with eccentric load → max/min stress across section (no-tension core check).

**Q4. Attempt the following:** *(5+5=10)*
(a) **Macaulay's method** — SS beam or overhang with point load + UDL; deflection at a point in terms of EI (possibly with "find W" inversion twist like ND25).
(b) Torsion power numerical — solid shaft, P & rpm given, T_max = 1.25·T_mean (Dec-2020 clone), find τ & θ.

**Q5. Attempt the following:** *(5+5=10)*
(a) Fatigue: definition, mechanism, testing, S-N curve, influencing factors (ND25 asked exactly this half).
(b) Creep: definition, curve stages, mechanisms, creep-resistant materials — OR Griffith/Orowan (rotation pair for 5.1/5.3).

---HOW BUILT / SELF-SCORE---
Built on: Q1 = module-1 + corrosion/defects shorts (ND25 trio was composites/corrosion/stacking fault — rotate within same pools); Q2 = composite/thermal bar (asked ND25 + ND21×2); Q3 = Mohr (4/4 papers) + bending/eccentric (3/4 papers); Q4 = Macaulay (4/4) + torsion power (3/4); Q5 = fatigue/S-N (ND25) with creep/Griffith as the pair rotation.
Rubric: full marks only with: labelled diagram (Mohr circle to scale, creep curve axes named), correct formula stated before substitution, units carried. 45+ ready; 38–44 solid; <38 → redo Demo 1–2 dropped items.
