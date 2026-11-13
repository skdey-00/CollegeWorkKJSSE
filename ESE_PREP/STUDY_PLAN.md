# STUDY PLAN — RAI Sem 3 ESE (Nov–Dec 2026)

Built from: past-paper weightage analysis (ESE_PREP pack) + validation test (83% item accuracy) + inventory of YOUR actual study material.

---

## PLAIN-ENGLISH SUMMARY (read first)

1. **Your material has dangerous gaps.** You have full slides for HPS (all 5 modules) and most of MoM/DSA. But:
   - **MoM:** no Module 3 (beams/bending) or Module 4 (torsion/Macaulay) notes — these carry ~40% of the paper (2 guaranteed numericals + parts of Q1). The scanned PDFs you have ("Principal Stresses", "Shear Force & Bending Moments") are handwritten-style notes; use them, but the torsion/Macaulay gap is real.
   - **MPR:** you only have Modules 1–3. Modules 4 (Rapid Prototyping — a guaranteed 10-mark Q4) and 5 (ECM/EDM/NDT — a guaranteed Q5) have NO material. Fix this first.
   - **CTO (Maths):** no folder at all. But it's formula-practice, not reading — the demo papers + Grewal-style worked examples cover it. **Official Nov-2026 module weights received: M1 Laplace 20 · M2 Fourier 15 · M3 Numerical 10 · M4 Vector 20 · M5 LPP 15 (offered with options).** Two consequences: (1) Laplace jumps to joint-heaviest — drill the property table + inverse pairs + one ODE-solve-by-Laplace until automatic; (2) Numerical Methods is only ONE skippable 10 — learn Newton-forward + trap/Simpson, then stop.
   - **DSA:** college slides cover hashing/set-map (not in RAI syllabus) — skip those; Reema Thareja book covers everything else.
2. **Study module-wise, not chapter-wise.** The exam maps 1 module = 1 question slot (validated 25/25). Every subject's Q1↔M1, Q2↔M2, Q3↔M3, Q4↔M4, Q5↔-within-M5, with small known swaps (DSA Q2/Q5 share linear+searching).
3. **Target ≈ 40/50 per subject:** master the archetype bank (the demo papers) + 2–3 rotation candidates per slot.
4. **Diagrams and code are the difference between 6/10 and 10/10.** Every HPS/MPR answer needs a labelled sketch; DSA answers want C snippets.

---

## GAP-FILL SHOPPING LIST (do today, 1 hr)

| Subject | Missing module | What to get | Why urgent |
|---|---|---7|---|
| MPR | Module 4 (RP) + Module 5 (NC machining + NDT) | NPTEL "Additive Manufacturing" notes or any SLA/SLS/FDM/LOM diagram sheet; one EDM/ECM/USM comparison chart; one NDT methods comparison chart | Q4 (10m) + Q5 (10m) = 20/50 marks guaranteed from these modules; ND25 asked SLA + ECM + UT exactly |
| MoM | Module 3 (SFD/BMD-lite, bending/shear in beams) + Module 4 (torsion + Macaulay) | Any Som "torsion of shafts" + "Macaulay's method" worked-examples sheet | Q3 bending numerical + Q4 Macaulay = 20/50; ND25 asked both |
| CTO | Everything | B.S. Grewal chapters: Laplace (20 offered — the pillar), Fourier, Numerical (10 — one method each), Vector, LPP-simplex/Big-M/duality | No material at all; formula-sheet + practice is enough (maths is doing, not reading). Official weights: M1 20 · M2 15 · M3 10 · M4 20 · M5 15 |

---

## THE PLAN — 4 passes over ~5 weeks (fits whatever time you actually have: compress by cutting Pass B short, never Pass A or C)

### PASS A — Archetype mastery (weeks 1–2) · target 40/50 locked in
Work through `06_Demo_Papers/` **one demo paper per study session, closed-book except formula sheet.** After each, mark with the answer-key pointers (given in each demo). Every archetype you drop, re-learn from your slides that same day.

Order (easiest marks first):
1. HPS Demo 1 → HPS Demo 2 (circuits; smallest syllabus, biggest repetition)
2. MoM Demo 1 → MoM Demo 2 (numerical archetypes are frozen since 2020)
3. CTO Demo 1 → CTO Demo 2 (8 recurring archetypes)
4. DSA Demo 1 → DSA Demo 2 (theory + C snippets)
5. MPR Demo 1 → MPR Demo 2 (after you've filled the M4/M5 gap)

### PASS B — Rotation coverage (week 3)
For each question slot, learn the 2–3 rotation candidates (listed in each subject file `01`–`05`):
- HPS: meter-in vs meter-out vs bleed-off; sequence vs counterbalance vs unloading; shuttle vs twin-pressure vs time-delay; AND vs OR electro-pneumatic.
- MoM: creep / Griffith / corrosion shorts; hollow-vs-solid shaft; UVL loading.
- CTO: ODE-solve-by-Laplace (now M1's likely second item under official weights — asked by COMP twice, never by RAI); Gauss/Stokes (both unasked in RAI yet); Big-M; Lagrange interpolation; Parseval.
- DSA: queue types/applications; tree-from-traversals; recursion-tree method.
- MPR: FDM/SLS/LOM vs SLA; EDM/WJM/LBM vs ECM; dye-penetrant/magnetic particle/radiography vs UT.

### PASS C — Mock exam week (week 4)
Sit `Demo_Paper_3` (the "predicted Dec-2026" paper) for each subject, timed 2 hrs, no notes. Mark yourself with the rubric at the end of each file. Score <35 → back to Pass A for that subject.

### PASS D — Final 72 hours
- Redo only the questions you dropped in Pass C.
- Rewrite the 5 one-page formula/sketch sheets (one per subject) from memory.
- Sleep before maths; the vector/LPP archetypes need a fresh head.

---

## DAILY SKELETON (adjust freely)

| Day type | Block 1 (75m) | Block 2 (75m) | Block 3 (45m) |
|---|---|---|---|
| Normal day | Demo paper (subject A) | Slides for dropped archetypes (subject A) | Flash-recall: circuits/sketches of subject B |
| Gap-fill day | MPR M4/M5 notes (you must source) | MoM M3/M4 torsion+Macaulay practice | CTO formula sheet build |
| Mock day | Timed Demo 3 | Self-mark + error log | Error-log re-attempts |

## PER-SUBJECT TIME SPLIT (based on weightage × your gap severity)

| Subject | Paper risk for you | Share of study time |
|---|---|---|
| MoM | Highest (missing M3/M4 notes + 3 frozen numericals) | 25% |
| CTO | High (no material, needs drilling not reading) | 25% |
| MPR | Medium-high (huge syllabus, missing M4/M5) | 20% |
| HPS | Medium (full notes; needs drawing practice) | 15% |
| DSA | Lowest (full coverage incl. book; theory-stable) | 15% |

## ERROR LOG RULE
Keep one page per subject: date · question type · what went wrong (concept / formula recall / arithmetic / diagram). Anything appearing twice gets a targeted half-hour the same week. This log, not the demo papers, is your real syllabus in week 4.
