# 05 · Manufacturing Processes (316U43C305) — ESE Question Bank

50 marks · 2 hrs · Q1 any-two ×5 · Q2 any-two ×5 · Q3 any-one ×10 · Q4 both ×10 · Q5 both ×5+5

Real RAI paper: Nov–Dec 2025. Reinforced with Production Engg-I ND25 (Mech) for module overlap.

RAI ND25 mapping: Q1 = casting steps + subtractive/additive/chip-less definitions + arc-vs-gas welding (Module 1). Q2 = indexing (simple vs compound) + milling cutter diagram & nomenclature (Module 2). Q3 = CNC advantages + **CNC part program** for turned component (Ø45 stock) + drilling 4 holes canned cycle (Module 3). Q4 = SLA with figure (Module 4). Q5 = ECM + ultrasonic testing (Module 5).

---

## CHEAT SHEET — the 10 recurring items

| # | Item | Evidence |
|---|------|----------|
| 1 | **Casting: steps/defects/moulding types with diagram** | RAI ND25 Q1, Prod ND25 Q1/Q2 |
| 2 | **Welding compare (arc vs gas) / defects / soldering-brazing** | RAI ND25 Q1, Prod ND25 Q1/Q4 |
| 3 | **Indexing: simple vs compound with example** | RAI ND25 Q2 |
| 4 | **Milling cutter diagram/nomenclature, milling operations** | RAI ND25 Q2, Prod ND25 Q1 |
| 5 | **CNC vs conventional lathe advantages** | RAI ND25 Q3 |
| 6 | **CNC part program (turning, G/M codes)** | RAI ND25 Q3 — 10 marker with figure |
| 7 | **CNC drilling program with canned cycle (G81)** | RAI ND25 Q3 |
| 8 | **RP: SLA process with figure** | RAI ND25 Q4 |
| 9 | **Non-conventional: ECM with figure** | RAI ND25 Q5 |
| 10 | **NDT: ultrasonic testing with figure** | RAI ND25 Q5 |

---

## MODULE 1 — Casting, Forming, Welding

### Possible questions
1. **Explain steps of casting with diagram** (pattern → mould → pour → solidify → shakeout → fettle) *(asked ND25)*.
2. Pattern types (solid, split, match-plate, sweep) + pattern materials + allowances; **design of patterns for moulding systems** *(Prod ND25 10-marker)*.
3. Moulding types: green sand, dry sand, shell moulding, CO₂, investment (lost-wax), centrifugal, die casting (hot/horizontal vs gravity) — "explain any one with diagram" *(Prod ND25)*.
4. Casting defects (blowholes, cold shut, misrun, shrinkage, hot tears...) with sketches *(Prod ND25)*; finishing of castings (fettling, cleaning).
5. Sheet forming/cutting: **blanking vs piercing**, drawing, bending, rolling, forging, extrusion, wire drawing — definitions + sketches (short-note bank).
6. Welding processes: **gas vs arc — differentiate** *(asked ND25)*; arc welding equipment/working; resistance welding (spot/seam); electro-slag; laser beam welding & cutting; electron beam welding.
7. **Soldering vs brazing** — with applications/advantages/disadvantages *(Prod ND25 10-marker)*.
8. Welding defects with sketches *(Prod ND25)*.
9. PCB manufacturing steps (syllabus-named; short note possible — RAI-flavoured).

### Notes to remember
- Green sand = clay+silica+water; shell moulding = resin-coated sand + heated metal pattern.
- Investment: wax pattern → ceramic slurry → burnout → pour. Die casting: high-rate, non-ferrous. Centrifugal: rotating mould, fine grain.
- Blanking = cut the workpiece out (slug is product); piercing = hole in workpiece (slug is scrap).
- Arc: consumable electrode, high temp, faster, deeper pen; Gas (oxy-acetylene ~3100°C): portable, cheaper, slower, flame adjustable.
- Solder < 450°C filler, brazing > 450°C, neither melt the base metal.
- Spot welding = resistance + pressure, lap joints, sheet metal.

## MODULE 2 — Subtractive (Lathe, Milling, Shaper, Grinding)

### Possible questions
1. **Lathe**: construction (bed, headstock, tailstock, carriage), operations (turning, facing, tapering — know taper turning methods), work-holding (3-jaw, 4-jaw, collet, faceplate) — standard Q2.
2. **Milling machine**: components, operations (face, slab, slot, gear), **up (conventional) vs climb milling** *(Prod ND25 short)*, universal milling machine *(Prod ND25 short)*.
3. **Indexing**: simple vs compound with one example each *(asked ND25)*; differential indexing *(Prod ND25)*. Formulae: 40/N; compound = (N₁/N₂)(A/B)...
4. **Milling cutter diagram**: single-angle/double-angle/end-mill/slab cutter nomenclature (tooth face, flank, rake, clearance angles) *(asked ND25 — draw + label)*.
5. **Shaper**: construction (ram, tool head, quick-return mechanism — Whitworth), operations *(Prod ND25 10-marker)*.
6. **Grinding**: types (surface, cylindrical, centerless, tool & cutter) + working; grinding wheel specification (letter code).
7. Drilling vs reaming *(Prod ND25)*; drill bit nomenclature possible short.

### Notes to remember
- Indexing: 40 teeth on index plate standard → one full rev turns work 1/40. Simple: 40/N turns. Compound: gear train (A/B)×(C/D) × 40/N.
- Quick-return: cutting stroke slow, return fast (ratio ~2:1).
- Climb milling: cutter rotation same as feed — better finish, needs backlash-free machine. Conventional: opposite — safer, rubs.
- Centerless: no centers, work supported by blade + regulating wheel — high production.

## MODULE 3 — CNC

### Possible questions
1. **NC vs CNC**; constructional features of CNC machine (ball screws, servo drives, feedback encoders, tool changer, controller); classification (point-to-point, contouring; 2/3/5-axis); advantages over conventional *(asked ND25 — prepare a full 10-mark answer)*.
2. **G-codes / M-codes**: meaning + use (G00 rapid, G01 linear, G02/G03 circular, G04 dwell, G81 drilling cycle, G90/G91 abs/inc; M03 spindle CW, M05 stop, M06 tool change, M08 coolant on, M09 off, M02/M30 end).
3. **Write a CNC turning part program** for a stepped/tapered component from Ø45 stock, explain codes *(asked ND25)*.
4. **Write a CNC drilling program using canned cycle** — 4 holes Ø10 in a plate *(asked ND25)*.
5. Canned cycles concept: what & why (G81 drill, G82 counterbore...).
6. Word/address programming format (N, G, X, Z, F, S, T, M blocks).

### Notes to remember
- Program skeleton: % / O-number → N10 G90 G71 (metric) → G00 X_ Z_ → G01... → G81 X_ Z_ R_ F_ → G80 → M30.
- Turning: X = diameter, Z = length (absolute from work face). Feed F mm/rev; speed S rpm (G97) or m/min (G96).
- Canned cycle = one block replaces repetitive hole moves; G80 cancels.
- CNC advantages: repeatability, complex profiles, less skill, CAD/CAM integration, inspection time down.

## MODULE 4 — Rapid Prototyping / 3D Printing

### Possible questions
1. **RP principle** (additive, layer-by-layer from CAD/STL), advantages/disadvantages of RP — general theory Q.
2. **SLA (Stereolithography)**: principle, machine parts (laser, vat, elevator platform, recoater), working with figure *(asked ND25 Q4 — 10 marks)*.
3. **SLS (Selective Laser Sintering)**: powder + laser — working, materials (nylon, PA12), vs SLA.
4. **FDM (Fused Deposition Modelling)**: filament extrusion — working; materials (ABS, PLA) — most relatable, likely alternative.
5. **LOM (Laminated Object Manufacturing)**: paper/adhesive sheets + laser cutting.
6. **STL file generation + slicing software working** (syllabus unit 4.2 explicit — didn't appear yet → overdue short/Q4).
7. Compare RP technologies table (material, accuracy, cost, speed, post-processing).

### Notes to remember
- All RP: CAD → tessellate to STL → slice (layers) → build layer-by-layer → post-process.
- SLA: photosensitive liquid resin + UV laser → polymerizes; needs supports + post-cure. Highest surface finish.
- SLS: powder bed, laser sinters; no supports needed; functional nylon parts.
- FDM: thermoplastic filament melted through nozzle; cheapest, desktop.
- LOM: glued paper sheets laser-cut — cheap, wood-like parts.

## MODULE 5 — Non-Conventional Machining + NDT

### Possible questions
1. **ECM (Electrochemical machining)**: principle (Faraday electrolysis), setup (tool cathode, work anode, electrolyte NaCl), working, MRR, advantages/disadvantages with figure *(asked ND25 Q5a)*.
2. **EDM (electric discharge)**: spark erosion, dielectric, die-sink vs wire-cut — the other big one; prepare equally.
3. **Water Jet / Abrasive Water Jet Machining**: principle, no HAZ, applications.
4. **Laser Beam Machining** and **Electron Beam Machining**: principle, focusing, comparison (LBM in air vs EBM vacuum).
5. **Plasma Arc Machining**: principle, temperature, cutting thick metal.
6. **Ultrasonic Machining (USM)**: brittle materials, abrasive slurry, horn/transducer — know diagram.
7. **NDT visual + dye penetrant** (steps: clean → penetrate → remove → develop), **magnetic particle** (ferro only), **radiography** (X-ray/γ internal defects), **ultrasonic testing** *(asked ND25 Q5b — pulse-echo, transducer, CRT screen, flaw echo between surface echoes)*.
8. Compare NDT methods table (defect type, material, cost, speed).

### Notes to remember
- ECM: reverse electroplating, tool doesn't wear, no thermal stress, any conductor (turbine blades).
- EDM: sparks ~8000–12000°C melt/vaporize; dielectric flushes; tool wears (graphite/copper); only conductors.
- USM: 20 kHz transducer + abrasive slurry; glass/ceramics; brittle materials only.
- Dye penetrant: surface cracks only, any material; magnetic particle: surface/near-surface, ferro only.
- Ultrasonic: pulse echo timing → flaw depth = (echo distance/total) × thickness.

---

## PRACTICE PRIORITY
(1) One CNC turning program + one drilling canned-cycle program (G81) — write by hand, 20 marks of Q3 across both RAI windows came from CNC; (2) SLA diagram + FDM/SLS working; (3) casting steps + defects; (4) arc vs gas + soldering/brazing; (5) ECM + ultrasonic NDT diagrams; (6) indexing + cutter nomenclature.
