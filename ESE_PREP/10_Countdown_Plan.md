# 10 — DAY-BY-DAY EXAM COUNTDOWN PLAN (Nov 9 → Nov 30)

## PLAIN-ENGLISH CHEAT SHEET (read this first)

1. 5 exams, every one at 2:30–4:30 pm: CTO 18th, MoM 20th, DSA 23rd, HPS 26th, MPR 30th.
2. The killer detail: **MoM gets only ONE day** between the CTO and MoM exams. So MoM must be ~90% ready before Nov 18.
3. Plan shape: **Nov 9–16 = cover everything** (2 days CTO, 2 MoM, 2 MPR, 1 HPS, 1 DSA), **Nov 17 = CTO final**, then each exam is followed by focused days for the next one.
4. Every afternoon 2:30–4:30 you either take a TIMED sample paper or do heavy practice in that slot — your brain must peak at exam time, not at 11 pm.
5. Method is never "read". Every session you DO: derive the formula, trace the code, draw the circuit, write the CNC program from memory. You learn like you build bots — hands first.
6. Timed paper for each subject = 07_Sample_Papers Paper 1 (BEST prediction, 83% backtested).
7. Carry: scientific (NOT programmable) calculator, your own drawing instruments + charts — borrowing is forbidden in the hall.
8. No phone/smartwatch in the hall. Reach by 2:15 pm. Seating list goes up on the notice board that morning.
9. Exam evening = 1 hr rest, then 2 hrs starting the NEXT subject. Never zero, never more.
10. If you lose a day, the recovery order is: skip the "second pass" items (marked OPTIONAL), never skip a timed paper.

---

## THE TIMETABLE (from your official SVU circular, OCR-verified)

| Day | Date | Time | Subject (RAI) | Code | Gap before it |
|---|---|---|---|---|---|
| Wed | 18-Nov-26 | 2:30–4:30 pm | Calculus, Transforms & Optimization | 316U43C301 | 9 days from Nov 9 |
| Fri | 20-Nov-26 | 2:30–4:30 pm | Mechanics of Materials | 316U43C302 | **1 day** |
| Mon | 23-Nov-26 | 2:30–4:30 pm | Data Structures & Algorithms | 316U43C303 | 2 days |
| Thu | 26-Nov-26 | 2:30–4:30 pm | Hydraulic & Pneumatic Systems | 316U43C304 | 2 days |
| Mon | 30-Nov-26 | 2:30–4:30 pm | Manufacturing Processes | 316U43C305 | 3 days |

Format (all subjects): 50 marks, 2 hrs, Q1–Q5 with internal choice.
CTO/MoM/DSA/HPS: Q1 any-two×5, Q2 or Q3×10, Q4 both×5, Q5×5.
MPR: Q1 any-two×5, Q2 any-two×5, Q3 any-one×10, Q4×10, Q5 (5+5).

## WHY THE PLAN LOOKS LIKE THIS

- **MoM is the trap.** Highest priority (25% of your risk) + only one gap day → it gets two FULL days now (Nov 11–12) so Nov 19 is pure polishing, not learning.
- **CTO is first.** Second-highest priority (25%) + appears before you've built exam stamina → two days now + a dedicated final day (Nov 17).
- **MPR has the biggest syllabus + a 20-mark CNC block + your Mod 4–5 material gap** → two days now, plus the longest final stretch (3 days).
- **DSA is your most predictable subject** (100% topic prediction, full book available, MSE already covered Mod 1–3.1) → one day now, two full days before it.
- **HPS is compact and pattern-driven** (MJ25/ND25 table, circuit drawing) → one day now, two before.

## YOUR PERSONAL WEAK SPOTS (from the paper analysis — attack these)

- MoM Mod 3–4 (≈20/50 marks): your study material was thin here. SFD/BMD, torsion, principal stress/Mohr.
- MPR Mod 4–5 (≈20/50 marks): non-conventional machining (ECM/EDM/USM) + NDT. Pressing/working of metals too.
- CTO: **Laplace (20 offered) + vector calculus (20 offered) are the two pillars** — Green/Gauss/Stokes + the Q4 irrotational family have a 100% appearance rate in history. Free marks if drilled. Numerical methods (10, skippable) goes last.
- HPS: Q4+Q5 are DRAWING questions — drawing circuits is a motor skill, you can't cram it the morning of.

---

# PHASE 1 — COVER EVERYTHING (Sat Nov 8 mindset: you're already ahead; Mon Nov 9 → Mon Nov 16)

Daily rhythm: **Morning 9:30–12:30** (heavy learning) · **Afternoon 2:30–4:30** (exam-slot training) · **Evening 7:00–9:00** (active recall + fix errors). Nights: sleep by 11:30, non-negotiable — your exams are all afternoon but recall is built overnight.

## Mon Nov 9 — CTO Day 1 (Laplace + ODEs) — *M1 = 20 offered marks, the joint-heaviest module*
- AM: Read `09_Visual_Guides/01_CTO_visual_guide.md` fully, pen in hand. Re-derive every Laplace rule and the 4 ODE archetypes ON PAPER (incl. verified y = t − sin t + cos t). Official weights (M1 20 · M2 15 · M3 10 · M4 20 · M5 15): today's module is a 20 — treat it accordingly.
- PM: 25 Laplace/inverse problems from the guide's table — mix shift, partial fractions, the e⁻ᵃᵗsin bt types. No peeking at the table after the first 10.
- EVE: Flash-write the Laplace table from memory, check, mark gaps.

## Tue Nov 10 — CTO Day 2 (Vector + LP; Numericals demoted)
- AM: Vector calculus FIRST (M4 = 20 offered): Green's, Gauss', Stokes' worked examples from the guide (100% hit-rate topic) + the Q4 irrotational family + DD shorts (DD = 110/7 verified).
- PM: Simplex loop + dual rules (M5 = 15); re-solve Big-M to z = 12 at (6,0). Then Fourier half-range pair (M2 = 15).
- LAST 45 min only — Numerical methods (M3 = 10, skippable): Newton fwd/bwd ONE each + trapezoidal & Simpson's on the same table (ln10 pair). Nothing more — under the official weights a second numerical method is marks you'll never attempt.
- EVE: 10 mixed questions from `01_CTO_question_bank.md`; check against `08_Answer_Keys/01_CTO_key.md`.

## Wed Nov 11 — MoM Day 1 (all verified numericals)
- AM: `09_Visual_Guides/02_MoM_visual_guide.md` fully. Re-derive by hand ALL 8 verified numericals: composite bar (22.3/44.7 MPa), thermal stress, bending, torsion (1.54°), T-section (ȳ = 67.8 mm, I = 3.14×10⁶ mm⁴).
- PM: δ=PL/AE family + E=2G(1+μ) + flexure-formula problems. Derive the flexure formula in the 4 moves shown in the guide — derivations are asked directly.
- EVE: Theory quickfire: fatigue, Griffith, SCC (needs ALL THREE), stress-strain chart from memory.

## Thu Nov 12 — MoM Day 2 (your weak Mod 3–4)
- AM: SFD/BMD — cantilever + simply-supported cases, point load + UDL. Draw, then check shear/moment values. This is your gap area: grind 6–8 beams.
- PM: Torsion + principal stresses + Mohr's circle — draw 5 circles for different states. Re-do the rotated-cantilever 120 MPa case (note the 2× factor trap).
- EVE: OPTIONAL if drained: skim question bank Q2/Q3 list so the question shapes feel familiar.
- ⚠ If your Mod 3–4 notes are still thin, TODAY is the day to photocopy a friend's — not Nov 19.

## Fri Nov 13 — MPR Day 1 (CNC block — 20 marks in ND25)
- AM: `09_Visual_Guides/05_MPR_visual_guide.md` CNC section. Memorize the G/M-code table (write it out twice from memory).
- PM: Write BOTH full programs from memory on paper: the turning program and G81 drilling (G81 Z-15.0 R5.0 F100). Block-by-block, say what each block does. Then indexing math: 40/N rule + the worked examples.
- EVE: Casting 8 steps + defects bank + pattern allowances — flash-recall each.

## Sat Nov 14 — MPR Day 2 (forming/welding/NDT)
- AM: Sheet metal (blanking vs piercing vs drawing), welding (arc vs gas table, spot, soldering vs brazing) — these are compare-questions, learn them AS tables.
- PM: NDT five methods (dye penetrant = red bleed-out, magnetic, UT, radiography, visual) + ECM/EDM/USM principles — your Mod 4–5 gap; draw each process labelled.
- EVE: 10 bank questions from `05_MPR_question_bank.md`, check with `08_Answer_Keys/05_MPR_key.md`.

## Sun Nov 15 — HPS Day (pattern + circuits)
- AM: `09_Visual_Guides/04_HPS_visual_guide.md` fully. Memorize the MJ25/ND25 pattern table. Hydraulic vs pneumatic full comparison.
- PM: DRAW circuits — this is the skill. All 12 from the guide's drill list, from memory: single-acting, double-acting, meter-in/meter-out, sequencing (sequence valve opens at setting), counterbalance, unloading. Every valve: symbol + label.
- EVE: The four pressure valves distinguished (relief / reducing / sequence / counterbalance) + Pascal's law, lift force (7200 N type), continuity worked numericals.

## Mon Nov 16 — DSA Day (+ evening audit)
- AM: `09_Visual_Guides/03_DSA_visual_guide.md`. BST: write insert/search/delete C functions from memory — including the two-children inorder-successor case. Hand-trace on the ND21 exam tree (preorder 10 4 3 1 5 8 11 12 14).
- PM: Stacks: push/pop code + infix→postfix trace (a b c * + d e − /) + postfix evaluation (verified answers 27 and 7). Then sorts: write each, trace one pass each, complexity table from memory.
- EVE (90 min): SELF-AUDIT — pick 1 question from each of the 5 banks, attempt in 10 min each, tally your weak topics. This list steers your gap days.

## Tue Nov 17 — CTO FINAL
- AM: Laplace table + ODE-by-Laplace archetypes FIRST (M1 = 20), then vector theorems re-derive (M4 = 20). Formula sheet only — nothing new.
- PM 2:30–4:30: **TIMED: `07_Sample_Papers/CTO Paper 1 (BEST)`** — strict exam conditions, calculator, no pauses.
- EVE: Mark it with the inline key. Every dropped mark → its topic gets 15 min re-drill. Then formula sheet once, sleep by 11.

---

# PHASE 2 — EXAM-BY-EXAM

## Wed Nov 18 — CTO EXAM
- AM: formula sheet + Laplace table skim ONLY. Nothing new. Eat lunch, reach by 2:15.
- 2:30–4:30: EXAM. Hall order: read all 5 Qs in first 5 min → pick your strongest internal choices → ~20 min per 10-marker, ~10 per 5-marker → keep last 10 min to check arithmetic.
- EVE: 1 hr complete rest. Then 2 hrs: skim `02_MoM_visual_guide.md` headers + formula sheet (light — the heavy lifting was Nov 11–12).

## Thu Nov 19 — MoM CRUNCH (the one gap day — no new learning after 4:30)
- AM: All 8 verified numericals AGAIN by hand, timed (15 min each). SFD/BMD two beams.
- PM 2:30–4:30: **TIMED: MoM Paper 1 (BEST)**.
- After: mark it, Mohr circle one more time, E=2G(1+μ) + flexure derivation written once. Formula sheet before bed. Sleep.

## Fri Nov 20 — MoM EXAM
- AM: formula sheet only. Reach 2:15.
- EVE: rest 1 hr → 2 hrs light: DSA guide headers + complexity table skim.

## Sat Nov 21 — DSA Day 1
- AM: BST all three C functions from memory + delete cases on the ND21 tree. SLL insert (head/end) + traversals as pseudocode.
- PM: infix→postfix new expressions (make up 5), evaluate postfix — the verified method: one stack, push operands, pop two on operator.
- EVE: rebuild-binary-tree-from-traversals worked example (from the guide) + bank Qs on stacks/queues.

## Sun Nov 22 — DSA Day 2
- AM: all four sorts — write, trace, complexity table. Binary search trace.
- PM 2:30–4:30: **TIMED: DSA Paper 1 (BEST)**.
- EVE: mark it; re-trace whatever you dropped. Code skim before bed.
- SKIP (sister-branch only, never asked from RAI): hashing, AVL, Dijkstra, MST, Z-transforms.

## Mon Nov 23 — DSA EXAM
- AM: C code skim + complexity table only.
- EVE: rest → 2 hrs: HPS pattern table + valve symbols redrawn once.

## Tue Nov 24 — HPS Day 1
- AM: Redraw all 12 circuits from memory; check against guide. Wrong ones → redraw immediately.
- PM: components-of-hydraulic-system + Pascal/lift/continuity numericals (7200 N type). PLC scan cycle: Read ALL inputs → execute → update outputs.
- EVE: MJ25/ND25 pattern table flash + past-paper Q list from the bank.

## Wed Nov 25 — HPS Day 2
- AM: weakest 4 circuits again + hydraulic vs pneumatic table written from memory.
- PM 2:30–4:30: **TIMED: HPS Paper 1 (BEST)**.
- EVE: mark it; every circuit question you avoided in the paper gets drawn now.

## Thu Nov 26 — HPS EXAM
- AM: pattern table + valve symbols only. Pack drawing instruments + charts tonight.
- EVE: rest → 2 hrs: MPR guide headers + G-code table skim.

## Fri Nov 27 — MPR Day 1
- AM: casting 8 steps, defects, allowances, welding compares — as flash-recall, not reading.
- PM: indexing problems (40/N) ×6, lathe operations + up-milling vs climb-milling + cutter nomenclature + grinding wheel spec.

## Sat Nov 28 — MPR Day 2
- AM: BOTH CNC programs from memory again + G/M table. Block-by-block explanation aloud.
- PM 2:30–4:30: **TIMED: MPR Paper 1 (BEST)**.
- EVE: mark it; NDT five methods flash.

## Sun Nov 29 — MPR Day 3 (final full day)
- AM: Mod 4–5 deep pass — ECM/EDM/USM labelled diagrams from memory, pressing/working of metals, SLA rapid-prototyping figure (it was a Q4 in ND25).
- PM: full `05_MPR_visual_guide.md` one-pass, ticking topics you can already flash-recall. Unticked → 10 min each.
- EVE: light — G-code table + casting steps. Sleep early.

## Mon Nov 30 — MPR EXAM — LAST ONE. Finish it and the semester is done.

---

## EXAM-DAY PROTOCOL (from the circular itself)
- 2:15 pm at the hall (15 min early is mandated). Seating on the notice board that morning.
- FORBIDDEN: phone, smartwatch, any electronics, books, notes, paper.
- ALLOWED + REQUIRED: scientific non-programmable calculator (CTO/MoM numericals), YOUR OWN drawing instruments and charts (HPS/MPR diagrams). No borrowing, no exchange mid-exam.
- 2 hrs / 50 marks budget: 5 min choose → strongest-first → ~20 min per 10-marker → 10 min per 5-marker → final 10 min check units and arithmetic.

## IF YOU LOSE A DAY (recovery rules)
- Drop the OPTIONAL/evening second-pass items first. Never drop: a timed Paper 1, the MoM Nov 11–12 days, CNC program practice.
- Behind on everything? Per-subject minimum viable prep = visual guide one-pass + timed Paper 1 + that subject's 08_ answer-key skim. That alone covers the 83%-backtested core.
- Two days before any exam and still shaky: skip Paper 2 (GOOD) attempts; drill the subject's weak-spot list from the Nov 16 audit instead.

## FILE MAP (what to open, when)
| Need | File |
|---|---|
| Complete subject revision | `09_Visual_Guides/0X_*_visual_guide.md` |
| Question drill | `01–05_*_question_bank.md` |
| Check answers | `08_Answer_Keys/0X_*_key.md` |
| Timed mock | `07_Sample_Papers/*Paper 1*` (BEST tier) |
| Extra paper if ahead | `07_Sample_Papers/*Paper 2*` (GOOD tier) |
| Print pack | `PDF/` (29 files, A4) |
