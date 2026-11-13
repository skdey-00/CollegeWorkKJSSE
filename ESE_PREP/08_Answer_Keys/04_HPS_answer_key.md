# ANSWER KEY — 04 · Hydraulic & Pneumatic Systems

Covers every "possible question" in 04_Hydraulic_Pneumatic_Systems.md. For this subject the marks are in labelled diagrams + component naming + working steps — each answer below lists exactly what to draw and name.

---

## MODULE 1 — Automation & Fluid Power Basics

**1. Need & types of automation**: reduce cost/time/error, hazardous-task safety, repeatability. Types: fixed (hard automation — high volume, e.g. bottling), programmable (CNC/PLC — batch variety), flexible (reconfigurable — robotics FMS).

**2. Generalized pneumatic system**: draw block chain: Compressor → Aftercooler → Receiver → FRL (Filter-Regulator-Lubricator) → Directional valve → Actuator (+ exhaust silencer). Label each block's function in one line.

**3. Reciprocating compressor**: piston-cylinder + inlet/discharge reed valves; down-stroke sucks air (inlet valve opens), up-stroke compresses & pushes to receiver (discharge opens). Types: single/two-stage (intercooling), rotary screw (continuous, quiet).

**4. FRL unit**: Filter (coalescing — removes dust/moisture before air reaches valves), Regulator (reduces & holds line pressure, with relief), Lubricator (venturi adds oil mist for moving parts). Draw the combined symbol trio.

**5. Air receiver**: stores compressed air, damps piston-compressor pulsations, lets moisture drop out; sized ~ (output − demand) × time / pressure drop.

**6. Pressure devices**: **Bourdon tube** *(asked MJ25)*: oval-section C-tube; internal pressure straightens it → linkage/gear → needle on calibrated dial. Draw tube + linkage + pointer. **Piezoelectric** *(asked ND25)*: quartz/ceramic crystal generates charge ∝ pressure → amplifier → reading; fast dynamic response. **Diaphragm gauge**: pressure deflects elastic diaphragm → transmission. **Manometer**: liquid column U-tube; P = ρgh.

**7. Pascal's law** *(asked ND25)*: pressure applied to confined fluid transmits equally in all directions: P = F/A. Applications: hydraulic lift/jack/press/brakes, robotic grippers.

**8. Hydraulic lift numerical** *(asked MJ25)*: F₂ = F₁(A₂/A₁) = F₁(D₂/D₁)². 60 cm & 5 cm pistons, 50 N → F₂ = 50×(60/5)² = **7200 N**. Variant 40/4 cm, 20 N → **2000 N**.

**9. Continuity** *(asked MJ25)*: A₁V₁ = A₂V₂ (incompressible steady flow) — pipe sizing, actuator speed from pump flow (v = Q/A), velocity in narrowed pipe.

**10. Hydraulic vs pneumatic table** *(asked ND25 — 100% must-prepare)*: medium oil vs air; pressure 70–350 bar vs 2–10 bar; force high vs moderate; speed slower vs very fast; control precision high vs lower (compressibility); cost higher vs lower; fire/explosion safety better vs excellent; leakage messy vs clean; typical use presses/heavy robots vs packaging/grippers.

**11. Logic in pneumatics**: AND = twin-pressure (dual-pressure) valve, OR = shuttle valve — both introduced here, examined as circuits in M2.

## MODULE 2 — Pneumatic & Electro-Pneumatic Circuits

**1. Symbols (ISO 1219)**: single-acting cylinder (single piston rod + spring), double-acting (two ports), 3/2 valve (3 ports/2 positions), 5/2 valve, one-way flow control (throttle + check), shuttle (two inlets arrow-merge), twin-pressure (two inlets AND-block).

**2. Direct control of single-acting cylinder**: 3/2 NC valve (push-button) between FRL and cylinder; press → extend; release → spring retracts. Components: supply, FRL, 3/2 valve, cylinder, exhaust.

**3. Oscillatory (auto-reciprocation) circuit** *(asked MJ25)*: 5/2 pilot-operated DCV; roller-lever limit valves at both stroke ends feed pilot ports alternately; cylinder self-reverses continuously. Draw cylinder with two roller valves at ends, pilot lines labelled.

**4. Indirect control of double-acting cylinder** *(asked ND25)*: small 3/2 push-button sends pilot signal to main 5/2 valve which switches main flow — small valve handles signal, big valve handles power. Components: FRL, 3/2 PB, 5/2 pilot DCV, double-acting cylinder.

**5. Logic circuits**: AND — twin-pressure valve requires both PBs; OR — shuttle valve, either PB extends single-acting cylinder.

**6. Time-delay valve** *(asked MJ25)*: one-way FCV charging an air reservoir → pressure builds slowly → piloted 3/2 switches after set time. Symbol: FCV+reservoir+pilot 3/2. Application: dwell between two cylinder actions, press-hold-then-return.

**7. Shuttle valve** *(asked ND25)*: body with two inlets one outlet, free-moving ball/piston; higher-pressure inlet pushes ball to block other side — output = whichever signal present (OR). Application: control a cylinder from either of two stations / safety interlock.

**8. Solenoid valves**: coil + armature shifts spool; 3/2 single solenoid (spring return), 5/2 double solenoid (last-position memory). Draw both symbols.

**9. Relays** *(asked MJ25)*: coil + iron armature + NO/NC contacts; energize coil → armature pulls → contacts change. Advantages: isolation (low-voltage control switching high-power), amplification, multiple simultaneous contacts, latching ability. Draw coil symbol + contact symbols.

**10. Latching**: NO contact in parallel with momentary PB keeps coil energized after release; NC stop PB breaks the path. Draw two-rung ladder.

**11. Auto-return electro-pneumatic** *(asked MJ25)*: PB → solenoid Y1 of 5/2 → cylinder extends → forward limit switch (NC→NO changeover) triggers Y2 → auto retract. Draw electrical part (PB, LS, Y1/Y2) + pneumatic part.

**12. OR logic electro-pneumatic** *(asked ND25)*: two NO PBs in parallel → either energizes relay K1 → K1 contact drives solenoid → single-acting cylinder extends. Electrical OR = parallel contacts.

**13. Power supply** *(asked ND25)*: converts mains 230 V AC to 24 V DC for solenoids/sensors; provides isolation (transformer), protection (fuse), smoothing (rectifier+capacitor); standard in electro-pneumatics.

**14. AND logic electro-pneumatic**: two NO PBs in series → both needed → relay → solenoid. Series = AND, parallel = OR.

## MODULE 3 — Hydraulics & Electro-Hydraulics

**1. Hydraulic fluids** *(asked MJ25)*: properties: proper viscosity + high VI (stable across temperature), lubricity, oxidation resistance, demulsibility (shed water), anti-foam, pour/flash point, compatibility with seals. Types: mineral-based (common), synthetic (fire-resistant — phosphate ester), water-glycol; selection by pressure/temperature/fire risk. Additives: VI improvers, anti-wear (ZDDP), anti-foam, antioxidants, rust inhibitors. Filter (fine, pressure/return line) vs strainer (coarse mesh, pump inlet) — 10 µm vs ~150 µm.

**2. Pumps**: Gear — two meshing gears carry oil in tooth spaces; cheap, noisy, fixed displacement, ~20–200 bar, tolerant of dirt. Vane — slotted rotor in cam ring; quieter, can be variable displacement/pressure-compensated. **Piston pump** *(asked ND25)*: axial swash-plate — rotating cylinder block, pistons reciprocate, ~300+ bar, efficient, costly; vs plunger pump: single plunger + seal, simple, low-pressure/lab use.

**3. Accumulators** *(asked MJ25)*: store pressurized fluid (energy reserve), damp pulsations, emergency power, leakage compensation. Types: weighted (constant pressure, huge), spring (low pressure), gas-charged: bladder (gas in rubber bladder inside shell — draw), diaphragm, piston.

**4. Intensifiers** *(asked ND25)*: large-area piston drives small-area piston → P₂ = P₁(A₁/A₂) — get high pressure from low-pressure source. Types: single-stage (air-oil), two-stage.

**5. DCVs**: 4/3 closed-centre (block all — hold load), tandem (pump unloaded, cylinder held), open (free flow to tank); check valve (one-way), pilot-operated check (free return when pilot signal) *(asked MJ25 — two types with symbols + use)*.

**6. Pressure valves**: **Relief** — normally closed, pilot senses pump line, opens at setting to tank = safety. **Reducing** — limits pressure in a branch below system. **Sequence** *(asked ND25)* — opens at set pressure to feed a SECOND actuator: circuit: pump → clamp cylinder; its line through sequence valve → press cylinder; clamp reaches pressure → sequence opens → press strokes. **Counterbalance** *(asked MJ25)* — pressure-controlled check in the rod-end line of a vertical cylinder; set slightly above load-induced pressure → prevents falling; smooth descent of presses/plastic-injection moulding. **Unloading** — external signal dumps pump to tank at low pressure (pump idles between operations).

**7. Flow control**: needle (non-compensated — flow varies with load), **pressure-compensated FCV** *(asked ND25)* — internal compensator holds ΔP across throttle constant → flow independent of load. **Meter-in**: FCV at cylinder inlet (resistive loads). **Meter-out**: FCV at outlet (overrunning/negative loads — presses) *(asked ND25)*. **Bleed-off**: FCV bleeds excess to tank before the valve — more efficient, less stable speed.

**8. Hydraulic circuit symbols**: pump (circle with triangle out), relief (square with arrow + spring), cylinder, 4/3 valve — practise the 8 most common.

**9. Electro-hydraulic basic**: solenoid 4/3 + cylinder + relay control — mirror the electro-pneumatic ladder.

**10. Power pack**: reservoir + pump + electric motor + relief + filter + gauge — draw labelled.

## MODULE 4 — PLC

**1. PLC advantages**: reprogrammable vs rewiring relays; reliable (no moving contacts), compact, diagnostics, easy integration SCADA; cost-effective for complex logic.

**2. Ladder symbols**: NO contact |¬|, NC |∨|, coil ( ), timer TON/TOF, counter CTU — draw each.

**3. Gates in LLD**: AND = contacts in series; OR = parallel.

**4. Start-stop with latch**: rung: NC Stop — NO Start ∥ NO seal-in (of coil) — coil M. Classic — draw + explain seal-in holds after Start release; Stop breaks.

**5. Single-cylinder PLC cycle**: inputs: start PB, LS1 (retracted), LS2 (extended); outputs: Y1 extend, Y2 retract; rungs: Start AND LS1 → Y1; LS2 → TON; TON.DN → Y2 (auto-return). Cycle: extend → dwell (timer) → retract.

**6. Scan cycle**: read all inputs → execute ladder top-to-bottom → write outputs → repeat (ms scale).

## MODULE 5 — Applications

**1. Robotics applications**: pneumatic grippers (fast, clean, simple open/close), vacuum suction cups for picking, hydraulic actuators for heavy-payload arms/legs (high force density), pneumatic joints for light assembly robots. Construction: excavators (hydraulic booms), jacks, brakes. Manufacturing: hydraulic presses, clamping fixtures, pneumatic tools, conveyors.

**2. Hydraulic case study (press)**: power pack → 4/3 valve → press cylinder; relief set above working pressure; draw + walk through one stroke; components: pump, relief, DCV, cylinder, gauge, filter, reservoir.

**3. Pneumatic case study (pick-and-place)**: double-acting X-axis cylinder + gripper; sequence: extend X → grip (gripper cylinder) → retract X → release; controlled by roller-lever valves or PLC; draw the two-cylinder circuit with limit valves.

**4. Fluid power vs electric drives**: higher force density (hydraulics), explosion-safe (pneumatics), instant stall tolerance; electrics win on efficiency/cleanliness — choose per application.

---

## WHAT TO PRACTISE DRAWING (the 20-mark Q4+Q5 bank)
oscillatory circuit · indirect control · single-acting direct + speed control · AND (twin-pressure) & OR (shuttle) · time-delay valve symbol · auto-return electro-pneumatic · OR/AND electro-pneumatic with relays · latching ladder · start-stop ladder · sequencing (hydraulic) · counterbalance · meter-in & meter-out · relief-valve protection circuit · bladder accumulator · power pack
