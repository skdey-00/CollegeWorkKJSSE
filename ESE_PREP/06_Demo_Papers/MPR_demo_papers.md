# MPR — DEMO PAPERS (3 papers, exam format: 50 marks · 2 hrs)

Format cloned from RAI ND-2025 (316U43C305): Q1 any-two ×5 · Q2 any-two ×5 · Q3 any-one ×10 · Q4 attempt ×10 · Q5 both (5+5). Note: ND25's Q3 actually carried two programming items (turning + drilling) — expect similar.

---

# =================== DEMO PAPER 1 ===================

**Q1. Attempt any two:** *(2×5=10)*
(i) Explain the steps of the **casting process** with a neat diagram.
(ii) Differentiate **soldering and brazing** (filler, temp, strength, applications).
(iii) Define with sketches: blanking, piercing, drawing, bending.

**Q2. Attempt any two:** *(2×5=10)*
(i) **Lathe operations**: list and explain turning, facing, taper turning with sketches.
(ii) Explain **simple vs compound indexing** with one example each.
(iii) Draw a **milling cutter** and label its nomenclature parts.

**Q3. Attempt any one:** *(10)*
(i) Discuss advantages of **CNC over conventional lathe**; write a **CNC part program** (turning) for a stepped shaft from Ø45 stock — 30 mm length steps as per figure you draw: Ø45→Ø30 over 20 mm, then Ø20 over 10 mm, face and part off. Explain each G/M code.
(ii) Write a **CNC drilling program using canned cycle G81** for 4 holes of Ø8 mm at the corners of a 60×40 mm rectangular plate (bolt-hole circle alternative: holes on 50 mm PCD). Assume cutting speed & feed; explain codes.

**Q4. Attempt the following:** *(10)*
Describe the **SLA (Stereolithography)** technique of additive manufacturing with a neat figure: principle, machine parts, working, advantages, limitations.

**Q5. Attempt the following:** *(5+5=10)*
(a) Explain **EDM (Electric Discharge Machining)** with a neat figure: principle, dielectric, MRR factors, applications.
(b) Describe **dye-penetrant testing** of NDT with a neat figure: steps, what it detects, limitations.

---KEY POINTERS (Demo 1)---
Q3(i): program skeleton — %; N10 G21 G90 G97; N20 T0101 M03 S800; G00 X47 Z2; G01 X45 F0.2 → turning passes G01 X30 Z−20; G01 X20 W−10; G00 X100 Z100; M30. Codes: G90 absolute, G01 linear interpolation, M03 spindle CW, M06 tool change, M30 end.
Q3(ii): G81 X_ Y_ Z_ R_ F_ repeated per hole or with X/Y shifts; G80 cancel; G98/G99 return plane.
Q4: SLA: UV laser + photopolymer resin vat + elevator + recoater; layer ~0.1 mm; needs supports & post-cure; finest surface finish of RP.
Q5(a): EDM: controlled sparks 8000–12000°C, tool (−) work (+), dielectric kerosene; only conductors; die-sinker vs wire-cut.
Q5(b): clean → apply penetrant (15 min) → remove excess → developer → inspect (red indication); surface-breaking defects only.

---

# =================== DEMO PAPER 2 ===================

**Q1. Attempt any two:** *(2×5=10)*
(i) Differentiate **arc welding and gas welding** (ND25 clone).
(ii) Explain **shell moulding** with diagram; two advantages over green sand.
(iii) Casting defects: name four with causes and remedies sketches.

**Q2. Attempt any two:** *(2×5=10)*
(i) **Shaper**: construction with quick-return mechanism — explain with sketch.
(ii) **Grinding**: types of grinding machines (surface, cylindrical, centerless) — one line each with sketch.
(iii) Explain **up (conventional) vs climb milling** with sketches; when is climb preferred?

**Q3. Attempt any one:** *(10)*
(i) Explain NC, CNC: constructional features (ball screw, servo, feedback), classification (PTP/contouring), advantages. Write a G-code **facing + turning** program with tool-change & coolant codes explained.
(ii) **Canned cycles**: explain G81/G82/G83 with meanings. Write a drilling program for 6 holes on a 60 mm PCD at Z−15 through 12 mm plate: assume centre, speed, feed; explain each block.

**Q4. Attempt the following:** *(10)*
Explain **FDM (Fused Deposition Modelling)** with a neat figure: principle, materials (ABS/PLA), working, advantages/disadvantages vs SLA. Add one line each on SLS and LOM to complete the RP family.

**Q5. Attempt the following:** *(5+5=10)*
(a) Explain **Ultrasonic Machining (USM)** with figure: transducer-horn-abrasive slurry; why only brittle materials.
(b) Describe **magnetic particle inspection** with figure: principle, ferromagnetic limitation, continuous vs residual method.

---KEY POINTERS (Demo 2)---
Q3(i): constructional features — recirculating ball screws (zero backlash), AC servo motors, linear encoders, automatic tool changer, CNC controller; PTP vs continuous path.
Q4: FDM: thermoplastic filament (ABS/PLA) extruded through heated nozzle; cheapest RP; anisotropic strength; support material breaks away.
Q5(a): USM: 20 kHz transducer + concentrator horn + abrasive slurry (boron carbide); chips by micro-impact; glass/ceramics/carbide; no thermal damage but low MRR.
Q5(b): MPI: magnetize part, spray magnetic particles (dry/wet fluorescent); leakage field at surface cracks aligns particles; ferro only; surface & near-surface.

---

# =================== DEMO PAPER 3 — PREDICTED DEC-2026 MOCK ===================

**Q1. Attempt any two:** *(2×5=10)*
(i) Casting steps with diagram (M1 opener; ND25 asked — repeat candidate).
(ii) Subtractive / additive / chip-less (forming) manufacturing — describe with examples (ND25 asked — repeat candidate).
(iii) Resistance welding (spot) or rolling/forging/extrusion definitions — module-1 rotation pool.

**Q2. Attempt any two:** *(2×5=10)*
(i) Indexing simple vs compound with example (ND25 asked — repeat candidate).
(ii) Milling cutter diagram + nomenclature (ND25 asked; or rotate to milling operations/up-vs-climb).
(iii) Lathe work-holding devices or shaper quick-return — module-2 rotation.

**Q3. Attempt any one:** *(10)*
(i) CNC vs traditional advantages + **turning part program** (ND25 format: stock Ø45, stepped/tapered profile, explain G/M codes).
(ii) **Drilling canned-cycle program** G81 (ND25 format: 4 holes Ø10, rectangular plate, assume speed/feed).

**Q4. Attempt the following:** *(10)*
RP: **SLA with figure** (ND25 asked SLA — highest repeat probability) — prepare FDM/SLS as the rotation backup (both demo'd above).

**Q5. Attempt the following:** *(5+5=10)*
(a) Non-conventional: **ECM with figure** (ND25 asked — repeat candidate); rotation pool EDM/USM/WJM/LBM/PAM.
(b) NDT: **ultrasonic testing with figure** (ND25 asked — repeat candidate); rotation pool dye penetrant/MPI/radiography.

---HOW BUILT / SELF-SCORE---
MPR has only ONE real RAI paper — weakest evidence base of the five subjects (validation still scored 90% on it via the module-map + syllabus-first-item rule). Demo 3 therefore leans on "ND25 repeat candidates" (exam re-asked identical items in other subjects across windows, e.g. CTO dual+simplex+Green asked in BOTH 2025 papers) plus the syllabus-order rule: SLA, ECM, UT are literally the first named items in modules 4 & 5.
The MPR mock is intentionally close to ND25 because that paper IS the pattern-owner: Q1 casting+welding taxonomy, Q2 machining + indexing, Q3 both CNC programs, Q4 one RP process, Q5 one NC process + one NDT method.
Rubric: every answer needs a labelled sketch (marks are split diagram/theory ~50-50 in this subject); CNC program graded on format (N/G/M blocks, absolute coords, tool & speed lines, M30 end). 45+ ready; 38–44 solid; <38 → redraw the six core diagrams (casting, cutter, CNC coordinate figure, SLA, ECM, UT) from memory.
