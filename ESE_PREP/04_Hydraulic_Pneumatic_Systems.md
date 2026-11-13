# 04 · Hydraulic and Pneumatic Systems (316U43C304) — ESE Question Bank

50 marks · 2 hrs · Q1 any-two ×5 · Q2 any-one ×10 · Q3 any-one ×10 · Q4 both ×5 · Q5 both ×5

Two real RAI papers analysed: May–Jun 2025 + Nov–Dec 2025. Highest repetition density of all five subjects.

---

## CHEAT SHEET — the pattern is nearly fixed

| Q | MJ 2025 asked | ND 2025 asked |
|---|---------------|----------------|
| Q1 (any 2×5) | Bourdon tube note · hydraulic lift piston force · continuity equation | Piezoelectric pressure sensor · Pascal's law + industrial applications · hydraulic vs pneumatic comparison |
| Q2 (any 1×10) | Accumulators function+types · directional control valves (2 types) | Piston pump (construction/working/±) vs plunger · intensifiers types |
| Q3 (any 1×10) | Counterbalance circuit draw+explain+uses · hydraulic oil properties + additives | Sequence valve + sequencing circuit · pressure-compensated FCV + meter-in circuit |
| Q4 (5+5) | Pneumatic oscillatory circuit (double-acting cylinder) · time-delay valve + symbol | Indirect control of double-acting cylinder · shuttle valve |
| Q5 (5+5) | Relay construction/working/advantages · auto-return electro-pneumatic circuit | Power supply role in electro-pneumatic · OR-logic electro-pneumatic circuit (single-acting cylinder) |

**Read:** Q1 = fluid basics/laws/sensors. Q2 = pumps/components. Q3 = valves + hydraulic circuits. Q4 = pneumatic circuits draw. Q5 = electro-pneumatics + relays/logic.

---

## MODULE 1 — Automation & Fluid Power Basics

### Possible questions
1. Need of automation; types of automation (fixed/programmable/flexible); automated flow lines — short theory.
2. Generalized pneumatic system block diagram (compressor → FRL → valve → actuator).
3. **Air compressors**: types (reciprocating/rotary/screw), working — didn't appear yet in ESE but named in syllabus; possible Q2.
4. **FRL unit**: function of filter, regulator, lubricator — classic short note.
5. Air reservoir/crosservoir function; receiver sizing idea.
6. **Pressure measurement devices**: Bourdon tube *(asked MJ25)*, piezoelectric sensor *(asked ND25)* — also possible: diaphragm gauge, manometer.
7. **Pascal's law** + equation + industrial applications *(asked ND25)*.
8. **Hydraulic lift/piston numericals**: F = P·A ratio — 60 cm & 5 cm pistons, 50 N → F_large = 50×(60/5)² = 7200 N *(asked MJ25)*. Practice variants.
9. **Continuity equation** A₁V₁=A₂V₂ + uses *(asked MJ25)*; Bernoulli-type ideas.
10. **Compare hydraulic vs pneumatic systems** — merits/demerits table *(asked ND25)* — 100% must-prepare.
11. Logic gates in pneumatics (AND/OR later in Q5 form).

### Notes to remember
- Pascal: pressure transmits equally in all directions → F₂ = F₁(A₂/A₁).
- Hydraulic: incompressible oil, high force, precise; Pneumatic: compressible air ~8 bar typical, fast, clean, lower force.
- FRL = Filter (removes dirt/moisture) + Regulator (sets pressure) + Lubricator (oil mist).
- Bourdon: oval tube straightens under pressure → linkage → needle. Piezoelectric: crystal charge under pressure.

## MODULE 2 — Pneumatic & Electro-Pneumatic Circuits

### Possible questions
1. Pneumatic circuit **symbols** (ISO 1219): cylinders (single/double-acting), 3/2, 5/2 valves, FCV, shuttle, dual-pressure.
2. **Basic single-cylinder circuits**: direct control of single-acting cylinder (3/2 valve); speed control (one-way flow control).
3. **Oscillatory motion circuit** for double-acting cylinder *(asked MJ25)* — draw with 5/2 pilot-operated valve + roller levers at both ends.
4. **Indirect control** of double-acting cylinder (pilot-operated 5/2 via 3/2 push-button) *(asked ND25)* — name components.
5. Logic circuits: single-acting cylinder **AND** (twin-pressure valve = both signals), **OR** (shuttle valve = either signal).
6. **Time-delay valve** — construction, symbol, application *(asked MJ25)*.
7. **Shuttle valve** (OR element) with diagram *(asked ND25)*.
8. Solenoid valves: construction, 3/2 and 5/2 single/double solenoid — how they switch.
9. **Relays**: construction, working, advantages, symbols *(asked MJ25)*.
10. **Latching circuit** in electrical control (syllabus-named; likely Q5 short).
11. **Automatic return electro-pneumatic circuit** — PB (3/2 valve) extend, auto-return at forward end *(asked MJ25)*.
12. **OR logic electro-pneumatic** for single-acting cylinder *(asked ND25)* — relays/parallel contacts.
13. Power supply role in electro-pneumatic/hydraulic circuits *(asked ND25)* — 24V DC standard, protection.
14. AND logic electro-pneumatic (series relay contacts) — rotate from ND25's OR.

### Notes to remember
- Valve notation: ports/states → 3/2 = 3 ports 2 positions; 5/2 for double-acting cylinders.
- Single-acting cylinder: 3/2 valve, spring return. Double-acting: 5/2 valve.
- Shuttle valve = pneumatic OR; twin-pressure (dual-pressure) valve = pneumatic AND.
- Roller-lever valves at cylinder ends give automatic reciprocation (oscillatory motion).
- Relay: electromagnet → contacts close; electrically isolated control vs power circuit.
- Electro-pneumatic ladder: PB in series with relay coil; relay NO contact drives solenoid.

## MODULE 3 — Hydraulics & Electro-Hydraulics

### Possible questions
1. **Hydraulic fluids**: properties (viscosity, VI, lubricity, pour point, flash point, demulsibility, oxidation resistance), quality requirements *(asked MJ25)*; types + selection; additives + uses *(asked MJ25)*; filters & strainers difference.
2. **Hydraulic pumps** (didn't appear in either paper yet → overdue): gear, vane, **piston pump construction/working/adv/disadv vs plunger** *(asked ND25)*.
3. **Intensifiers** — types + diagram *(asked ND25)*; also accumulators function+types, one explained *(asked MJ25)*.
4. **Directional control valves** types: 4/3, 5/2, check valve, pilot-operated check *(asked MJ25)*.
5. **Pressure valves**: relief (safety), reducing, **sequence valve + sequencing circuit** *(asked ND25)*, counterbalance + circuit + applications *(asked MJ25)*, unloading.
6. **Flow control**: needle valve, **pressure-compensated FCV** *(asked ND25)*; **meter-in / meter-out / bleed-off circuits** — ND25 asked meter-in draw *(know all three)*.
7. Hydraulic circuit symbols.
8. Industrial electro-hydraulic circuits (basic: solenoid-operated 4/3 with cylinder).
9. Hydraulic power pack / power unit components (reservoir, pump, relief, filter, gauge).

### Notes to remember
- Accumulator types: weighted, spring-loaded, gas-charged (bladder/diaphragm/piston). Stores energy, damps pulsation, emergency supply.
- Intensifier: large-area piston drives small-area piston → P₂ = P₁(A₁/A₂).
- Sequence valve: pressure-operated — opens when upstream reaches set pressure → second actuator moves after first. Circuit: two cylinders in sequence.
- Counterbalance: back-pressure valve on cylinder outlet prevents falling loads (presses, loaders).
- Meter-in: FCV at inlet (resistive loads); meter-out: at outlet (negative/overrunning loads); bleed-off: branch to tank (less used).
- Pressure-compensated FCV: keeps flow constant despite load pressure changes.

## MODULE 4 — PLC

### Possible questions
1. PLC basics: what/why, advantages over relay logic (hardwired) — didn't appear in either paper yet → due as Q1 short or Q2.
2. Ladder logic symbols: NO/NC contacts, coil, timers, counters.
3. Logic gates in LLD (AND = series, OR = parallel).
4. Ladder diagram for simple operations: motor start-stop with latching (classic), AND/OR logic.
5. PLC circuit for single-cylinder sequential operation (extend→return cycle) *(syllabus 4.2 explicit)*.
6. PLC scan cycle: input → logic → output.

### Notes to remember
- Ladder: power rails L (left) and N; rung = contacts + coil. Start/stop latching: NO start ∥ NO seal-in contact, in series with NC stop.
- PLC beats relays: reprogrammable, reliable, compact, diagnostics.
- Cylinder sequence: two solenoid outputs, limit-switch inputs as conditions.

## MODULE 5 — Applications & Case Studies

### Possible questions
1. Applications of pneumatics/hydraulics **in Robotics** (grippers, actuators — syllabus headline for RAI), construction (excavators, jacks, brakes), manufacturing (presses, clamping, assembly).
2. Case study: any industrial hydraulic circuit (e.g. press machine) — explain components + working.
3. Case study: pneumatic pick-and-place / PLC-controlled automation line.
4. Combined short: where fluid power beats electric drives (high force density, safety in explosion zones).

### Notes to remember
- Prepare ONE hydraulic case (hydraulic press/jack/crane) and ONE pneumatic case (pick-and-place gripper) with sketch — reusable for any "application/case study" phrasing.
- Robotics hooks: pneumatic grippers, hydraulic heavy-arm actuation — easy RAI-flavoured marks.

---

## PRACTICE PRIORITY
Draw until your hand remembers: (1) double-acting cylinder oscillatory circuit, (2) indirect control circuit, (3) sequencing circuit, (4) meter-in/meter-out, (5) counterbalance, (6) electro-pneumatic OR + auto-return, (7) shuttle & twin-pressure & time-delay symbols. Q4+Q5 = 20 marks are pure circuit-drawing every single year.
