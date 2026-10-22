# RQ Validation — Team Synthesis (Week 7)

**Status:** Working validation document. It is complete as an audit structure, but the group must not mark source-verification and feasibility items as passed until the stated checks are actually performed.

## 1. Research Question and PICO

**RQ:** When designing black-box tests for 20 frozen functional requirements from PURE, do students using an EP-BVA worksheet or a Decision-Table worksheet achieve higher item coverage compared with the instructor reference inventory?

| Element | Operational definition | Validation note |
|---|---|---|
| P | Students who design black-box tests for functional requirements | Define course/level, inclusion criteria, and participant recruitment in the experiment protocol. |
| I | Manual EP-BVA worksheet and manual Decision-Table worksheet | The worksheets must be frozen and have parallel instructions/time limits. |
| C | The alternative worksheet condition | The instructor reference inventory is the scoring reference for O, not itself a worksheet intervention. |
| O | Item coverage across the same 20 frozen PURE functional requirements | Define item unit, numerator, denominator, handling of partial/duplicate items, and scoring rubric before data collection. |

## 2. Three required questions

### Q1. Has a paper already answered the exact RQ?

**Current answer:** No exact 4/4 P/I/C/O match has been identified in the current merged evidence map. The closest student study is E41, which evaluates EP, branch testing, and code reading with students on three C programs; it does not compare the two target worksheets, use PURE requirements, or measure item coverage against the instructor inventory. Recent adjacent studies E43–E45 also do not match the complete RQ based on the currently inspected metadata/abstracts.

**Scope qualifier:** “Not identified in the literature examined so far,” not “nobody has ever done it.” Complete the final full-text and recent-paper checks before locking this conclusion.

### Q2. What was the initial gap?

**Initial gap statement (provisional reconstruction if no dated pre-count record exists):** Within the literature currently assembled by the team, no identified study directly compares students using a manual EP-BVA worksheet with students using a manual Decision-Table worksheet to design black-box tests for the same 20 frozen functional requirements from PURE, with item coverage assessed against the same instructor reference inventory.

**Primary type:** GAP-T — the exact worksheet comparison has not been evaluated in the currently examined set.

**Related scope dimension:** The target PURE requirement set and common instructor-reference outcome make the context specific, but do not count this as a second independent gap unless a separate measurable RQ is justified.

**Recordkeeping warning:** The instructor requires the initial gap to be recorded before paper counting. If the group did not preserve a dated pre-count statement, label this a reconstruction. Do not backdate it or claim preregistration.

### Q3. Is the gap strong or weak, and why does it remain open?

**Current answer:** The exact-comparison gap is a provisional novelty observation, not yet a “strong gap” under the rule that ≥3 independent papers explicitly report the same limitation. The current evidence does not provide enough exact limitation quotations and page references to count G01 as a strong frequency-based gap.

**Why it may remain open:** Not established within the literature examined. Do not speculate that it is too expensive, overlooked, or ineffective without evidence. Check the nearest papers' Limitations/Threats to Validity/Future Work and run a targeted search for negative results before making a causal explanation.

## 3. Counter-evidence and novelty label

| Candidate | Closest P/I/C/O elements | Why it does not answer the exact RQ | Status |
|---|---|---|---|
| E41 — Comparing the Effectiveness of Equivalence Partitioning, Branch Testing and Code Reading by Stepwise Abstraction Applied by Subjects (2012) | P = students; I = manual EP among techniques | Different intervention comparison, three C programs, defect-revelation outcome; no PURE/reference inventory | Closest in student + EP context; not exact |
| E43 — Enhancing Software Testing Education: Understanding Where Students Struggle (2025) | P = students; partial O/C = coverage and a reference test suite | Focuses on automated feedback and ineffective revisions, not EP-BVA vs DT worksheets or PURE | Recent near-RQ evidence |
| E44 — How students use generative AI for software testing (2026) | P = students; O adjacent = mutation score/test smells | ChatGPT-assisted unit testing, not manual black-box worksheet comparison; no PURE item coverage | Recent near-RQ evidence |
| E45 — Identifying testing behaviour patterns in conceptual modelling education (2026) | Student testing/coverage context | Conceptual-model validation and no identified target worksheet comparison; full text still needed | Provisional recent candidate |

**Novelty label:** Provisional `extension` (preferred working label) if the team frames the study as extending existing student test-design/coverage research to a new worksheet comparison and frozen PURE inventory. Use `new` only if the registration card defines novelty that way and the final search supports it. Do not call it `replication` unless a paper matches all four P/I/C/O elements. Confirm against the RQ registration card and tell the instructor if the label differs.

## 4. GapList decisions

See `team-synthesis/gaplist.md` for the separate rows G01–G05. Current decision:

- G01 remains the candidate central gap.
- G02 (specific PURE/student scope) and G03 (exact outcome) are best treated as dimensions that specify G01, not automatically separate strong gaps.
- G04 (automation/model dependence) is not central because applied manual testing evidence exists.
- G05 (single-system context) is too general and may be resolved by broader studies.
- No gap receives a “strong” label by frequency until exact author limitation quotations, page numbers, independent-paper counts, and resolver checks are complete.

## 5. Nearest-paper alignment table

| Element | Nearest student paper E41 | Team RQ | Difference and evidence |
|---|---|---|---|
| P | Students/subjects | Students designing black-box tests | Broadly aligned population |
| I | EP, branch testing, and code reading | Manual EP-BVA worksheet vs manual Decision-Table worksheet | Different technique comparison and worksheet operationalization |
| C | Branch testing and code reading are comparison techniques | Alternative worksheet condition | Different comparison |
| O | Defect-revelation effectiveness | Item coverage against instructor inventory across 20 PURE requirements | Different outcome and benchmark |
| Dataset | Three C programs | 20 frozen functional requirements from PURE | Different unit of analysis/context |

**Closest paper conclusion:** E41 is the closest in student participation and EP, but the RQ differs on I, C, O, and dataset context. This supports an `extension` working label, subject to final registration-card check. It does not by itself prove a strong literature gap.

## 6. Feasibility — Part A: Is the RQ statistically testable?

| Criterion | Current proposed approach | Status / required action |
|---|---|---|
| Metric | `Item coverage (%) = 100 × number of reference inventory items covered by a student's test design / total number of applicable reference inventory items` | **Needs action:** specify how partial matches, duplicates, invalid items, and ambiguous requirements are scored. Freeze rubric before scoring. |
| Comparison | Each participant completes one assigned worksheet condition; if within-subject, counterbalance order and avoid reusing the same requirements in both conditions without a carryover plan | **Needs action:** confirm actual design with instructor. Do not claim a paired design until both conditions are genuinely observed per participant. |
| H0/H1 | H0: no difference in item-coverage scores between EP-BVA and Decision-Table conditions. H1: item-coverage scores differ between conditions. | **Provisional:** select independent or paired test based on the actual assignment design. |
| Test | If same students produce both scores: paired Wilcoxon signed-rank (or paired t-test only if assumptions justify it). If different student groups: Mann–Whitney U (or independent t-test if assumptions justify it). | **Needs action:** specify one primary analysis before collecting results. |
| Effect threshold | Not yet provided in the supplied project files | **A / needs action:** define a practically meaningful difference and cite rationale; do not invent a threshold after observing results. |
| Sample size | Not established in supplied files | **A / needs action:** determine N using the selected test/effect size, or explicitly label the study exploratory if N is insufficient. |
| Scoring reliability | Two independent raters on a pilot subset; report agreement and resolve rubric disagreements | **Needs action:** define pilot size and agreement measure; record resolution process. |

**Part A current decision:** No fatal X is established from the files alone, but the design is not ready to lock because the metric rubric, assignment design, effect threshold, and sample-size rationale are not fully documented. These are A/needs-action items, not passes.

## 7. Feasibility — Part B: Are resources sufficient?

| Resource | Current evidence | Status / action |
|---|---|---|
| Dataset | Team states 20 frozen PURE requirements; exact frozen file/path not confirmed in this ZIP | **A:** link/hash the frozen requirement file and reference inventory. |
| Reference inventory / ground truth | Instructor reference inventory is part of the RQ, but no actual inventory file is in the ZIP | **A:** obtain and freeze it; without it, item coverage cannot be scored. |
| Worksheet artifacts | RQ specifies EP-BVA and Decision-Table worksheets; final worksheet files not in this ZIP | **A:** create/freeze both worksheets and parallel instructions. |
| Tool/API | Manual worksheet study does not inherently require paid API | **Safe provisionally:** document software used for data collection/scoring if any. |
| Computing | Ordinary spreadsheet or small script should suffice for 20-item coverage scoring | **Safe provisionally:** validate scoring calculation on a pilot. |
| Raters / skills | Two raters are desirable for reliability; actual team assignment not documented | **A:** assign raters and time budget. |
| Time | Remaining schedule not included | **A:** record actual hours/dates and leave >3 days buffer if possible. |

**Part B current decision:** No documented hard X yet, but several resources are unconfirmed. Do not mark “safe” until the requirements, reference inventory, worksheets, raters, and schedule are available.

## 8. Four team conclusions

1. **Exact-RQ counter-evidence:** No exact 4/4 P/I/C/O paper has been identified in the current evidence set. This is a bounded conclusion pending final screening and recent-paper verification.
2. **Nearest study:** E41 is nearest in student participation and EP, but differs in intervention comparison, outcome, and dataset. Recent E43–E45 study adjacent student-testing/coverage questions but do not answer the exact worksheet/PURE comparison based on currently inspected evidence.
3. **Gap strength:** G01 is the most defensible candidate central gap, but it is not yet a strong frequency-based gap because exact limitation quotations and a ≥3-paper independent count are not verified. State it as a bounded novelty observation for now.
4. **Feasibility:** Keep the RQ provisionally; before lock, freeze the 20 requirements, instructor reference inventory and worksheets, define the scoring rubric, choose the analysis from the actual experimental design, and justify N/effect threshold. Report any RQ change to the instructor before lock.

## 9. Completion checklist

- [ ] Evidence table has ≥12 final included records, with final inclusion decisions reconciled to `03_final_included_team.csv`.
- [ ] Tool/LLM populated or explicitly `Not reported` in ≥90% of merged rows.
- [ ] ≥50% of rows contain source-verified numerical results when available; all `†` claims checked against tables/figures.
- [ ] ≥50% of rows contain source-supported limitation data or explicitly `Not stated`.
- [ ] Every row has a specific metric and definition.
- [ ] Each member has completed `SLR/rq-check.md` with P/I/C/O, limitation quotation, section/page, and conclusion.
- [ ] Three recent papers checked; exact query/date and selection rationale recorded.
- [ ] Gap counts use independent studies and source quotations; resolver check complete.
- [ ] Novelty label matches the registration card and nearest-paper alignment.
- [ ] Part A and Part B have actual numeric values and no unresolved X; all A items have action plans.
- [ ] PRISMA counts match the reconciled CSV; no pending decisions are silently counted as exclusions or inclusions.
- [ ] Any RQ change has been reported to the instructor before the lock.
