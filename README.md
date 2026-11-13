# ESE Paper-Pattern Intelligence — B.Tech Robotics & AI, Semester 3

Past-paper analysis turned into a complete, ranked, back-tested exam prep pack for the five Sem-3 subjects of the RAI branch (K.J. Somaiya, SVU 2023 scheme). Built Nov 2026 by a student, with AI doing the heavy lifting of reading every paper ever set for these subjects.

**Everything here was derived from legitimately available past papers and the official syllabus. No leaked papers. No paper "solutions" from the exam hall. Just pattern analysis.**

---

## READ THIS FIRST — the whole idea in 6 lines

1. Every ESE paper here is **50 marks, 2 hours, 5 questions × 10 marks** — all compulsory, but each question has internal choice ("attempt any two of three").
2. **One module = one question.** Q1 comes from Module 1, Q2 from Module 2, and so on. This held in **25 out of 25** question-slot checks across every paper analysed. Study module-wise, not chapter-wise.
3. **Examiners recycle question archetypes heavily.** The same 8–10 question *types* reappear session after session, rotating slightly within their slot (e.g. Bourdon gauge → piezometer, counterbalance valve → sequence valve).
4. So instead of "study everything equally," this pack ranks what's **most likely to appear** and drills that first — then covers the rest as insurance.
5. The prediction method was **back-tested**: predict the 2025 paper using only older evidence, then check against the real 2025 paper. Result: **83% exact item hits, 100% module-to-slot mapping** (see `ESE_PREP/PREDICTION_VALIDATION.md`).
6. **"Draw neat diagrams" is instruction #1 on every paper.** A labelled sketch is often half the marks. This pack treats diagrams as first-class content.

---

## THE MAP — what's in this repo

| Folder / file | What it is | When you'd open it |
|---|---|---|
| `ESE_PREP/` | **The generated study pack** — question banks, ranked sample papers, answer keys, visual guides, plans (see next section) | Daily, from now till the exam |
| `SORTED_BY_SUBJECT/` | **The raw evidence** — 41 real past papers, verified by branch code and sorted into the 5 subjects | When you want to see a real paper with your own eyes |
| `SEM 3 RAI.pdf` | The official syllabus everything was mapped against | Checking module boundaries |
| `Mechanics Of Materials (MMR)/`, `Hydraulics and Pnumatics Systems (HPS)/`, `Manufacturing Processes (MPR)/`, `Data Structures And Algorithms (DSA)/` | College slide decks + reference material (⚠ see "What is NOT in the repo" below) | First pass over a subject |

Two giant folders of ~2,200 raw exam PDFs per window (the original college archive) and their .zip parts are **deliberately kept out of the repo** — see the bottom of this file.

---

## START HERE — pick your situation

**Exam within ~2 weeks (this was mine):**
1. `ESE_PREP/README.md` → the 6-line cheat sheet + evidence table (10 min)
2. `ESE_PREP/10_Countdown_Plan.md` → the day-by-day plan (it was built around a real timetable: CTO → MoM → DSA → HPS → MPR, one day at a time)
3. Each subject, in exam order: the **Visual Guide** first (fast recall), then **Paper 1 (BEST prediction)** from `07_Sample_Papers/` under exam timing, then check against the key
4. Nights before each exam: the demo papers' inline answer keys + the question-bank cheat sheet for that subject

**A month or more:**
1. Read `ESE_PREP/STUDY_PLAN.md` — the 4-pass plan (archetype mastery → weak modules → timed papers → audit)
2. Work through `06_Demo_Papers/` closed-book, one per session
3. Read the subject question banks (`01_`–`05_`) properly — they're the "everything that can come" list with frequencies
4. Finish with the ranked sample papers as your mock-exam series

**You're from a different branch / college:**
- Skip to **"Reuse this method for your own subjects"** near the bottom. The pack itself is RAI-specific; the *method* is fully general.

---

## INSIDE `ESE_PREP/` — the pack, file by file

Every `.md` also exists as a clean printable PDF in `ESE_PREP/PDF/` (30 PDFs, diagrams rendered).

| # | File / folder | What it gives you |
|---|---|---|
| 01–05 | `01_Calculus_Transforms_Optimization.md` … `05_Manufacturing_Processes.md` | One file per subject: cheat sheet → paper pattern → recurring-questions table **with frequency counts** → full possible-question bank per module → notes to remember |
| — | `PREDICTION_VALIDATION.md` | The honesty check: guess-the-2025-paper-then-score-it experiment, question by question |
| — | `STUDY_PLAN.md` | Weightage-based 4-pass study plan + a gap-fill shopping list for missing study material |
| 06 | `06_Demo_Papers/` | 3 practice papers per subject (2 drills + 1 predicted-mock), each with inline answer keys |
| 07 | `07_Sample_Papers/` | **The ranked papers** — start here for exam prep. `00_HOW_RANKED.md` explains the tiers (below) |
| 08 | `08_Answer_Keys/` | Complete worked answer key per subject, covering EVERY question in the 01–05 banks |
| 09 | `09_Visual_Guides/` | The complete revision guide per subject: every definition, algorithm, pseudocode, C program, formula and worked example, structured with mindmaps and decision trees |
| 10 | `10_Countdown_Plan.md` | Day-by-day countdown built around a real 5-exam timetable, with per-gap-day crunch plans |

### The ranking system (this is the core trick)

Each subject gets 3 sample papers, ranked by prediction confidence:

| Tier | Paper | Built from | Expected coverage |
|---|---|---|---|
| 1 | **BEST PREDICTION** | Items asked in BOTH real RAI papers, or 3+ of 4 sister papers, or exact ND-2025 repeats | Master this alone → ~70–80% of the paper's marks are items you've seen |
| 2 | **GOOD PREDICTION** | Items asked once in RAI + the strongest rotation neighbour in that slot | Papers 1+2 → ~95% of marks |
| 3 | **DECENT PREDICTION** | Syllabus items never asked in RAI yet — overdue candidates | All three → nothing can appear you haven't practised |

Do them **in order**. Paper 1 cold, then Paper 2, then Paper 3 as insurance.

### The 5 subjects

Codes below are as printed on the actual paper headers (the syllabus PDF lists the same five courses with a 316U prefix — both refer to the identical SVU-2023 RAI scheme).

| Code (on paper) | Subject | Short name | Real RAI papers found | Sister-branch papers used |
|---|---|---|---|---|
| 216U43C301 | Calculus, Transforms & Optimization | CTO | 2 (MJ25, ND25) | 6 (ITVC, COMP/EXCP) |
| 216U43C302 | Mechanics of Materials | MoM | 1 (ND25) | 6 (SOM, Mech) |
| 216U43C303 | Data Structures & Algorithms | DSA | 2 (MJ25, ND25) | 17 (DS, COMP/IT/EXTC/AIDS) |
| 216U43C304 | Hydraulic & Pneumatic Systems | HPS | 2 (MJ25, ND25) | — |
| 216U43C305 | Manufacturing Processes | MPR | 1 (ND25) | 4 (Production Engg-I, Mech) |

RAI is a new branch — only 8 real RAI papers exist for these subjects. That's why sister-branch papers from the same scheme were mined for extra pattern evidence (their off-syllabus topics like hashing, AVL trees, Z-transforms are flagged and excluded).

---

## THE EVIDENCE — where the numbers come from

- **41 verified papers** in `SORTED_BY_SUBJECT/` — every one checked by opening the PDF and reading the programme code printed on its header (43 = RAI, 05 = Mech, 01 = Comp, 04 = IT, 42 = AIDS, 40 = EXCP, 50 = CSBS), *not* by trusting the folder it was found in. Three RAI papers were actually misfiled in the college archive under SY/Mech — the course codes `216U43C3xx` on the headers proved what they really were.
- **`SORTED_BY_SUBJECT/00_README - which paper is which.md`** documents every file: branch, scheme code, marks, quirks (KT papers are often 100-mark old-scheme; "objective" files are COVID-era Google-Form exports).
- The raw archive (2 extracted trees, ~2,200 files each, 2016 → 2025, all branches all semesters) stays local — too big for GitHub, and `SORTED_BY_SUBJECT/` already contains the 41 papers relevant to these five subjects.

### Paper naming you'll see everywhere

`MJ2025` = May–June 2025 exam window · `ND2025` = Nov–Dec 2025 window · `KT` = repeat-attempt paper (usually 100-mark, 3-hr, old scheme — different format, still useful for spotting recycled questions) · `PWD` = variant paper for differently-abled students.

---

## DOES IT ACTUALLY WORK? — the validation test

For each subject, a prediction was rebuilt using **only evidence that existed before** the target paper, then scored against the real paper, item by item (EXACT = same topic + same task format; TOPIC = right module, different angle; MISS = nothing covered it):

| Subject | Prediction basis | Result |
|---|---|---|
| CTO (Maths) | MJ-2025 → predict ND-2025 | 82% exact |
| HPS | MJ-2025 → predict ND-2025 | 77% exact |
| DSA | 2021 papers → predict MJ-2025 | 73% exact, 100% topic coverage |
| MoM | 2020+2021 papers → predict ND-2025 | 95% exact |
| MPR | syllabus + pattern only | 90% exact |
| **Overall** | **52 items tested** | **83% exact · 25/25 module-slot map** |

**The honest caveat (read it):** these are *reconstructed* blind predictions — the papers had already been read once during the original analysis, so some pattern knowledge could have leaked in. Scoring was kept mechanical (fixed rubric) to limit that, but treat 83% as "strong pattern," not "guaranteed." The full blow-by-blow, including every miss and why, is in `ESE_PREP/PREDICTION_VALIDATION.md`.

---

## REUSE THIS METHOD FOR YOUR OWN SUBJECTS

The pack is branch-specific; the method is not. If you have a folder of past papers, this is the recipe that was followed:

1. **Gather** every past paper you can get for the subject, from *any* branch of the same scheme that shares the course — sister-branch papers massively extend thin history for new branches.
2. **Verify branch & scheme from the paper header**, never from the folder name. Archives misfile papers constantly (3 found here). Note the programme code (branch) and course code (subject + scheme) printed on page 1.
3. **Read every paper fully** (text-extract the PDFs; OCR the scanned pages). Record, per question: module it came from, topic, task format (numerical / derivation / diagram / code), and marks.
4. **Build the slot map** — which module feeds which question number, and how marks are offered per module. Confirm it's stable across sessions (25/25 here).
5. **Find the archetypes** — group questions into recurring types and count frequencies across sessions. The high-frequency items are your Tier 1 predictions; items that rotate within a slot are Tier 2; never-asked syllabus items are Tier 3.
6. **Back-test before trusting it** — hide the newest paper, predict it from the older ones, score with a fixed rubric (EXACT / TOPIC / MISS). Only a back-tested prediction deserves confidence. Publish the misses too; they teach more than the hits.
7. **Generate the output pack**: question banks per module → 3 ranked sample papers per subject → answer keys with worked numbers → a visual revision guide → a study plan driven by the mark-weightage table and your own material gaps.

Steps 1–7 took one person + an AI agent about a week, evenings. The pattern-holding assumptions to re-verify for your college: fixed Q-structure, module→slot mapping, and archetype recycling. If your papers show a *changed* pattern (new scheme, post-COVID format shift), weight recent papers more heavily — old-format 100-mark KT papers were used here only as archetype evidence, never as format evidence.

---

## WHAT IS INTENTIONALLY *NOT* IN THIS REPO

- **The raw college archive** (2 trees × ~2,200 PDFs + two 1.3 GB zips, 2016→2025, every branch/semester) — GitHub blocks files over 100 MB, and 3 GB of unrelated papers helps nobody. The `.gitignore` keeps it out. If you want the raw archive, the 41 relevant papers are already in `SORTED_BY_SUBJECT/`, and the sorted README tells you exactly what exists beyond them.
- **`data-structures-using-c-2nd_reema_thareja (1).pdf`** (in the DSA study-material folder) — a copyrighted textbook. Do not republish it. If you clone this repo for the study-material folders, that file is on you to own legally. Everything in `ESE_PREP/` is original generated content.
- **College faculty slide decks** (the four subject folders: MMR, HPS, MPR, DSA) — these are lecturers' own material. They're excluded by the `.gitignore` out of respect for copyright; un-comment those lines if you have permission to share them.
- **Stray OCR artifacts** (`_ocr_*.png`) — working files from text-recovering a scanned page.

## DISCLAIMER

- This is a **study aid built from pattern analysis of public/legitimately-obtained past papers**. It contains no confidential or leaked exam material, and nothing here guarantees what will appear in any future paper — predictions are probabilities, back-tested but not infallible.
- Papers in `SORTED_BY_SUBJECT/` remain the property of the university that set them; they are shared here for study, in the spirit of every student-shared past-paper collection.
- The countdown plan embeds one real student's exam timetable — use it as a template, rebuild the dates for your own.

## LICENSE

Everything in `ESE_PREP/` (the generated analysis, banks, papers, keys, guides) — **MIT License**. Use it, fork it, improve it, pass your exams with it. The past papers in `SORTED_BY_SUBJECT/` and the syllabus PDF are included under fair-use study purposes and stay the property of their authors.

---

*Built November 2026 · 41 papers verified by header and sorted · 19 of them read end-to-end for pattern analysis · 52 predictions back-tested (83% exact). If this helped you, pay it forward: sort and verify your own college's archive and open-source it.*
