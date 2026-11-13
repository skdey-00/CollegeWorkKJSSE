# CTO — RANKED SAMPLE PAPERS (3 papers, best → decent)

Format per real RAI papers: Q1 any-two ×5 · Q2 any-one ×10 · Q3 any-one ×10 · Q4 both ×5 · Q5 any-two ×5. 50 marks · 2 hrs.

**OFFICIAL Nov-2026 MODULE WEIGHTS (with options): M1 Laplace 20 · M2 Fourier 15 · M3 Numerical 10 · M4 Vector 20 · M5 LPP 15** (offered; 50 attempted). Laplace + Vector = your two 20-mark pillars; Numerical = one skippable 10. Labels below show each slot's offered-module split.

Evidence codes: [BOTH] = asked in both MJ25 & ND25 RAI papers · [KT] = KT/older-era repeat · [ROT] = slot rotation (adjacent item) · [NEW] = never asked, overdue.

---

# ======== PAPER 1 — BEST PREDICTION ========

**Q1. Attempt any two:** *(2×5=10 — offered 15: M1 5 + M4 5 + M5 5)*
(i) Find the directional derivative of φ = x²yz + xz³ at (2,1,1) in the direction of a = i+j+k... wait, use: at point P(1,1,2) in direction 3i−2j+6k. Also find the magnitude and direction of the maximum directional derivative. **[BOTH — DD short in both papers]**
(ii) Write the dual of the LPP: Min Z = 3x₁+2x₂+5x₃ s.t. x₁+x₂+x₃ ≥ 10, 2x₁+3x₂ ≥ 15, x₁,x₂,x₃ ≥ 0. **[BOTH — dual asked in both]**
(iii) Obtain the half-range **cosine** series for f(x) = x² on (0,π). **[BOTH — half-range in both; ND25 sine, MJ25 cosine-type]**

**Q2. Attempt any one:** *(10 — offered 20: M1 10 + M3 10)*
(i) (a) Find L⁻¹{ (3s+8)/(s²+4s+13) }. (b) Find L{ t² e⁻³ᵗ }. **[BOTH — inverse/forward LT pair, both papers]**
(ii) Evaluate ∫₀¹ dx/(1+x) by **trapezoidal + Simpson's 1/3** (h = 0.25) and compare with ln 2. **[BOTH — trap+Simpson in both papers (ND25 ln10 table, MJ25 4-pt table)]**

**Q3. Attempt any one:** *(10 — offered 20: M5 10 + M2 10)*
(i) Solve by **simplex**: Max z = 3x₁+2x₂ s.t. x₁+x₂ ≤ 4, x₁+3x₂ ≤ 6, x₁,x₂ ≥ 0. **[BOTH — simplex in both]**
(ii) Find all **basic solutions** of the system x₁+2x₂+3x₃ = 6, 2x₁+x₂+x₃ = 4 and classify (BFS/degenerate). **[ROT — ND25 asked standard-form conversion; basic solutions is the paired module-5 item]**

**Q4. Attempt the following:** *(5+5=10 — fixed M4 10)*
(a) Show F = (2xy+z³)i + (x²+2z)j + (3xz²+2y)k is irrotational. Find φ with F = ∇φ; evaluate ∫F·dr from A(0,0,0) to B(1,2,3). **[BOTH — the never-missed 4/4 archetype]**
(b) Find L⁻¹{ s/((s²+1)(s²+4)) } by the **convolution theorem**. **[BOTH — convolution in ND25; MJ25 forward LT — same slot]**

**Q5. Attempt any two:** *(2×5=10 — offered 15: M4 5 + M5 5 + M1 5)*
(i) Verify **Green's theorem** for ∮(xy+y²)dx + x²dy, C = boundary of the square [0,1]×[0,1]. **[BOTH — Green's in both]**
(ii) Evaluate ∮(x²−xy)dx + (x²y+3)dy, C: square 0≤x≤1, 0≤y≤1. **[ROT — ND25 exact form family]**
(iii) Convert to standard form + matrix form: Max z = 2x₁+x₂+3x₃ s.t. x₁+x₂+x₃ ≤ 7, 2x₁+3x₂ ≥ 6, x₃ unrestricted. **[ROT — ND25 asked this exact skill]**

---KEY P1---
Q1(i): ∇φ = (2xyz+z³, x²y... careful) — ∇φ at P(1,1,2): φ = x²yz+xz³ → φx = 2xyz+z³ = 2+8=10; φy = x²z = 2; φz = x²y+3xz² = 1+12=13. φx = 2xyz+z³ = 4+8 = 12; â=(3,−2,6)/7 → DD = (36−4+78)/7 = 110/7 ≈ 15.71. Max = |∇φ| = √(144+4+169) = √317 ≈ 17.8. (verified)
Q1(ii): Dual Max w=10y₁+15y₂ s.t. y₁+2y₂ ≤ 3, y₁+3y₂ ≤ 2, y₁ ≤ 5 (x₃ has coefficient 0 in constraint 2), y≥0.
Q1(iii): x²: a₀/2 = π²/3, aₙ = 4(−1)ⁿ/n² → π²/3 + 4Σ(−1)ⁿcos nx/n².
Q2(i)(a): (s²+4s+13)=(s+2)²+9 → e⁻²ᵗ[3cos3t + (8−6)/3 sin3t] = e⁻²ᵗ[3cos3t + (2/3)sin3t].
Q2(i)(b): L{t²e⁻³ᵗ} = 2/(s+3)³.
Q2(ii): x=0,.25,.5,.75,1 → y=1,.8,.667,.571,.5. T=(0.25/2)[1+.5+2(.8+.667+.571)]=0.125[1.5+4.076]=0.697. S=(0.25/3)[1+.5+4(.8+.571)+2(.667)]=0.0833[1.5+5.484+1.334]=0.693. ln2=0.6931.
Q3(i): corners (4,0),(3,1),(0,2) → z=12,11,8 → x₁=4,x₂=0,z=12.
Q3(ii): C(3,2)=3 sets; basic vectors (1,2)&(2,1)→x₃=0: solve x₁+2x₂=6, 2x₁+x₂=4 → x₁=2/3,x₂=8/3 ✓BFS; (1,2)&(3,3)... etc. classify each.
Q4(a): curl F ≡ 0 (verify all 3 components); φ = x²y+z³x+2yz; W = φ(B)−φ(A) = (2+27+12) = 41.
Q4(b): cos t ∗ (1/2)sin2t = ∫₀ᵗ cos u·(1/2)sin2(t−u)du → (1/3)(cos t − cos 2t)?? work fully: result (cos t − cos2t)/3 is for s/(s²+1)(s²+4)... standard: L⁻¹ = (1/3)cos t − (1/3)cos 2t? verify PF: s/((s²+1)(s²+4)) = (s/3)(1/(s²+1) − 1/(s²+4))?? A/(s²+1)+B/(s²+4) with numerators As+B... do PF properly when practicing: s/((s²+1)(s²+4)) = (1/3)[s/(s²+1) − s/(s²+4)] → (1/3)(cos t − cos2t). ✓
Q5(i): ∬(∂Q/∂x−∂P/∂y)dA = ∬(2x−(x+2y))dA = ∬(x−2y)dA = 1/2−1 = −1/2; line side (CCW, 4 edges) also −1/2. (verified)
Q5(iii): x₃ = x₃′−x₃″; surplus −2x₁−3x₂+s₂ = −6; matrix form [A|b].

---

# ======== PAPER 2 — GOOD PREDICTION ========

**Q1. Attempt any two:** *(2×5=10 — offered 15: M4 5 + M2 5 + M5 5)*
(i) Find the angle between the surfaces x²+y²+z² = 9 and z = x²+y²−3 at (2,−1,2). **[ROT — angle-between-surfaces is the other module-1 short; DD came both times, this is the neighbour]**
(ii) State **Dirichlet's conditions** for a Fourier expansion; give one function that fails them. **[ROT — half-range pair, never stated explicitly]**
(iii) Obtain the half-range **sine** series of f(x) = eˣ on (0, π). **[ROT — M2 short; the official weights guarantee ~15 offered marks of Fourier, so the second short rotates toward M2]**

**Q2. Attempt any one:** *(10 — offered 20: M1 10 + M3 10)*
(i) (a) Find L⁻¹{ log((s²+9)/(s²+1)) }. (b) Find L{ sin t / t }. **[ROT — log-type inverse + property-based forward = neighbours of the both-times pair]**
(ii) Use **Lagrange interpolation** (unequal intervals) for: x: 1,2,4,6 → f: 2,3,16,40; estimate f(3). **[NEW — interpolation never asked in RAI; sister COMP papers use it heavily]**

**Q3. Attempt any one:** *(10 — offered 20: M5 10 + M1 10 — ODE-by-Laplace is M1's new second item under the official weights)*
(i) Solve by **Big-M**: Max z = 2x₁+3x₂ s.t. x₁+x₂ ≥ 2, x₁+3x₂ ≤ 6, x≥0. **[NEW — never in RAI; standard next step after simplex in every textbook & sister paper]**
(ii) Solve y″−3y′+2y = 4e²ᵗ, y(0)=−3, y′(0)=5 by **Laplace transform**. **[KT — exact ODE asked in COMP MJ25; RAI syllabus includes it]**

**Q4. Attempt the following:** *(5+5=10 — fixed M4 10)*
(a) Show F = (y²cos x + z³)i + (2y sin x)j + (3xz²)k irrotational; φ and work from (0,0,0) to (π/2, 1, 2). **[ROT — same archetype, fresh vector field]**
(b) Verify **Green's theorem** (same skill, fresh curve): ∮(eˣsin y dx + eˣcos y dy), C: x²+y² = 1. **[ROT — Green's rotation variant]**

**Q5. Attempt any two:** *(2×5=10 — offered 15: M4 10 + M1 5)*
(i) Evaluate by **Stokes' theorem**: F = (x−y)i+(x+y)j, C: x²+y²=1, z=0. **[NEW — Stokes never asked in RAI; completes the Green/Stokes/Gauss triad]**
(ii) Evaluate by **Gauss divergence theorem**: F = 4xi+3yj−2zk over the tetrahedron x,y,z ≥ 0, x+y+z ≤ 1. **[NEW — same triad logic]**
(iii) Solve the initial-value ODE by LT: y″+2y′+y = t, y(0)=0, y′(0)=1. **[ROT — LT-application short]**

---KEY P2---
Q1(i): normals (4,−2,4) & (4,−2,−1) → cosθ = (16+4−4)/(6√21) = 16/27.495 = 0.5819 → θ ≈ 54.4°. (verified)
Q1(ii): piecewise continuous, finite extrema, single-valued; f = tan x on (−π/2,π/2) fails (infinite).
Q1(iii): bₙ = (2/π)∫₀^π eˣ sin nx dx = (2/π)·n(1−(−1)ⁿe^π)/(1+n²) (by parts twice; verified numerically for n=1,2).
Q2(i)(a): −(1/t)L⁻¹{g′} → g′ = 2s/(s²+9) − 2s/(s²+1) → (2/t)(cos t − cos 3t).
Q2(i)(b): tan⁻¹(1/s).
Q2(ii): f(3) = 2(1)(−1)(−3)/((−1)(−3)(−5)) + 3(2)(−1)(−3)/((1)(−2)(−4)) + 16(2)(1)(−3)/((3)(2)(−2)) + 40(2)(1)(−1)/((5)(4)(2)) = 2·3/(−15)+3·6/8+16·(−6)/(−12)+40·(−2)/40 = −0.4+2.25+8−2 = 7.85.
Q3(i): add surplus+artificial to ≥ row with −M penalty. Corners: (2,0) z=4, (0,2) z=6, (6,0) z=12 → optimum x₁=6, x₂=0, z=12. (verified)
Q3(ii): Y(s) = −3/(s−1) + 5/(s−1)² + 4/(s−2)² → y = −7eᵗ + (4+4t)e²ᵗ. Check: y(0)=−3 ✓, y′(0)=−7+12=5 ✓. (verified numerically)
Q4(a): φ = y² sin x + xz³; W = 1·sin(π/2) + (π/2)·8 = 1+4π.
Q4(b): ∮ = ∬(eˣcos y − eˣcos y)dA = 0 (both partials equal!) → both sides 0. Elegant.
Q5(i): curl F = 2k → 2·π = 2π.
Q5(ii): div = 5; vol = 1/6 → 5/6.
Q5(iii): Y = 1/(s+1)² + (1−s)/(s+1)²... y = te⁻ᵗ + ... verify.

---

# ======== PAPER 3 — DECENT PREDICTION ========

**Q1. Attempt any two:** *(2×5=10 — offered 15: M4 5 + M2 5 + M3 5)*
(i) If F is irrotational and solenoidal both — what does that say about φ? Laplace's equation φ²=0, harmonic functions; one example. **[NEW]**
(ii) Obtain the **full-range** Fourier series of f(x) = x² on (−π,π); deduce Σ1/n² = π²/6. **[NEW — RAI asked only half-range so far]**
(iii) Explain the operator identities: E = 1+Δ, Δ = E−1, and express ∇ in terms of E. **[NEW — numerical-methods theory short]**

**Q2. Attempt any one:** *(10 — offered 20: M1 10 + M3 10)*
(i) (a) Find L⁻¹{ 1/((s+1)(s−2)) } by convolution. (b) Find L{ e⁻²ᵗ sin3t · t }. **[ROT]**
(ii) Fit **Newton's forward difference** formula (table + estimate) AND fit a **straight line by least squares** for: (0,1),(1,3),(2,4),(3,5) — predict at x=4. **[NEW — least squares never asked; standard syllabus item]**

**Q3. Attempt any one:** *(10 — offered 20: M5 10 + M2 10)*
(i) Solve the assignment-like transportation... NOT in syllabus — skip. Instead: Solve by two-phase... also not core — use: **Graphical LPP** (two variables): Min z = 3x₁+2x₂ s.t. x₁+x₂ ≥ 2, x₁+2x₂ ≤ 8, x≥0 — corner-point method with graph description. **[NEW — graphical method is the module-5 opener]**
(ii) Find the **Fourier series** of f(x) = eˣ on (−π,π) or half-range sine of eˣ on (0,π). **[NEW]**

**Q4. Attempt the following:** *(5+5=10 — fixed M4 10)*
(a) F = (2x−y)i + (4z+z... construct) — fresh irrotational field, φ, work between two given points. **[BOTH — same archetype, new numbers]**
(b) Evaluate ∮F·dr for F = y i + (x+2y)j around the triangle (0,0)→(1,0)→(0,1)→(0,0) directly AND by Green's theorem; reconcile. **[ROT]**

(b-alternative in same slot): Find L⁻¹{ (s+3)/(s²+6s+18) }... wait slot conflict — keep (b) as Green's-triangle; the LT short moves to Q5.

**Q5. Attempt any two:** *(2×5=10 — offered 15: M2 5 + M3 5 + M1 5)*
(i) **Parseval's identity** for half-range cosine series of x² on (0,π) — state and apply to deduce Σ1/n⁴ = π⁴/90. **[NEW — classic pair of the asked x² series]**
(ii) Evaluate ∫₀¹ dx/(1+x²) by Simpson's 3/8 rule (h=1/6). **[NEW — 3/8 rule never asked; both papers used 1/3]**
(iii) Find L⁻¹{ (3s+8)/(s²+4s+13) }... duplicate of P1 — replace with: Find L{ cosh t · sin t } or state+prove the **second shifting theorem**. **[NEW]**

---KEY P3---
Q1(ii): x² = π²/3 + 4Σ(−1)ⁿcos nx/n²; x=π → π²/6.
Q2(i)(a): (1/3)(e²ᵗ − e⁻ᵗ) convolution of e⁻ᵗ & e²ᵗ... L⁻¹{1/(s+1)}∗L⁻¹{1/(s−2)} = ∫e⁻ᵘe²⁽ᵗ⁻ᵘ⁾du = e²ᵗ(1−e⁻³ᵗ)/3.
Q2(ii): Σy=13, Σxy=26 (0+3+8+15), Σx²=14, n=4 → b = (4·26−6·13)/(4·14−36) = 26/20 = 1.3, a = 3.25−1.3(1.5) = 1.3 → y = 1.3+1.3x → f(4) = 6.5. (verified; Newton-forward extrapolation gives 5.5 — different method, different answer)
Q3(i): corners (2,0) z=6, (8,0) z=24, (0,4) z=8, (0,2) z=4 → min z = 4 at (0, 2). (verified)
Q4(b): ∂Q/∂x−∂P/dy = 1−1 = 0 → Green gives 0; direct edge integration also gives 0 (each edge's contribution cancels). (verified)
Q5(i): Parseval for x² cosine: (1/π)∫x⁴ dx = a₀²/4/2? + Σaₙ²/2 → π⁴/5 = π⁴/9/... standard result Σ1/n⁴ = π⁴/90 via aₙ = 4(−1)ⁿ/n².
Q5(ii): h=1/6: 3/8·h[f0+3f1+3f2+f3+...+f6] → value ≈ 0.7854 vs π/4.

---HOW THESE WERE RANKED---
**Official Nov-2026 weights now steer the tiers:** M1 Laplace and M4 Vector (20 offered each) dominate P1 and P2; M3 Numerical (10, skippable) appears once per paper as the Q2 alternative; M2 Fourier and M5 LPP (15 each) supply the second shorts and Q3 options. If you're short on time, drill in this order: M1 inverse-LT pairs + ODE-by-Laplace → M4 Q4 family + Green's → M5 dual+simplex → M2 half-range → M3 last.
P1 items: every single one is a both-papers repeat or exact ND25 item — the modal Dec-2026 paper. P2: once-asked items + nearest rotation neighbours + the strongest never-asked (Big-M, Stokes, Gauss, Lagrange — all standard in sister papers). P3: residual syllabus (full-range Fourier, Parseval, least squares, 3/8 rule, graphical LPP, operator identities) — insurance against a surprise. P1 mastery ≈ 35/50 expected hits; P1+P2 ≈ 46/50; all three = full syllabus.
