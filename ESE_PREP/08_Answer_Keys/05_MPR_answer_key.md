# ANSWER KEY — 05 · Manufacturing Processes

Covers every "possible question" in 05_Manufacturing_Processes.md. Diagram-led answers: what to draw + what to label + working steps.

---

## MODULE 1 — Casting, Forming, Welding

**1. Steps of casting** *(asked ND25)*: 1) Pattern making 2) Mould preparation (green sand in flask: cope/drag) 3) Core setting (if needed) 4) Melting (furnace) 5) Pouring (ladle → gate) 6) Solidification & cooling 7) Shakeout (sand removed) 8) Fettling/finishing (cut risers/gates, clean, inspect). Draw two-box mould cross-section: cope, drag, pattern cavity, gate, riser, runner, core, vent.

**2. Patterns**: types: solid/one-piece, split, match-plate, sweep, skeleton, loose-piece. Materials: wood (cheap, low life), aluminium (light, best all-round), cast iron (long life, heavy), plastic/epoxy, wax (investment). Allowances: shrinkage/contraction (most important — pattern larger), machining, draft (taper for withdrawal), distortion, shake/movement.

**3. Moulding types**: Green sand (clay+silica+water — cheapest, most used). Dry sand (baked — better surface). **Shell moulding**: resin-coated sand against heated metal pattern → hard shell halves → glued → fine finish, accurate, good for medium volume; draw heated pattern + dump box + shell. CO₂ process: sodium silicate sand gassed with CO₂ → instant hardening. **Investment (lost wax)**: wax pattern cluster → ceramic slurry dip → stucco → dry → burnout wax → pour → break shell — excellent finish, complex shapes (turbine blades). Centrifugal: mould spins, metal thrown outward — dense, fine grain, cylindrical parts (pipes, liners); no risers/gates needed. Die casting (HPDC): molten metal injected under high pressure into metal die — very high rate, non-ferrous (Al, Zn); vs gravity die (permanent mould): poured by gravity, better quality, slower.

**4. Casting defects**: blowholes (gas entrapment — wet sand/insufficient vents), cold shut (two streams meet but don't fuse — low pouring temp), misrun (cavity unfilled — thin sections/low temp), shrinkage cavity (insufficient feed metal — riser too small), hot tears (restrained contraction), sand wash/inclusions, porosity. Finishing: fettling → shot blasting → machining.

**5. Forming definitions** (each = definition + sketch): **Rolling** (metal passed between rotating rolls — plates/sheets; draw two rolls + stock). **Forging** (compressive shaping between dies — crank, spanners; drop vs press). **Extrusion** (billet pushed through die — rods/tubes; direct vs indirect). Wire drawing (pulled through successive dies). Sheet metal: **Blanking** — punch cuts the OUTLINE, slug IS the product; **Piercing** — hole punched, slug is scrap; **Drawing** (cup/deep drawing — flat blank → cup); **Bending** (angle in a straight line). Remember: blanking/piercing are identical mechanics, opposite products.

**6. Welding**: **Arc vs gas** *(asked ND25)*: arc — consumable flux-coated electrode + work arc ~6000–7000 °C, faster, deeper penetration, equipment power supply + electrode holder; gas (oxy-acetylene ~3100–3200 °C flame + filler rod) — portable, cheap, slower, better control on thin sheet. Resistance/spot: current through overlapped sheets + pressure → local fusion at interface — lap joints, sheet-metal bodies (draw two electrodes + sheets + nugget). Electroslag: vertical thick plates, molten slag pool resistance-heats. Laser beam: focused coherent beam — tiny HAZ, precise, no vacuum; electron beam: high-velocity electrons in VACUUM — deepest penetration, needs vacuum chamber.

**7. Soldering vs brazing** *(Prod ND25 10-marker)*: both use filler, base metal does NOT melt. Solder: filler < 450 °C (Sn-Pb, Sn-Cu) — electrical joints, plumbing, weak. Brazing: filler > 450 °C (copper-zinc, silver alloys) — stronger joint, carbide tool tips, bicycle frames. Compare: temp, strength, filler, application + sketches of joint + torch.

**8. Welding defects** (sketch each): undercut, incomplete penetration, slag inclusion, porosity/blowholes, spatter, distortion, cracks, overlap.

**9. PCB manufacturing**: substrate (FR4 glass-epoxy) → copper cladding → drill holes → pattern (photoresist + etch FeCl₃) → plating → solder mask → silkscreen → test. One-line steps acceptable for 5 marks.

## MODULE 2 — Subtractive

**1. Lathe**: parts: bed, headstock (spindle + chuck), tailstock (dead/live centre), carriage (saddle, cross-slide, compound, tool post), apron, lead screw, feed rod. Operations: turning (reduce diameter along axis), facing (flat end surface), taper turning (compound-slide set at half-angle / tailstock offset / taper attachment), knurling, cutting, drilling, boring, parting. Work-holding: 3-jaw self-centring (round/hex), 4-jaw independent (square/off-centre), collet (precise small bars), faceplate (irregular), between centres.

**2. Milling**: multi-tooth cutter rotates while work feeds. Operations: face (flat surface), slab/surface, slotting, gear cutting, straddle, gang. **Up (conventional) vs climb milling**: conventional — cutter rotation OPPOSITE to feed, tooth starts at zero chip thickness, safer, rubs slightly, no backlash need; climb — rotation WITH feed, starts max chip thickness, better finish + tool life, REQUIRES backlash-free machine — draw both with arrows.

**3. Indexing** *(asked ND25)*: purpose: divide work into equal angles (gear teeth, splines). Simple: crank turns = 40/N (40:1 ratio standard); e.g. 8 divisions → 5 full turns. Compound: change gears (A/B)×(C/D) multiply the ratio for non-simple N. Differential: plate itself rotates via gear train from work spindle — for prime N like 127.

**4. Milling cutter nomenclature** *(asked ND25 — draw + label)*: end mill/slab cutter with: tooth/face, rake angle (tooth face), clearance/relief angle (flank), land, flute, body, hub/arbor hole. Label cutting edge, primary/secondary clearance.

**5. Shaper**: quick-return — Whitworth/hydraulic drive: cutting stroke slow (forward), return stroke fast (~2:1 ratio) — draw crank + slotted lever. Operations: flat surfaces, slots, grooves, V-blocks, gears ( indexing), keyways.

**6. Grinding**: types: surface (flat), cylindrical (between centres — rotate + traverse), centerless (work on blade between grinding + regulating wheel — no centres, through-feed/in-feed — high production of pins), internal, tool & cutter. Wheel spec: e.g. 51-A-36-L-5-V-23: abrasive (A Al₂O₃), grain size, grade (hardness of bond), structure, bond (V vitrified).

**7. Drilling vs reaming**: drill cuts original hole; ream finishes existing hole to accurate size/finish (slight stock removal, multi-flute, no heavy cutting).

## MODULE 3 — CNC

**1. NC vs CNC + features + advantages** *(asked ND25 — full 10-mark answer)*: NC = punched-tape hardwired control; CNC = dedicated mini-computer controller storing/editing programs. Constructional: machine body, recirculating BALL screws (zero backlash — convert rotation to motion), AC servo motors per axis, linear/rotary ENCODERS (feedback), ATC (auto tool changer), tool magazine, coolant, spindle with programmable speed. Classification: PTP (positioning only — drilling) vs continuous-path/contouring (milling, turning); 2.5/3/4/5-axis. Advantages: high repeatability, complex profiles, reduced operator skill, less WIP, CAD/CAM integration, fewer fixtures, inspection reduced.

**2. G/M codes** (memorise table): G00 rapid traverse · G01 linear interpolation · G02 CW arc · G03 CCW arc · G04 dwell · G28 home · G40/41/42 cutter comp off/left/right · G81 drilling cycle · G82 counterbore (with dwell) · G83 peck drilling · G80 cancel cycle · G90 absolute · G91 incremental · G92 offset · G94/G95 feed/min vs feed/rev · G96 constant surface speed · G97 rpm. M03 spindle CW · M04 CCW · M05 stop · M06 tool change · M08 coolant on · M09 off · M00 program stop · M02 end · M30 end+reset.

**3. CNC turning part program** *(asked ND25)* — stepped shaft Ø45→Ø30×20→Ø20×10:
```
%
O0001
N10 G21 G90 G97;          (mm, absolute, rpm mode)
N20 T0101;                 (tool 1, offset 1 — turning tool)
N30 M03 S800;              (spindle CW, 800 rpm)
N40 G00 X47.0 Z2.0 M08;    (rapid to start, coolant on)
N50 G01 X45.0 F0.25;       (approach stock)
N60 G01 X30.0 Z-20.0 F0.2; (taper/step cut to Ø30 at 20 mm)
N70 G01 X20.0 W-10.0;      (step to Ø20, next 10 mm — W incremental)
N80 G00 X100.0 Z100.0 M09; (retract, coolant off)
N90 M05;
N100 M30;                  (end, reset)
%
```
Explain each word: N block number, G function, X/Z coordinates (X = DIAMETER in turning), F feed mm/rev, S speed, T tool, M miscellaneous.

**4. Drilling with canned cycle G81** *(asked ND25)* — 4 holes Ø10 corners of 60×40 plate:
```
%
O0002
N10 G21 G90 G80 G40;       (safety line: metric, absolute, cancel cycles/comp)
N20 G54 X0 Y0;             (work offset)
N30 M06 T02;               (tool 2 — Ø10 drill)
N40 M03 S1200 M08;
N50 G00 X10.0 Y10.0;       (rapid to hole 1)
N60 Z5.0;                  (approach plane R)
N70 G81 Z-15.0 R5.0 F100;  (canned cycle: drill to depth 15, retract to R)
N80 X50.0;                 (hole 2 — cycle repeats at new X)
N90 Y30.0;                 (hole 3)
N100 X10.0;                (hole 4)
N110 G80;                  (cancel cycle)
N120 G00 Z50.0 M09;
N130 M05; M30;
%
```
G81 = drill → retract rapid; each new X/Y while active drills another hole — one block per hole instead of 6.

**5. Canned cycles**: pre-stored repetitive sequences (drill, peck, tap, bore) — shorten programs, less error. G81 drill, G82 drill+dwell (counterbore — break chip/flat bottom), G83 peck (deep holes — retract clears chips each peck Q).

**6. Word/address format**: each block = words: N (sequence), G (preparatory), X/Y/Z (dimensions), F (feed), S (speed), T (tool), M (miscellaneous). Explain "address + number".

## MODULE 4 — Rapid Prototyping

**1. RP principle**: additive layer-by-layer fabrication directly from CAD: CAD → STL tessellation → slicing into layers → machine builds layer by layer → post-process. Advantages: fast iteration, no tooling, complex geometries free, custom parts (medical). Disadvantages: material limits, anisotropy, surface finish, size limits, cost per part for volume.

**2. SLA** *(asked ND25 Q4)* — draw: vat of liquid PHOTOPOLYMER resin, UV laser (He-Cd/solid-state), galvanometer mirrors (steer beam), elevator platform (drops per layer ~0.1 mm), recoater blade. Working: laser traces layer cross-section → photopolymer solidifies → platform drops → recoater sweeps fresh resin → next layer, bonds to previous → after build: drain, wash (solvent), UV POST-CURE oven. Advantages: highest accuracy/finest features of RP, smooth surface. Limitations: resin expensive, brittle, photosensitive degradation, needs supports, post-cure needed.

**3. SLS**: powder bed (nylon/PA12, polystyrene, elastomers, sand); CO₂ laser SINTERS (fuses) layer; un-sintered powder SUPPORTS the part — no supports needed; functional nylon parts; rougher surface than SLA; no post-cure.

**4. FDM**: thermoplastic FILAMENT (ABS ~220–250 °C, PLA ~180–220 °C) fed by rollers through heated nozzle; extruded strand deposited layer-wise; build platform; supports = second material (break-away/soluble). Cheapest, desktop-friendly, anisotropic (weak across layers), visible layer lines.

**5. LOM**: adhesive-coated PAPER sheets laminated + laser/blade cuts outline each layer; cheap sheet material, wood-like parts; wasteful, poor fine detail.

**6. STL + slicing** (overdue short): STL = triangular facet mesh of CAD surface (chordal tolerance); slicing software cuts model into horizontal layers, generates toolpaths/hatching + supports. Mention file size vs resolution trade-off.

**7. RP comparison table**: rows: material (liquid resin / powder / filament / paper), accuracy (best SLA), supports (SLS no), strength (FDM/SLS functional), cost, post-processing, typical use (visual models SLA/LOM; functional SLS/FDM).

## MODULE 5 — Non-Conventional Machining + NDT

**1. ECM** *(asked ND25 Q5a)* — draw: tool (cathode −), workpiece (anode +), small gap (~0.5 mm) with electrolyte (NaCl/NaNO₃) pumped at high velocity, DC supply 5–20 V, high current. Principle: reverse electroplating — Faraday electrolysis dissolves workpiece atom by atom at the gap; tool shapes the field → cavity forms. NO tool wear (tool is cathode), NO thermal damage, mirror finish, any CONDUCTOR regardless of hardness — turbine blade airfoils, dies, deburring. MRR by Faraday's law (MRR = AI/(zFρ)).

**2. EDM**: controlled SPARKS (10⁴–10⁵ Hz) between tool and work in dielectric (kerosene/deionized water); spark temp 8000–12000 °C melts/vaporizes micro-craters; servo maintains gap; dielectric flushed (suction/pressure). Tool DOES wear (graphite/copper/tungsten), inverse polarity for low tool wear. Die-sinking (3D cavity) vs WIRE-cut (2D profile through sheet with traveling wire electrode). Only conductors; HAZ/thin recast layer; dies, moulds, carbide.

**3. WJM/AWJM**: high-pressure water (up to 400 MPa) jet ~800–1000 m/s through sapphire nozzle; add garnet abrasive for hard metals (AWJM); NO heat-affected zone, cuts any material (composites, glass, food); noisy, abrasive recycling.

**4. LBM**: focused laser (CO₂ / Nd:YAG) vaporizes material — drilling tiny holes, cutting sheet, medical; HAZ small; no tool contact; in AIR. EBM: high-velocity electron beam in VACUUM — highest depth-to-width welds/drills, tiny holes, expensive vacuum equipment. Compare: LBM in air vs EBM vacuum; both thermal.

**5. PAM**: constricted arc through nozzle → plasma ~20,000 °C — cuts THICK metal fast (steel plates), rough cut edge, noisy/ glare.

**6. USM**: magnetostrictive/ piezo transducer at ~20 kHz + concentrator HORN amplifies amplitude; abrasive slurry (boron carbide/SiC in water) hammered into work by tool; micro-chipping — BRITTLE materials only (glass, ceramics, carbide, germanium); no thermal effects; low MRR; tool wears (soft steel tool).

**7. NDT methods**: **Visual** — eyes/magnifier, surface only. **Dye penetrant**: clean → spray PENETRANT (15 min dwell) → remove excess → apply DEVELOPER → red bleed-out marks surface-breaking cracks — any material, surface only. **Magnetic particle**: magnetize (yoke/coil) → sprinkle dry/wet fluorescent particles → leakage field at crack attracts particles — FERROMAGNETIC only, surface + near-surface. **Radiography**: X-ray/γ (Ir-192) through part onto film — internal voids/inclusions appear as density differences; expensive, radiation hazard; permanent record. **Ultrasonic testing** *(asked ND25 Q5b)*: piezoelectric TRANSDUCER sends pulse through couplant; normalincident echoes: initial → flaw echo → back-wall echo on CRT screen; flaw DEPTH = (flaw-echo position / back-wall position) × thickness; detects internal defects in thick sections, thickness gauging; needs skilled operator, couplant, complex geometry hard.

**8. NDT comparison table**: method × (defect location: surface/subsurface/internal), material limit, cost, speed, record permanence.

---

## THE 6 DIAGRAMS TO BE ABLE TO DRAW BLIND
casting mould cross-section (cope/drag/gate/riser) · milling cutter nomenclature · CNC coordinate figure for turning (X diameter, Z length) · SLA machine (vat/laser/mirrors/elevator/recoater) · ECM cell (tool −, work +, electrolyte flow, gap) · UT A-scan screen (initial/flaw/back-wall echoes)
