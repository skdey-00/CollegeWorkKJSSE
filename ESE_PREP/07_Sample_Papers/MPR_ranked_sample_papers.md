# MPR — RANKED SAMPLE PAPERS (3 papers, best → decent)

Format per RAI ND-2025: Q1 any-two ×5 · Q2 any-two ×5 · Q3 any-one ×10 · Q4 ×10 · Q5 (5+5).

Evidence codes: [ND25] = exact item in the only real RAI paper · [SYL] = syllabus-first-item rule (validated: predicted SLA/ECM/UT correctly) · [ROT] = rotation · [NEW] = never asked.

---

# ======== PAPER 1 — BEST PREDICTION ========

**Q1. Attempt any two:** *(2×5=10)*
(i) Steps of the **casting process** with a neat diagram. **[ND25 exact]**
(ii) **Subtractive / additive / chipless** manufacturing — define with examples. **[ND25 exact]**
(iii) Differentiate **arc welding vs gas welding**. **[ND25 exact — Q1 slot took exactly these three families]**

**Q2. Attempt any two:** *(2×5=10)*
(i) **Simple vs compound indexing** with one example each. **[ND25 exact]**
(ii) Milling cutter nomenclature — diagram with labels. **[ND25 exact]**
(iii) Lathe operations: turning/facing/taper turning sketches. **[ROT — same module-2 pool]**

**Q3. Attempt any one:** *(10)*
(i) CNC advantages over conventional machines + **part program (turning)** for stepped shaft Ø45 stock: Ø45→Ø30 over 20 mm, then Ø20 over 10 mm; face + part off; explain G/M codes. **[ND25 exact — turning program was Q3]**
(ii) **CNC drilling program with canned cycle G81** for 4 holes Ø8 at corners of 60×40 plate; explain codes. **[ND25 exact — drilling program was Q3 second item]**

**Q4. Attempt the following:** *(10)*
**SLA (Stereolithography)** with a neat figure: principle, parts, working, advantages, limitations. **[ND25 exact + SYL — first RP process named in syllabus]**

**Q5. Attempt the following:** *(5+5=10)*
(a) **ECM** with a neat figure: principle, electrolyte, MRR, applications. **[ND25 exact + SYL — first NC process named]**
(b) **Ultrasonic testing (UT)** with figure: principle, transducer, advantages, applications. **[ND25 exact + SYL — first NDT method named]**

---KEY P1---
Q3(i): %; G21 G90 G97; T0101 M03 S800; G00 X47 Z2; G01 X45 F0.2 → X30 Z−20 → X20 W−10; G00 X100 Z100; M30.
Q3(ii): G81 X_ Y_ Z_ R_ F_ per hole (or G91 shifts); G80; G98/G99.
Q4: UV laser, vat, elevator, recoater; post-cure; finest finish.
Q5(a): NaCl electrolyte, Faraday MRR, mirror finish, no tool wear, conductors only.
Q5(b): piezoelectric transducer + couplant; pulse-echo; subsurface; thickness gauging.

---

# ======== PAPER 2 — GOOD PREDICTION ========

**Q1. Attempt any two:** *(2×5=10)*
(i) **Soldering vs brazing**. **[ROT — welding-family short]**
(ii) Casting defects (four, cause+remedy). **[ROT]**
(iii) **Rolling / forging / extrusion** — define + sketch each (metal forming = chipless family). **[ROT]**

**Q2. Attempt any two:** *(2×5=10)*
(i) **Shaper** with quick-return mechanism sketch. **[ROT]**
(ii) **Up vs climb milling** with sketches. **[ROT]**
(iii) Grinding machine types (surface/cylindrical/centerless) — one line + sketch each. **[ROT]**

**Q3. Attempt any one:** *(10)*
(i) NC/CNC **constructional features** (ball screws, servos, encoders, ATC) + PTP vs contouring + advantages. **[ROT — theory half of ND25's Q3]**
(ii) **G-codes family**: G00/G01/G02/G03/G81/G82/G83 meanings + write a facing+turning program with coolant codes explained. **[ROT]**

**Q4. Attempt the following:** *(10)*
**FDM** with figure: principle, ABS/PLA, working, adv/lim vs SLA + one line each on SLS and LOM. **[ROT — FDM is syllabus-second RP process; rotate from SLA]**

**Q5. Attempt the following:** *(5+5=10)*
(a) **EDM** with figure: principle, dielectric, spark erosion, applications (die-sinker vs wire). **[ROT — second NC process]**
(b) **Dye-penetrant testing** with figure: steps, detects surface flaws only. **[ROT — second NDT method]**

---KEY P2---
Q4: FDM cheapest; anisotropic; supports; PLA vs ABS temp (~180 vs ~220–250 °C).
Q5(a): 8000–12000 °C sparks; kerosene/deionized; tool wear inverse polarity; conductors only.
Q5(b): clean→penetrate→dwell→remove→develop→inspect; red bleed-out.

---

# ======== PAPER 3 — DECENT PREDICTION ========

**Q1. Attempt any two:** *(2×5=10)*
(i) Shell moulding / investment casting — process + two advantages. **[NEW]**
(ii) Spot welding (resistance welding) — sketch + applications. **[NEW]**
(iii) Sheet-metal operations: blanking/piercing/drawing/bending with sketches. **[NEW]**

**Q2. Attempt any two:** *(2×5=10)*
(i) **Drilling machine** parts + operations. **[NEW]**
(ii) Differential indexing — concept + one example. **[NEW — syllabus names it; ND25 asked simple+compound only]**
(iii) Abrasive machining: grinding wheel specification/grade/structure. **[NEW]**

**Q3. Attempt any one:** *(10)*
(i) **CNC lathe vs machining centre** + write a program with subprogram/canned cycle G83 (peck drilling) for a deep hole. **[NEW]**
(ii) **Part programming for milling**: contour with G02/G03 arcs, cutter compensation G40/41/42. **[NEW]**

**Q4. Attempt the following:** *(10)*
**SLS** (or LOM) with figure: principle, powder sintering, materials (nylon), no supports, vs SLA/FDM. **[NEW — syllabus RP items 3–4]**

**Q5. Attempt the following:** *(5+5=10)*
(a) **USM / WJM / LBM / PAM** — any one with figure: principle, abrasive jet/laser/plasma, applications. **[NEW — remaining NC processes]**
(b) **Magnetic particle inspection or radiography** with figure: principle, ferro-only / film-based, vs UT. **[NEW — remaining NDT]**

---KEY P3---
Q2(ii): differential = simple + change-gear offset of the plate; formula 40/(N±z) style with gear ratio.
Q3(i): G83 pecks Z−5 R1 Q5 F_; subprogram M98/M99.
Q4: SLS laser sinters nylon powder; no supports; functional parts.
Q5(a): USM 20 kHz horn+slurry, brittle mats; WJM 1000 m/s jet+garnet; LBM focused CO2/ND:YAG; PAM 20k °C plasma.

---HOW THESE WERE RANKED---
MPR has ONE real paper, so "best" = ND25 repeats + syllabus-first-items (the two rules that scored 90% in validation). The examiner repeated identical items across windows in other subjects (CTO dual/simplex/Green asked in BOTH 2025 papers) — so ND25's exact items are the modal repeat. P2 = the named seconds (FDM, EDM, DP). P3 = the rest of the syllabus (SLS/LOM, WJM/LBM/PAM, MPI/radiography, differential indexing, milling contour) — full-coverage insurance.
Reminder: you have NO college material for Q4/Q5 content — source RP + NC-machining + NDT notes first (gap list in STUDY_PLAN.md).
