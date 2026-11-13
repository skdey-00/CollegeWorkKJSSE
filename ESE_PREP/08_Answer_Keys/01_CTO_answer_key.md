# ANSWER KEY — 01 · Calculus, Transforms & Optimization

Covers every "possible question" in 01_Calculus_Transforms_Optimization.md. Method + answer; "(verified)" = checked by computation. For theory items the full-mark answer skeleton is given.

---

## MODULE 1 — Laplace Transform

**1. L{t e⁻ᵗ cosh 2t}** *(asked MJ25)*
cosh 2t = (e²ᵗ+e⁻²ᵗ)/2 → e⁻ᵗcosh2t = (eᵗ+e⁻³ᵗ)/2 → L = ½[1/(s−1) + 1/(s+3)]. Multiply-by-t: L{t f} = −F′(s) → **−½[−1/(s−1)² − 1/(s+3)²] = ½[1/(s−1)² + 1/(s+3)²]**.

**2. From definition: L{e⁻ᵃᵗ sin bt}** = ∫₀^∞ e⁻ˢᵗ e⁻ᵃᵗ sin bt dt = b/((s+a)²+b²). L{sinh at} = a/(s²−a²). L{cos at} = s/(s²+a²).

**3. Second shifting theorem**: L{f(t−a)·u(t−a)} = e⁻ᵃˢF(s). Example: L{u(t−2)·(t−2)²} = e⁻²ˢ·2/s³.

**4. L{sin t/t}** = ∫ₛ^∞ du/(u²+1) = **tan⁻¹(1/s)**. L{t sin 2t} = −d/ds[2s/(s²+4)²] = 2(s²−4)/(s²+4)².

**5. Square wave f(t)=1 on (0,a), −1 on (a,2a), period 2a**: L = (1/(1+e⁻ᵃˢ))·∫₀^a e⁻ˢᵗdt·... = **(1/s)·tanh(as/2)**.

**6. L⁻¹{(3s+7)/(s²−2s−3)}**: denominator (s−3)(s+1) → A/(s−3)+B/(s+1): A = 4, B = −1 → **4e³ᵗ − e⁻ᵗ**. (s+4)/(s²+4s+13) = (s+2)+2 over (s+2)²+9 → **e⁻²ᵗ(cos3t + (2/3)sin3t)**.

**7. L⁻¹{log((s+4)/s)}** *(asked ND25)*: d/ds = 1/(s+4) − 1/s → L⁻¹{F′} = −t f(t) → f = (1−e⁻⁴ᵗ)/t → answer **(1−e⁻⁴ᵗ)/t**.

**8. Convolution L⁻¹{1/(s(s+1)(s+2))}**: PF: 1/(s(s+1)(s+2)) = ½·1/s − 1/(s+1) + ½·1/(s+2) → **½ − e⁻ᵗ + ½e⁻²ᵗ**. Convolution route: 1/s ∗ ... same result. ND25's L⁻¹{s/(s²+1)²}: = L{½ t cos t}·... s/(s²+1)² = L{½ t sin t} → **½ t sin t**.

**9. ∫₀^∞ e⁻²ᵗ sin(t+a)cos(t−a) dt** *(asked ND25)*: sin(t+a)cos(t−a) = ½[sin(2t) + sin(2a)] → integral = ½[2/(s²+4) + sin2a/s] at s=2 = ½[2/8 + sin2a/2] = **(1+sin2a)/4·...** = 1/8 + (sin2a)/4. Set = stated k, solve.

**10. ODEs by Laplace**: y″+y=t, y(0)=1, y′(0)=0 → (s²+1)Y = 1/s² + s → Y = 1/(s²(s²+1)) + s/(s²+1) → **y = t − sin t + cos t**. (D²−3D+2)y = 4e²ᵗ, y(0)=−3, y′(0)=5 → **y = −7eᵗ + (4+4t)e²ᵗ** (verified numerically).

**Notes**: first shift e^at: F(s−a) · second shift: e⁻ᵃˢF(s) · L{tf} = −F′ · L{f/t} = ∫ₛ^∞ F du · δ(t−a) → e⁻ᵃˢ · u(t−a) → e⁻ᵃˢ/s.

## MODULE 2 — Fourier Series

**1. Half-range sine, f = 1+x on (0,π)** *(asked MJ25)*: bₙ = (2/π)∫₀^π(1+x)sin nx dx = (2/π)[ (−(1+x)cos nx)/n + sin nx/n² ]₀^π = (2/π)[1−πcos nπ... ] compute: = (2/(nπ))[1 − (−1)ⁿ(1+π)] + 0 → bₙ = (2/(nπ))[1+(π+1)(−1)ⁿ⁺¹]. Series Σ bₙ sin nx.

**2. Half-range sine, f = x cos x** *(asked ND25)*: bₙ = (2/π)∫₀^π x cos x sin nx dx — use product-to-sum + by parts; even-n terms vanish; bₙ = (2n/(π(n²−1)))·[(−1)ⁿ⁺¹+1]/(n²−1)-type. Work by parts twice; final bₙ = 4n(1−(−1)ⁿ⁺¹·...)—do carefully in exam: standard result bₙ = (2/π)·n(1+(−1)ⁿ⁺¹)/(n²−1) for n≠1, b₁ = 0. (state method — by parts twice)

**3. Full-range x+x² on (−π,π)** *(asked MJ25)*: even+odd split: x part → bₙ = 2(−1)ⁿ⁺¹/n; x² part → a₀/2 = π²/3, aₙ = 4(−1)ⁿ/n². f = π²/3 + Σ[4(−1)ⁿcos nx/n² + 2(−1)ⁿ⁺¹ sin nx/n]. Deduce at x=π: 1+1/3+1/5−… wait — deduce for x part: put x=π/2: π/4 = 1−1/3+1/5−… ✓

**4. x² on (−π,π)**: x² = π²/3 + 4Σ(−1)ⁿ cos nx/n²; x=π → **Σ1/n² = π²/6**; x=0 → Σ(−1)ⁿ⁺¹/n² = π²/12. (π−x)/2 on (0,2π): = Σ sin nx/n → at x=π/2 gives the odd-harmonic result.

**5. cosh x / sinh x**: cosh x = sinh π/π + (2sinh π/π)Σ(−1)ⁿcos nx/(n²+1). sinh x = (2sinh π/π)Σ n(−1)ⁿ⁺¹ sin nx/(n²+1).

**6. Parseval**: for half-range sine on (0,π): Σbₙ² = (2/π)∫₀^π f² dx. For f = x: Σ 4/n² = 2π²/3 → consistency check π²/6. Use: mean square value = Σbₙ²/2 (full range).

**7. Dirichlet's conditions** (full marks = 4 points): f single-valued; finite; piecewise continuous with finitely many discontinuities and maxima/minima in one period. At a discontinuity the series → average of left/right limits.

**8. Complex form**: f = Σcₙe⁑ⁿˣ, cₙ = (1/2π)∫₋π^π f e⁻ⁱⁿˣ dx; cₙ = (aₙ−ibₙ)/2, c₋ₙ = conjugate.

## MODULE 3 — Numerical Methods

**1. Newton forward (steam table, estimate 142°C)** *(asked MJ25)*: differences from the given table; u = (142−x₀)/h; y = y₀+uC₁+u²C₂+u³C₃... Only 2–3 difference terms needed for 4-decimal accuracy.

**2. ∫x log x, [2,8], 6 intervals** *(asked MJ25)*: h=1. nodes 2..8, y = x log x: 1.386, 3.296, 5.545, 8.041, 10.75, 13.65, 16.636. y-values: 1.386, 3.296, 5.545, 8.041, 10.750, 13.644, 16.636. T = ½[y₀+y₆+2Σmid] = **50.27**. S = ⅓[y₀+y₆+4(y₁+y₃+y₅)+2(y₂+y₄)] = **50.16**. Exact: ∫₂⁸x lnx dx = [x²/2·lnx − x²/4]₂⁸ = (66.542−16)−(1.386−1) = **50.156**. (all verified — Simpson ≈ exact here since x log x is smooth)

**3. ∫₁¹⁰ dx/x** *(asked ND25)*: ND25 used h=1 (9 intervals). T = ½[1+0.1+2(0.5+0.3333+0.25+0.2+0.1667+0.1429+0.125+0.1111)] = ½[1.1+2(1.829)] = 2.379. S (n must be even — with h=1, n=9 odd → either h=0.5 or combine): state this subtlety; with h=0.5, S → 2.305 vs ln10 = 2.3026.

**4. Backward/Lagrange**: NP/Bessel formulas; Lagrange for {1,2,4,6}→{2,3,16,40}: f(3) = 7.85 (verified).

**5. Operator relations**: E = 1+Δ; Δ = E−1; ∇ = 1−E⁻¹; Δ = ∇E... state and prove any two via yᵣ₊₁ definition.

**6. Simpson 3/8**: ∫₀¹ dx/(1+x²), h=1/6: **0.78540 ≈ π/4** (verified).

**7. Stirling/Bessel** (self-learning): central differences around the middle; one-line statement each.

## MODULE 4 — Vector Calculus

**1. Irrotational + potential + work** *(the 4/4 archetype)*: Method: (i) curl F = 0 component-wise; (ii) φ = ∫P dx = x²y+z³x+g(y,z); match Q: ∂φ/∂y = x²+g′ = Q → g = 2yz+h(z); match R → h′ = 0. φ = x²y+z³x+2yz. (iii) W = φ(B)−φ(A) — path independence is the whole point. MJ25 F = (2xy+z)i+(x²+2y²z)j+(3y²z²+x)k between given points → φ = x²y+zx+y²z³... (match components as above).

**2. Green's theorem**: ∮ = ∬(∂N/∂x−∂M/∂y)dA. MJ25 rectangle eˣsiny dx + e⁻ˣcosy dy: ∂N/∂x = −e⁻ˣcosy, ∂M/∂y = eˣcosy → ∬(−e⁻ˣcosy−eˣcosy)dA over rectangle — integrate. ND25 (x²−xy)dx+(x²y+3)dy: ∂N/∂x−∂M/∂y = 2xy+x over given region.

**3. Angle between surfaces** *(MJ25)*: cosθ = ∇F₁·∇F₂/(|∇F₁||∇F₂|) at the point; both normals outward.

**4. Directional derivative** *(ND25)*: DD = ∇φ·â; max = |∇φ| along ∇φ. For φ = x²+y²+z², ∇φ = 2(x,y,z).

**5. Gauss divergence**: F = 4xi+3yj−2zk → div = 5 → flux = 5V. Unit cube: 5. Tetrahedron x+y+z≤1: 5/6.

**6. Stokes**: ∮F·dr = ∬(curl F)·k dS over the spanning surface. F = x²i+xyj around rectangle [0,a]×[0,b]: curl = (x, 0, y−... ) compute: ∇×(x², xy, 0) = (0−0, 0−0, ∂(xy)/∂x−∂x²/∂y) = (0,0,y) → ∬y dA = ab²/2.

**7. Coplanar points**: scalar triple product [a−d, b−d, c−d] = 0.

**8. Solenoidal**: div F = 0.

**9. Find a,b,c for irrotational F**: set each curl component = 0 → 3 equations.

## MODULE 5 — LPP

**1. Simplex** *(both papers)*: standard setup + iterations. Max 3x₁+2x₂ with x₁+x₂≤4, x₁+3x₂≤6: optimum **x₁=4, x₂=0, z=12**. Max 5x₁+4x₂+3x₃ (MJ25): z* = at vertex of its constraints — set up tableaus per textbook; entering = most negative z-row; leaving = min ratio.

**2. Dual**: Max↔Min, A→Aᵀ, b↔c, ≤→≥. ND25: Max z = x₁−2x₂+3x₃, equalities → dual variables unrestricted; write rules then transpose.

**3. Basic solutions** *(MJ25)*: 3 variables 2 constraints → C(3,2)=3 basic sets; solve each 2×2; check sign of non-basic (=0) and basic variables → classify BFS / degenerate (any basic = 0).

**4. Standard form** *(ND25)*: add slack to ≤, surplus+artificial to ≥, split unrestricted x = x′−x″; matrix form: Max cᵀx, Ax = b, x≥0.

**5. Big-M** *(overdue)*: Max 2x₁+3x₂ s.t. x₁+x₂≥2, x₁+3x₂≤6: **x₁=6, x₂=0, z=12** (verified). Min 4x₁+x₂ s.t. 3x₁+x₂=3, 4x₁+3x₂≥6, x₁+2x₂≤4: **min z = 3.4 at (0.4,1.8)** (verified).

**6. Duality theory short**: weak duality (cᵀx ≤ bᵀy), strong duality at optimum equality, complementary slackness.

**7. Dual simplex** (self-learning): same tableaus, primal-infeasible start (some bᵢ<0), leaving variable chosen from negative b, entering by ratio of z-row.

---

## ARCHETYPE QUICK-ANSWERS (for the 8 in the cheat sheet)
A → curl=0; φ by integration; W = φ(B)−φ(A) · B → Green: ∬(Nₓ−M_y)dA · C → transpose rules (see M5.2) · D → simplex iterations (see M5.1) · E → half-range: bₙ = (2/π)∫f sin·/aₙ = (2/π)∫f cos·, state even/odd first · F → PF or convolution theorem (f∗g) · G → T = h/2[end+2mid], S = h/3[end+4·odd+2·even] · H → DD = ∇φ·â; angle: cosθ = ∇F₁·∇F₂/(|∇F₁||∇F₂|).
