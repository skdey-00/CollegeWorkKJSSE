# ANSWER KEY — 02 · Mechanics of Materials

Covers every "possible question" in 02_Mechanics_of_Materials.md. "(verified)" = checked by computation.

---

## MODULE 1 — Materials & Deformation (theory answers)

**1. Classification**: Metals (crystalline, good conductors, ductile — steel/Al); Ceramics (hard, brittle, high temp resistance — alumina, SiC); Polymers (long chains, light, insulators — PMMA, nylon); Composites (two-phase: matrix + reinforcement — CFRP, GFRP). Applications of composites in robotics: robot arm links (high stiffness-to-weight), drone frames, end-effectors/grippers.

**2. Point defects**: Vacancy (missing atom — diffusion, creep); Interstitial (extra atom in gap — lattice strain, hardening); Impurity/substitutional (foreign atom in site — solid solution strengthening). Form by thermal fluctuation; concentration n = N e^(−Q/kT) idea.

**3. Edge vs screw dislocation**: Edge — extra half-plane, Burgers vector ⊥ dislocation line; Screw — lattice spiral, b ∥ line. Slip occurs by dislocation motion (why real strength ≪ theoretical). Frank-Read source: pinned segment bows under stress, pinches off a loop, multiplies dislocations — explains strain hardening.

**4. Surface defects**: Grain boundary (misoriented crystals — blocks dislocations → fine grain = stronger, Hall-Petch); sub-boundary (low angle); stacking fault (interruption of packing sequence ABC|ABAB..., e.g. in FCC — local HCP-like sequence; low energy in FCC, affects work hardening). *(ND25 short note.)*

**5. Single vs polycrystal deformation**: single crystal slips on densest planes along densest directions (FCC {111}⟨110⟩); CRSS: τ_R = σ cosφ cosλ (Schmid factor). Polycrystal: grains constrain each other → finer grain → higher yield.

**6. Strain hardening**: dislocation density ↑ with strain → tangles block motion → σ–ε curve rises; recovered by recrystallization annealing.

**7. Recrystallization annealing**: cold-worked metal heated 0.3–0.5 T_m: recovery (stress relief) → recrystallization (new strain-free grains) → grain growth. Factors: % cold work, temperature, time, purity.

**8. Short notes**: Schottky defect (pair of missing ions in ionic crystal); APF: FCC & HCP 0.74, BCC 0.68, SC 0.52; ductility = % elongation/reduction; endurance limit = stress below which infinite cycles (ferrous ~10⁶ cycles); creep = time-dependent strain under constant stress.

## MODULE 2 — Stress/Strain numericals

**1. Stress-strain diagram (ductile)**: proportional limit → elastic (Hooke σ=Eε) → yield (upper/lower) → strain hardening → UTS → necking → fracture. Label all; draw mild-steel version with distinct yield point.

**2. Elastic constants**: E = 2G(1+μ) = 3K(1−2μ). Derivation of E–G: pure shear τ = σ/2 at 45°; equate shear strain from Mohr geometry γ = τ/G with τ(1+μ)/E from normal strain rotation → G = E/2(1+μ). Given E, G → μ = E/2G − 1; K = E/3(1−2μ).

**3. Hooke's law σ = Eε; FoS = working/stress or ultimate/working; μ = lateral/axial strain (0.25–0.35 metals, 0.5 incompressible).**

**4. Axial numericals**: δ = PL/AE. Strain energy U = P²L/2AE (gradual); sudden load: ×2 stress, ×4 energy (deflection doubles).

**5. Composite bar (copper Ø25 E=100 GPa + steel Ø20 E=200 GPa, 25 kN, 1.5 m)** *(ND25 type)*: equal strain σs/σc = 2; σc = 25000/(490.9+2·314.2) = **22.3 MPa, σs = 44.7 MPa, δ = 0.335 mm** (verified).

**6. Thermal stress**: fully fixed: σ = EαΔT (independent of length!). Steel rod 30 mmØ 4 m, ΔT=60, α=12e−6, E=210 GPa: free expansion = 2.88 mm; σ = **151.2 MPa**; supports yield 0.5 mm → σ = 151.2×2.38/2.88 = **124.9 MPa** (verified). Force = σA.

**7. Principal stresses / inclined planes**: formulas σ′ = (σx+σy)/2 ± R cos2θ..., feeds Mohr (below).

**8. Volumetric strain** e = ε(1−2μ) for axial loading.

**9. Eccentric loading & core**: σ = P/A ± Pe·y/I; no-tension condition e ≤ S/6 (middle third for rectangle; S/4·... middle quarter for circle d/8).

## MODULE 3 — Beams

**1. Max BM formulas**: SS + central W: WL/4; SS + UDL: wL²/8; cantilever + end W: WL; cantilever + UDL: wL²/2. SFD/BMD shapes: SS+UDL → SF linear (±wL/2 to ∓wL/2, zero at mid), BM parabolic (max mid).

**2. Bending stress numerical** *(ND25)*: SS 5 m, UDL 10 kN/m, 150×300: M = 31.25 kN·m; I = 3.375×10⁸ mm⁴; σ_max = M·y/I = 31.25e6×150/3.375e8 = **13.89 MPa**; Z = bh²/6 = 2.25×10⁶ mm³ (σ = M/Z ✓). Safe-load variant: W = σ_allow·Z/L ×4.

**3. Flexure formula derivation**: pure bending assumptions (plane sections remain plane) → strain ∝ y → σ = E y/R → equilibrium: ∫σ dA = 0 → NA through centroid; ∫σ y dA = M → M/I = E/R = σ/y.

**4. Shear stress distribution**: τ = VAȳ/(Ib). Rectangle: parabola, τ_max = 1.5 V/A at NA. Circle: 4/3 V/A. Example 100×200 with V = 14 kN: τ_max = 1.5×14000/20000 = **1.05 MPa**.

**5. I-section**: compute ȳ and I by parallel-axis; τ at flange-web junction jumps because b changes.

**6. Eccentric compressive load on section**: σ_corner = P/A ± Pe·c/I per corner; sign per quadrant.

**7. I computations**: rect bh³/12; circle πd⁴/64; T-section via parallel axis theorem.

## MODULE 4 — Torsion + Macaulay

**1. Torsion numericals**: T = 60P/(2πN) — for P in W. 30 kW, 200 rpm: T = 30000/(2π·200/60) = **1432.4 N·m**. τ = 16T/πd³, d=60: **33.8 MPa**. θ = TL/GJ = 1432.4e3×2000/(84000×1.272e6) = 0.0268 rad = **1.54°** (verified). Hollow 200 OD 25 thick at 200 rpm, 0.5°/2 m: J = π(200⁴−150⁴)/32; solve G or T. T_max = 1.25 T_mean variant (Dec20): T_mean from power then τ check.

**2. Hollow vs solid**: same J → hollow much lighter (material at radius where it works); same weight → hollow J larger. Compare weights: (d_o²+d_i²)/(d²)... standard ratio result ≈ 0.56 for equal strength d_i = d/2? — state qualitative + one quantitative ratio.

**3. GJ = torsional rigidity; Zp = J/r = πd³/16 solid.**

**4. Compound shaft**: equate twist of sections: T·L1/(G1J1) = T·L2/(G2J2) shared torque split by GJ/L; permissible T₀ = min of (τ1·G-condition, τ2-condition).

**5. Pure torsion principal stresses**: σ1,2 = ±τ (Mohr circle centred at origin) — 40 MPa shear → ±40 MPa at 45°.

**6. Macaulay** *(ND25 asked with "find W" twist)*: Steps: reactions; M(x) with (x−a) brackets; integrate twice; boundary conditions; negative-bracket terms = 0. SS + central W: δ_mid = WL³/48EI, θ_ends = WL²/16EI. Cantilever + UDL: δ = wL⁴/8EI, θ = wL³/6EI. "Find W" twist: set given δ_allow = W L³/48EI → W = 48EIδ/L³.

**7. Cantilever end couple M**: θ = ML/EI, δ = ML²/2EI.

## MODULE 5 — Failure theory

**1. Fatigue** *(ND25 exact)*: failure below yield under cyclic loading; stages: crack initiation (surface, stress concentration) → propagation (beach marks) → final fast fracture. Testing: rotating-beam (Wöhler) — specimen loaded in bending while rotating → fully reversed stress; results plotted S vs log N. Steel shows endurance limit (~0.5 UTS); Al does not. Factors: surface finish, size, temperature, stress concentration, residual stress, mean stress.

**2. Creep**: time-dependent inelastic strain at constant stress, high T (>0.4 Tm). Curve: primary (decreasing rate — strain hardening) → secondary (steady minimum rate) → tertiary (accelerating — necking/voids → rupture). Creep-resistant: high melting point, coarse grain, dispersed precipitates (superalloys, Mo alloys).

**3. Griffith**: brittle failure from pre-existing cracks: energy balance — elastic energy release ≥ 2γ_s surface energy → σ_f = √(2Eγ_s/πa) thin plate. Orowan: plastic work at crack tip γ_p ≫ γ_s → σ_f = √(2E(γ_s+γ_p)/πa).

**4. Ductile fracture**: void nucleation-growth-coalescence, cup-cone; notch effect triaxiality; toughness = resistance to crack propagation; ductile-brittle transition (DBTT — ships/liberty ships, low T + high strain rate + notch).

**5. Corrosion** *(ND25 asked types)*: uniform, galvanic, pitting, crevice, intergranular (weld decay), stress-corrosion cracking (SCC — needs susceptible material + specific environment + tensile stress; e.g. brass in ammonia, SS in chlorides). Prevention: coatings, inhibitors, cathodic protection, material selection, stress relief.

**6. Strain hardening / dislocation fracture link**: pile-ups at barriers nucleate cracks (Zener-Stroh).

---

## NUMBER-CHECK TABLE (all verified by code)
composite 22.3/44.7 MPa, δ=0.335 mm · thermal 151.2→124.9 MPa · Mohr 87.08/−47.08/67.08, 13.28° · bending 13.89 MPa, Z 2.25e6 · torsion 1432.4 N·m, 33.8 MPa, 1.54° · hollow power 277.6 kW · cantilever 60→120 MPa (2×) · T-section ȳ=67.8, I=3.14e6, 205/431 MPa · shear 1.05 MPa · strain energy 51.2 J
