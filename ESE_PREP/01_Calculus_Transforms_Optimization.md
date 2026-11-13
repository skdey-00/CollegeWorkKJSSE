# 01 · Calculus, Transforms and Optimization (316U43C301) — ESE Question Bank

50 marks · 2 hrs · Pattern: Q1 any-two ×5 · Q2 any-one ×10 · Q3 any-one ×10 · Q4 both ×5 · Q5 any-two/both ×5

## OFFICIAL MODULE WEIGHTS (Nov-2026, received 11 Nov — supersedes the even-spread assumption)

Offered marks per module (paper offers 80, you attempt 50):

| Module | Offered | How it appears in the Q-frame (reconciled with MJ25/ND25 papers) | Your attack order |
|---|---|---|---|
| M1 Laplace | **20** | Q1 5-mark short (forward/inverse LT property) + a 10-mark Q2 option (inverse-LT pair, or ODE-by-Laplace) + often a 5-mark Q5 convolution/short | **#1 — joint-heaviest. Drilled formulas = near-full marks.** |
| M2 Fourier | 15 | Q1 half-range 5-mark short + a 10-mark Q3 option (full-range + deduce) | #3 |
| M3 Numerical | 10 | ONE 10-mark Q2 option only (interpolation OR trap+Simpson) | **#5 — skippable. One method of each; no more.** |
| M4 Vector Calc | **20** | Q4 fixed (a)+(b) = 10 (irrotational family) + Green's/Stokes/Gauss 5-mark Q5 + DD/angle 5-mark Q1 short | **#2 — joint-heaviest, most predictable.** |
| M5 LPP | 15 | Dual 5-mark Q1 short + a 10-mark Q3 option (simplex) + 5-mark Q5 option (standard form / basic solutions) | #4 |

What changed vs the two real papers: they offered M1 15 / M5 20; the official table flips 5 marks from LPP into Laplace. Practical effect: a **second Laplace item** (most likely an ODE-solve-by-Laplace — in the syllabus, asked by COMP twice, never yet by RAI) now outranks one LPP short. M3 is confirmed thin: offered only through a single skippable 10 — learn ONE interpolation method + ONE integration pair, skip the rest.

---

## CHEAT SHEET — the 8 recurring archetypes

| # | Archetype | Seen in | Frequency |
|---|-----------|---------|-----------|
| A | **Irrotational vector + scalar potential φ + line integral work/flux** | MJ25 (F=(2xy+z)i+(x²+2y²z)j+(3y²z²+x)k), ND25 (F=(ye^x cosz)i+(xe^x sinz)k variant) | 2/2 RAI papers + 2 COMP papers |
| B | **Green's theorem** evaluate ∮(M dx + N dy) over given curve C | MJ25 (e^x siny dx + e^−x cosy dy, rectangle), ND25 ((x²−xy)dx+(x²y+3)dy) | 2/2 RAI |
| C | **Dual of an LPP** | MJ25 (Min Z=5x₁+2x₂−7x₃...), ND25 (Max Z=x₁−2x₂+3x₃...) | 2/2 RAI |
| D | **Simplex method** solve LPP | MJ25 (Max z=5x₁+4x₂+3x₃), ND25 (Max z=6x₁−2x₂+3x₃) | 2/2 RAI |
| E | **Half-range Fourier sine/cosine series** | MJ25: f(x)=1+x on (0,π); ND25: f(x)=x cos x on (0,π) | 2/2 RAI |
| F | **Inverse Laplace via partial fractions / convolution** | MJ25 (te^−t cosh t type), ND25 (log((s+4)/s), convolution of sin) | 2/2 RAI |
| G | **Trapezoidal + Simpson's rules** (same table both rules, compare) | MJ25 (∫x·logx dx, [2,8]/6 parts), ND25 (∫dx/x = ln10, h=1) | 2/2 RAI |
| H | **Angle between surfaces / directional derivative** | MJ25 (angle between x²+y²+z²=12 & plane; ND25 (dir. deriv. of x²+y²+z² along line) | 2/2 RAI |

Everything else that appeared once: full-range Fourier with deduce-series (MJ25, also COMP twice), basic solutions of LPP (MJ25), standard form conversion + matrix form (ND25), Laplace of t e^−t cosh t (MJ25), ∫₀^∞ e^−2t sin(t+a)cos(t−a) dt (ND25).

**Reading the pattern:** Q1 always ≈ {vector-numerical, dual, half-range Fourier}. Q2 ≈ {inverse Laplace + small (b) part, interpolation/Trapezoidal}. Q3 ≈ {simplex, basic solutions, full Fourier}. Q4 = irrotational/potential/work — **essentially fixed**. Q5 ≈ {Green's theorem, standard form, convolution}.

---

## MODULE 1 — Laplace Transform

### Possible questions
1. Find L{t e^−t cosh 2t} (first shift + multiplication by t). *(asked MJ25)*
2. Find L{e^−at sin bt}, L{sinh at}, L{cos at} from definition.
3. State and use the second shifting theorem (unit step) — evaluate expressions with H(t−a).
4. Find L{ sin t / t } (division by t), L{ t sin 2t }.
5. Find L of a periodic function (square wave / sawtooth).
6. Find L⁻¹ using partial fractions: e.g. of (3s+7)/(s²−2s−3), (s+4)/(s²+4s+13)-type.
7. Find L⁻¹{ log((s+4)/s) } — differentiate first, then invert. *(asked ND25)*
8. **Convolution theorem**: find L⁻¹ of 1/(s(s+1)(s+2)) or L⁻¹{ sin t · sin 2t products } — *(asked ND25: L⁻¹{ (s/(s²+1)²) } via convolution; COMP MJ25 asked similar)*
9. If ∫₀^∞ e^−2t sin(t+a) cos(t−a) dt = k, find a. *(asked ND25 — recognize Laplace integral)*
10. Solve ODE by Laplace: y″+y=t with y(0)=1, y′(0)=0 *(COMP ND25)*; (D²−3D+2)y=4e²t with y(0)=−3, y′(0)=5 *(COMP MJ25)*. RAI hasn't asked it yet but it's unit 1.4 and both COMP papers did → **high probability it appears as Q2/Q5 option**.

### Notes to remember
- First shifting: L{e^at f(t)} = F(s−a). Second shifting: L{f(t−a)·u(t−a)} = e^−as F(s).
- L{t f(t)} = −F′(s); L{f(t)/t} = ∫_s^∞ F(u)du — this is how the log question works: L⁻¹{log((s+4)/s)} = ∫... = (1−e^−4t)/t.
- Convolution: (f*g)(t)=∫₀^t f(u)g(t−u)du, L⁻¹{F(s)G(s)} = f*g.
- For ODEs: transform → algebraic equation in Y(s) → partial fractions → invert. Initial conditions get substituted at the algebraic stage.
- Dirac delta: L{δ(t−a)} = e^−as; unit step L{u(t−a)} = e^−as/s (self-learning but COMP asked it twice).

## MODULE 2 — Fourier Series

### Possible questions
1. Half-range sine series of f(x)=1+x on (0,π). *(asked MJ25)*
2. Half-range sine series of f(x)=x cos x on (0,π). *(asked ND25)*
3. Full-range expansion of f(x)=x+x² on (−π,π), deduce 1−1/3+1/5−… = π/4-type results. *(asked MJ25 & both COMP papers — deduce-series is a favourite)*
4. f(x)=x² on (−π,π) → deduce π²/6 series; f(x)=(π−x)²/4 or cosh/sinh variants (COMP asked f(θ)=(π−θ)/2 → deduce odd harmonic series).
5. Even/odd function expansions: cosh x, sinh x on (−π,π) (COMP MJ25 complex-form variant).
6. Parseval's identity — compute mean square value / deduce series value (syllabus explicitly lists it; not yet asked → **possible Q1 short**).
7. Dirichlet's conditions statement (2–3 marks theory).
8. Complex form (self-learning; COMP asked twice — know the cₙ = (1/2π)∫f e^−inx dx form).

### Notes to remember
- Even function → only aₙ (cosine) terms; odd → only bₙ. Half-range on (0,π): sine series bₙ=(2/π)∫₀^π f sin nx dx; cosine aₙ=(2/π)∫₀^π f cos nx dx.
- x cos x: integration by parts twice.
- "Hence deduce" marks: substitute a specific x (usually x=π/2 or x=π) into your series.
- Parseval: a₀²/2 + Σ(aₙ²+bₙ²) = (2/π)∫f² dx (check your textbook's exact constant for the interval).

## MODULE 3 — Numerical Methods

### Possible questions
1. **Newton's forward interpolation** from a steam pressure-vs-temperature table → estimate at 142°C. *(asked MJ25)*
2. Trapezoidal vs Simpson's 1/3 for ∫x log x dx over [2,8], 6 subintervals. *(asked MJ25)*
3. Trapezoidal + Simpson's for ∫₁¹⁰ dx/x → estimate ln 10 both ways. *(asked ND25)*
4. Backward interpolation (estimate near table end) or Lagrange (unequal intervals, small table).
5. Operator relations: E=1+Δ, Δ∇=Δ−∇, δ etc. — short theory Q1 material.
6. Simpson's 3/8 rule numerical (listed in syllabus; combine with 1/3 for composite rules).
7. Stirling/Bessel (self-learning) — one short note possible.

### Notes to remember
- Forward: u=(x−x₀)/h, y=y₀+uC₁+u²C₂+… Use FORWARD when interpolating near the TOP of the table, backward near the bottom.
- Trapezoidal: h/2[(y₀+yₙ)+2(middle terms)]. Simpson 1/3: h/3[(y₀+yₙ)+4(odd)+2(even)]. Simpson needs EVEN intervals; 3/8 needs multiples of 3.
- ln 10 = 2.302585 — the ND25 answer check: both rules under/over-estimate monotonically for 1/x.

## MODULE 4 — Vector Calculus

### Possible questions
1. **Prove irrotational + find potential φ + evaluate ∫F·dr (work)** between two points. *(asked BOTH RAI papers AND both COMP papers — the single most repeated question in this course. Practice 3 variants.)*
2. **Green's theorem** numerical evaluation. *(asked both RAI papers)*
3. Angle between surfaces x²+y²+z²=12? & plane... at (2,−2,2). *(MJ25)*
4. Directional derivative of φ=x²+y²+z² along line L at (1,2,3); direction of max increase. *(ND25; COMP variant: normal to surface x log z − y² + 4 = 0)*
5. Gauss divergence theorem: evaluate flux of F=4xi+3yj−2zk over closed surface (COMP asked; syllabus 4.5 → expect as Q5 option).
6. Stokes' theorem: evaluate ∮F·dr for F=x²i+xyj around rectangle / circle boundary (COMP asked twice; same unit → **high probability Q5 for RAI**).
7. Show points with given position vectors are coplanar (COMP ND25 short).
8. Solenoidal check: div F = 0 (short Q1).
9. Find constants a,b,c so that F is irrotational (COMP MJ25 short).

### Notes to remember
- Irrotational ⇒ curl F = 0 ⇒ F = ∇φ. Get φ by integrating components: φ = ∫P dx + ∫(Q−∂φ/∂x terms)dy + …
- Work along a path = ∫F·dr; for a conservative (irrotational) field it's path-independent = φ(B)−φ(A) — use this to check your line-integral answer.
- Green: ∮(M dx+N dy) = ∬(∂N/∂x − ∂M/∂y)dx dy — reduce the line integral to an area integral over the region.
- Angle between surfaces = angle between normals ∇F₁·∇F₂/(|∇F₁||∇F₂|).
- Directional derivative = ∇φ·â; maximum = |∇φ| in direction of ∇φ.
- Gauss: ∯F·n̂ dS = ∭div F dV. Stokes: ∮F·dr = ∬(curl F)·n̂ dS.

## MODULE 5 — LPP / Optimization

### Possible questions
1. **Simplex method** full iteration problem. *(asked both RAI papers)*
2. **Write the dual** of a given LPP. *(asked both RAI papers)*
3. Find all **basic solutions**, identify basic feasible / non-degenerate / optimal. *(asked MJ25)*
4. Convert to **standard form** (surplus + artificial variables) + matrix form. *(asked ND25)*
5. Big-M method on an LPP with ≥ or = constraints (syllabus 5.2; not yet asked directly → likely next).
6. Duality theory short: state primal-dual relationships (weak duality, complementary slackness idea).
7. Dual simplex (self-learning — short note possible).

### Notes to remember
- Standard form: all constraints as equalities with slack/surplus, RHS ≥ 0, x ≥ 0. Canonical: max ↔ min swap, constraint directions flip, transpose A, b ↔ c.
- Dual of Max z = cᵀx s.t. Ax ≤ b, x≥0 is Min w = bᵀy s.t. Aᵀy ≥ c, y ≥ 0.
- Simplex: pick most negative in z-row (entering), min-ratio test (leaving), pivot. Stop when z-row has no negatives. Optimal z(primal) = z(dual) — check your dual answer with this.
- Basic solutions: choose n columns from m constraints... if all basics ≥ 0 → feasible; if any basic variable = 0 → degenerate.
- Big-M: penalize artificials with −M in z-row for max problems; drive artificials out of the basis.

---

## WHAT I'D PRACTICE TONIGHT (one of each archetype, re-ordered by official weights)
**Tier 1 (20+20):** A (irrotational, Q4) + one Laplace inverse pair (M1) + B (Green's, Q5) + DD short (Q1).
**Tier 2 (15+15):** C (dual, Q1) + D (simplex, Q3) + E (half-range Fourier, Q1) — plus the overdue ODE-by-Laplace (M1's second item).
**Tier 3 (10, skippable):** G (trapezoidal+Simpson OR interpolation — pick one).
