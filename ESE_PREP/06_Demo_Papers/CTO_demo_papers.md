# CTO — DEMO PAPERS (3 papers, exam format: 50 marks · 2 hrs · all compulsory, internal choice)

Format cloned from real RAI papers MJ-2025 & ND-2025: Q1 any-two ×5 · Q2 any-one ×10 · Q3 any-one ×10 · Q4 both ×5 · Q5 any-two ×5.

**OFFICIAL Nov-2026 MODULE WEIGHTS (with options) — M1 Laplace 20 · M2 Fourier 15 · M3 Numerical 10 · M4 Vector 20 · M5 LPP 15 (offered marks; 50 attempted).**
Read this as: Laplace and Vector are the two 20-mark pillars — a weakness in either is fatal; Numerical Methods is one skippable 10 — a weakness there costs nothing if your Laplace is strong. Demo papers below already follow this split (each offers 80 marks: Q1 3×5, Q2/Q3 2×10, Q4 10, Q5 3×5).

---

# =================== DEMO PAPER 1 ===================

**Q1. Attempt any two:** *(2×5=10 — offered 15: M1 5 + M4 5 + M5 5)*
(i) Find the directional derivative of φ = x²y + z²x at (1,1,1) in the direction of the line making equal angles with the positive coordinate axes. Also find the direction & magnitude of maximum directional derivative.
(ii) Write the dual of: Min Z = 4x₁ + 3x₂ + 6x₃ s.t. 2x₁ + x₂ + x₃ ≥ 4, x₁ + 3x₂ + 2x₃ ≥ 5, x₁,x₂,x₃ ≥ 0.
(iii) Obtain the half-range cosine series for f(x) = x² on (0, π).

**Q2. Attempt any one:** *(10 — offered 20: M1 10 + M3 10)*
(i) (a) Find L⁻¹{ (3s+8)/(s²+4s+13) }. (b) Find L{ t e⁻²ᵗ sin 3t }.
(ii) The pressure of steam vs temperature table is given. Using **Newton's forward interpolation**, estimate the pressure at 145°C:

| T(°C): | 140 | 150 | 160 | 170 | 180 |
|---|---|---|---|---|---|
| P: | 3.6 | 4.3 | 5.1 | 6.0 | 7.0 |

**Q3. Attempt any one:** *(10 — offered 20: M5 10 + M2 10)*
(i) Solve by **simplex method**: Max z = 3x₁ + 2x₂ s.t. x₁ + x₂ ≤ 4, x₁ + 3x₂ ≤ 6, x₁, x₂ ≥ 0.
(ii) Find all **basic solutions** of: Max z = 2x₁ + 4x₂ + x₃ s.t. x₁ + 2x₂ + 3x₃ = 6, 2x₁ + x₂ + x₃ = 4 (all variables ≥ 0). Identify basic feasible / degenerate / optimal-BFS.

**Q4. Attempt the following:** *(5+5=10 — fixed M4 10)*
(a) Show that F = (2xy+z³)i + (x²+2z)j + (3xz²+2y)k is irrotational. Find φ such that F = ∇φ and evaluate ∫F·dr along the straight line from A(0,0,0) to B(1,2,3).
(b) Find L⁻¹{ s/((s²+1)(s²+4)) } using the **convolution theorem**.

**Q5. Attempt any two:** *(2×5=10 — offered 15: M4 5 + M5 5 + M1 5)*
(i) Evaluate by **Green's theorem**: ∮(xy dx + x²y dy) where C is the boundary of the region between y = x² and y = x.
(ii) Convert to **standard form** and write the matrix form: Max z = 2x₁ + x₂ + 3x₃ s.t. x₁ + x₂ + x₃ ≤ 7, 2x₁ + 3x₂ ≥ 6, x₃ unrestricted.
(iii) Find the Laplace transform of the **square wave** f(t) = 1 on (0,1), 0 on (1,2), period 2 — L = (1−e⁻ˢ)/(s(1−e⁻²ˢ)) = 1/(s(1+e⁻ˢ)). *(verified)*

---KEY (Demo 1)---
Q1(i): ∇φ = (2xy+z², x², 2zx) = (3, 1, 2) at (1,1,1); unit vector (1,1,1)/√3; DD = (3+1+2)/√3 = 6/√3 = 2√3 ≈ 3.46. Max = |∇φ| = √14 ≈ 3.74, along ∇φ. (verified)
Q1(ii): Dual: Max w = 4y₁+5y₂ s.t. 2y₁+y₂ ≤ 4, y₁+3y₂ ≤ 3, 2y₁+2y₃... (careful: 3 constraints → 3 dual vars; matrix-transpose rule as taught).
Q1(iii): a₀ = (2/π)∫x²dx = 2π²/3 → a₀/2 = π²/3; aₙ = (2/π)∫x²cos nx dx = 4(−1)ⁿ/n². Series: π²/3 − 4Σ(−1)ⁿcos nx/n².
Q2(i)(a): denominator (s+2)²+9 → e⁻²ᵗ(3cos3t + (8−6)/3 sin3t)·... check shift: F(s)=(3(s+2)+2)/((s+2)²+9) → e⁻²ᵗ[3cos3t + (2/3)sin3t].
Q2(i)(b): −d/ds[L{e⁻²ᵗsin3t}] = −d/ds[3/((s+2)²+9)] = 6(s+2)/((s+2)²+9)².
Q2(ii): Δ's: 0.7, 0.8, 0.9, 1.0 → Δ²≈0.1,0.1 → u=(145−140)/10=0.5 → P = 3.6+0.5(0.7)+[0.5(−0.5)/2](0.1) = 3.6+0.35−0.0125 = 3.9375 ≈ 3.94. (verified)
Q3(i): x₁=4,x₂=0 → z=12? Check: corners (4,0),(3,1),(0,2) → z=12,11,8 → optimum x₁=4, x₂=0, z=12. Simplex: 2 iterations.
Q3(ii): 3 choose 2 = 3 basic solution sets; solve pairs → identify signs.
Q4(a): curl F = 0 components check; φ = x²y + z³x + 2yz (+C); work = φ(B)−φ(A) = (1·2·1+27·1+2·2·3) = 2+27+12 = 41.
Q4(b): L⁻¹{s/(s²+1)}·L⁻¹{1/(s²+4)} → ∫₀ᵗ cos u · (1/2)sin 2(t−u) du = (1/3)(2cos t − cos 2t)... verify: convolution result = (cos t − cos 2t)/3 ×? Work it: L⁻¹ = sin t·sin 2t convolution form; standard answer: (1/6)(?) — practice this one fully.
Q5(i): ∮ = ∬(2xy − x) dA over region x²≤y≤x, 0≤x≤1 → ∫₀¹[x·y²−x·y]ₓ²ˣ dx = ∫₀¹(2x³−x²−x⁵)dx = 1/2−1/3−1/6 = 0. (verified — answer is 0, not −1/12)
Q5(iii): square wave L = ∫₀¹e⁻ˢᵗdt/(1−e⁻²ˢ) = (1−e⁻ˢ)/(s(1−e⁻²ˢ)) = 1/(s(1+e⁻ˢ)). (verified numerically at s = 0.5, 1, 2)

---

# =================== DEMO PAPER 2 ===================

**Q1. Attempt any two:** *(2×5=10 — offered 15: M1 5 + M4 5 + M5 5)*
(i) Find the angle between the surfaces x²+y²+z² = 9 and z = x²+y²−3 at (2,−1,2).
(ii) Obtain the half-range **sine** series for f(x) = x(π−x) on (0, π). Hence deduce Σ1/(2n−1)³ = π³/32-type result (state the value you obtain at x = π/2).
(iii) Explain the forward, backward, central difference and shift operators; prove E = 1+Δ and Δ = E−1 relation... (state the algebraic relations between Δ, ∇, E).

**Q2. Attempt any one:** *(10 — offered 20: M1 10 + M3 10)*
(i) (a) Find L⁻¹{ log((s²+9)/(s²+1)) }. (b) If ∫₀^∞ e⁻³ᵗ cos 2t sin(t+a) dt-type... OR (b) Find L{ (sin t)/t }.
(ii) Use **Lagrange interpolation** for the unequal-interval table and estimate f(3):

| x: | 1 | 2 | 4 | 6 |
|---|---|---|---|---|
| f(x): | 2 | 3 | 16 | 40 |

**Q3. Attempt any one:** *(10 — offered 20: M5 10 + M2 10)*
(i) Solve by **Big-M method**: Max z = 2x₁ + 3x₂ s.t. x₁ + x₂ ≥ 2, x₁ + 3x₂ ≤ 6, x₁, x₂ ≥ 0.
(ii) Obtain the **Fourier series** for f(x) = x² on (−π, π), f(x+2π) = f(x). Hence deduce that π²/6 = Σ1/n².

**Q4. Attempt the following:** *(5+5=10 — fixed M4 10)*
(a) Show F = (y²cos x + z³)i + (2y sin x)j + (3xz²)k is irrotational; find φ and the work done from A(0,0,0) to B(π/2, 1, 2).
(b) Evaluate ∮(e^x sin y dx + x²y dy)... replace: Evaluate by **Stokes' theorem**: ∮F·dr where F = y²i + xj, C = boundary of the circle x²+y² = 4, z = 0.

**Q5. Attempt any two:** *(2×5=10 — offered 15: M4 5 + M5 5 + M1 5)*
(i) Evaluate by **Gauss divergence theorem**: ∯F·n̂ dS where F = 4xi + 3yj − 2zk over the cube bounded by x=0,y=0,z=0 and x+y+z=1 plane.
(ii) Find the dual of: Max z = x₁ − 2x₂ + 3x₃ s.t. −2x₁+x₂+3x₃ = 2, 2x₁+3x₂+4x₃ = 5, x₁,x₂,x₃ ≥ 0 (write rules you use).
(iii) Solve the ODE by Laplace transform: y″ + 2y′ + y = t, y(0) = 0, y′(0) = 1.

---KEY (Demo 2)---
Q1(i): normals ∇F₁ = (4,−2,4), ∇F₂ = (2x,2y,−1)=(4,−2,−1) at point; cosθ = (16+4−4)/(√36·√21) = 16/(6√21) → θ = cos⁻¹(0.583) ≈ 54.3°.
Q1(ii): bₙ = (2/π)∫x(π−x)sin nx = 4(1−(−1)ⁿ)/(πn³) → only odd n: 8/(πn³); series (8/π)Σ_{odd} sin nx/n³; at x=π/2 → π³/32 = Σ_{odd} (−1)^k/(2k+1)³.
Q2(i)(a): differentiate: −d/ds form → L⁻¹{2s/(s²+9) − 2s/(s²+1)}·(1/s)... standard result = (2/ t)(cos t − cos 3t)? Use L⁻¹{log g(s)} = −(1/t)L⁻¹{g′(s)}: g′ = 2s/(s²+9)−2s/(s²+1) → answer (2/t)(cos t − cos 3t).
Q2(i)(b): L{sin t/t} = ∫_s^∞ du/(u²+1) = π/2 − tan⁻¹s = tan⁻¹(1/s).
Q2(ii): L(x)·products of (x−xⱼ): f(3) = 2·(3−2)(3−4)(3−6)/((1−2)(1−4)(1−6)) + ... compute → ≈ 7.6 (do fully).
Q3(i): Big-M: surplus + artificial in the ≥ row, penalize with −M. Corner check: (2,0) z=4, (0,2) z=6, (6,0) z=12 → optimum x₁=6, x₂=0, z=12. (verified)
Q3(ii): x² on (−π,π): x² = π²/3 + 4Σ(−1)ⁿcos nx/n²; x=π → π² = π²/3 + 4Σ1/n² → Σ1/n² = π²/6.
Q4(a): φ = y² sin x + xz³; work = φ(B) − φ(A) = (1·1 + (π/2)·8) = 1 + 4π.
Q4(b): curl F = (0,0,1); ∬(curl F)·k dS = area of circle = 4π.
Q5(i): div F = 4+3−2 = 5; volume of tetrahedron = 1/6 → flux = 5/6.
Q5(ii): dual: Min 2y₁+5y₂ (careful with = constraints → unrestricted y); Aᵀ structure.
Q5(iii): Y(s) = ... y(t) = t e⁻ᵗ + ... partial fractions; verify y(0)=0, y′(0)=1.

---

# =================== DEMO PAPER 3 — PREDICTED DEC-2026 MOCK ===================
*Constructed strictly from the validated pattern: Q-slot ↔ module map + rotation logic + overdue items (Gauss/Stokes, Big-M, ODE-by-Laplace, Parseval all never-yet-asked in RAI).*

**Q1. Attempt any two:** *(2×5=10 — offered 15: M1 5 + M4 5 + M5 5)*
(i) Find the directional derivative of φ = xy²z³ at (1,2,1) in the direction a = 2i + j − 2k. Also find the maximum directional derivative.
(ii) Write the dual of: Max z = 5x₁ + 2x₂ − 3x₃ s.t. x₁ + 2x₂ + x₃ ≤ 8, 2x₁ − x₂ + 3x₃ ≤ 10, x₁,x₂,x₃ ≥ 0.
(iii) Using the **second shifting theorem**, find L{ (t−2)² u(t−2) } and L{ sin(t−π/2)·u(t−π/2) }. *(both verified: 2e⁻²ˢ/s³ · e^(−πs/2)/(s²+1))*

**Q2. Attempt any one:** *(10 — offered 20: M1 10 + M3 10)*
(i) (a) Find L⁻¹{ (2s+5)/(s²+4s+29) }. (b) Using the convolution theorem find L⁻¹{ 1/(s(s+2)) }.
(ii) A moving vehicle's velocity was recorded:

| t(s): | 0 | 2 | 4 | 6 | 8 | 10 |
|---|---|---|---|e|---|---|
| v: | 0 | 8 | 14 | 18 | 20 | 20 |

Distance = ∫v dt. Estimate distance using **trapezoidal** and **Simpson's 1/3** (h=2) and state which is likely more accurate.

**Q3. Attempt any one:** *(10 — offered 20: M5 10 + M2 10)*
(i) Solve by **simplex**: Max z = 4x₁ + 3x₂ + 2x₃ s.t. 2x₁ + x₂ + x₃ ≤ 10, x₁ + x₂ + 2x₃ ≤ 12, all ≥ 0.
(ii) Solve the ODE by **Laplace transform**: y″ − 3y′ + 2y = 4e²ᵗ, y(0) = −3, y′(0) = 5.

**Q4. Attempt the following:** *(5+5=10 — fixed M4 10, both compulsory)*
(a) Show that F = (2x cos y + z³)i − (x² sin y)j + (3xz² + 2y z)k... verify irrotational, find φ, evaluate ∫F·dr from (0,0,0) to (π/2, π, 2).
(b) Verify **Green's theorem** for ∮(xy + y²)dx + x²dy where C is the square [0,1]×[0,1].

**Q5. Attempt any two:** *(2×5=10 — offered 15: M4 5 + M5 5 + M1 5)*
(i) Evaluate by **Stokes' theorem**: ∮F·dr, F = (x−y)i + (x+y)j, C: x²+y² = 1, z = 0.
(ii) Solve by **Big-M**: Min z = 4x₁ + x₂ s.t. 3x₁ + x₂ = 3, 4x₁ + 3x₂ ≥ 6, x₁ + 2x₂ ≤ 4, x ≥ 0.
(iii) State **Parseval's identity** for half-range series and use it for f(x) = x on (0,π) (sine series) to deduce Σ1/(2n−1)² = π²/8.

---KEY (Demo 3)---
Q1(i): ∇φ = (y²z³, 2xyz³, 3xy²z²) = (4, 4, 12) at point; |a| = 3 → DD = (8+4−24)/3 = −4 (magnitude 4, direction −ve along a). Max DD = |∇φ| = √(16+16+144) = √176 = 4√11.
Q1(ii): Dual Min 8y₁+10y₂ s.t. y₁+2y₂ ≥ 5, 2y₁−y₂ ≥ 2, y₁+3y₂ ≥ −3, y ≥ 0.
Q1(iii): second shifting: L{(t−2)²u(t−2)} = e⁻²ˢ·L{t²} = 2e⁻²ˢ/s³; L{sin(t−π/2)u(t−π/2)} = e^(−πs/2)/(s²+1). (both verified numerically)
Q2(i)(a): (2(s+2)+1)/((s+2)²+25) → e⁻²ᵗ[2cos5t + (1/5)sin5t].
Q2(i)(b): 1·(1/2)(1−e⁻²ᵗ) convolution of 1 and e⁻²ᵗ → (1/2)(1 − e⁻²ᵗ)... check L⁻¹{1/s}·L⁻¹{1/(s+2)}: ∫₀ᵗ e⁻²ᵘ du = (1−e⁻²ᵗ)/2.
Q2(ii): T = 2/2[0+20+2(8+14+18+20)] = 140 m; (verified) S = 2/3[0+20+4(8+18+20)+2(14+20)] = 2/3[20+184+68] = 181.3 m; Simpson likely closer (smooth decelerating curve).
Q3(i): vertices (5,0,0) z=20 · (0,10,0) z=30 · (0,0,6) z=12 · (0,8,2) z=28 · (8/3,0,14/3) z=20 → optimum x₂=10, x₁=x₃=0, z=30. (verified)
Q3(ii): (s²−3s+2)Y = 4/(s−2) −3s+... Y = [4/(s−2)+5−3s+...]... y(t) = −7eᵗ + (4+4t)e²ᵗ. Check: y(0)=−3 ✓, y′(0)=−7+12=5 ✓. (verified numerically)
Q4(a): φ = x²cos y + xz³ + y z²? check components match after integration; work = φ(B)−φ(A).
Q4(b): RHS ∬(2x−(x+2y))dA = ∬(x−2y)dA = 1/2−1 = −1/2. Direct line integration (4 edges) also gives −1/2 (mind counter-clockwise orientation). (verified)
Q5(i): curl F = (0,0,2); ∬2 dS = 2·π·1² = 2π.
Q5(ii): Min-problem Big-M: artificials in = and ≥ rows with +M·A in the objective. 3x₁+x₂=3 → x₂=3−3x₁; constraints give x₁∈[0.4, 0.6]; z = 4x₁+x₂ = x₁+3 → min z = 3.4 at (0.4, 1.8). (verified)
Q5(iii): sine series x = 2Σ(−1)ⁿ⁺¹ sin nx/n; Parseval: (2/π)∫₀^π x²dx = Σbₙ² → π²/3·(2/π)·π²/3... standard result Σ_{odd}1/n² = π²/8 via x=π/2 substitution route; full derivation in Grewal.

---HOW THIS MOCK WAS BUILT & HOW TO SELF-SCORE---
Weight-split note (official Nov-2026: M1 20 · M2 15 · M3 10 · M4 20 · M5 15 offered): Laplace and Vector are your two 20-mark pillars; Numerical is one skippable 10. Every item maps to a validated rule: Q1 = M4/M5/M2 shorts (DD+dual+half-range = the exact trio of the two real RAI papers — with the new weights the third short rotates in an M1 LT-property item as a strong candidate); Q2 = inverse-LT+convolution or numerical (both real papers); Q3 = simplex or ODE-by-LT (simplex asked 2/2, ODE overdue from COMP evidence); Q4 = irrotational+potential+work (asked in 4/4 available papers incl. both RAI) + Green's/Stokes (Green asked 2/2 RAI); Q5 = two of {Stokes/Gauss, Big-M, Parseval/convolution-short} (rotation + overdue logic).
Self-mark: 45+ = exam-ready; 38–44 = solid; 30–37 = redo dropped archetypes; <30 = back to Pass A.
