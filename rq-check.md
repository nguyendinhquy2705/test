# SLR / RQ Check — Nguyễn Đình Quý (Member 1)

**Research question:** When designing black-box tests for 20 frozen functional requirements from PURE, do students using an EP-BVA worksheet or a Decision-Table worksheet achieve higher item coverage compared with the instructor reference inventory?

**Purpose:** Check whether the RQ has already been answered and record source-supported limitations. The P/I/C/O comparison below is about similarity to the exact RQ, not general topic similarity.

## 1. P/I/C/O reference

| Element | Target definition |
|---|---|
| P | Students designing black-box tests |
| I | Manual EP-BVA worksheet versus manual Decision-Table worksheet |
| C | The alternative worksheet, applied to the same task; instructor inventory is the scoring reference, not the intervention |
| O | Item coverage across the same 20 frozen PURE functional requirements, scored against the instructor reference inventory |

## 2. Paper-to-RQ comparison and limitations

| Paper | P match | I match | C match | O match | Highest match | Source-supported limitation / evidence | Quote and page status | Interpretation |
|---|---|---|---|---|---:|---|---|---|
| SS001 — *Implementation of Equivalence Partitioning and Boundary Value Analysis in Black Box Testing: A Case Study on the Admin Website of PAUD KB Al Husna* (2025), https://doi.org/10.36378/jtos.v8i2.5028 | No: one website case study, not a student experiment | Partial: EP and BVA, but not the target worksheet intervention | No | No: scenario pass/fail and validation defects, not PURE reference-item coverage | 1/4 direct; technique context only | One admin website and a manually designed test set; the available extraction identifies no student comparison, no instructor reference inventory, and no PURE requirement set. The existing extraction has an internal count inconsistency: 82 total scenarios, 27 failures, but also 45 passes. Do not report a pass rate until Table 3 is checked. | Exact author-stated limitation quote and page still need to be transcribed from the paper; do not present the team's interpretation as a quotation. | Background evidence for EP-BVA application; does not answer the RQ. |
| SS084 — *Pengujian Software Menggunakan Metode Boundary Value Analysis dan Decision Table Testing* (2021), https://openjournal.unpam.ac.id/index.php/ESIT/article/view/14827 | No: single pension-claim form, not a student experiment | Partial: uses BVA and Decision Table Testing, but not a controlled worksheet comparison | No | No: qualitative findings, not item coverage on PURE | 1/4 direct; technique context only | The extracted record describes one pension-claim form and qualitative findings that the form still needed improvement. No student worksheet comparison, shared PURE requirements, or instructor-reference coverage is documented in the extraction. | Exact author-stated limitation quote and page need to be verified from the article. If the paper does not state a limitation, record `Not stated`; do not infer a quotation. | Background evidence; does not answer the RQ. |
| E43 — Andleeb et al. (2025), *Enhancing Software Testing Education: Understanding Where Students Struggle*, https://arxiv.org/abs/2510.00957 | Yes: students in a software-testing course | No: automated feedback and test-suite revisions, not EP-BVA vs DT worksheets | Partial: tool uses a reference test suite, not alternative worksheet conditions | Partial: code coverage, not PURE item coverage | 2/4 (P and partial O/C) | The available paper text reports 46 students and focuses on ineffective revisions, decision coverage and exception handling. It does not compare the target worksheets or frozen PURE requirements. | Abstract/sections 3.1–3.3 should be cited in final source notes; exact limitation wording/page to be captured during full-text review. | Recent counter-evidence: student testing and reference-based feedback have been studied, but not the target comparison. |
| E44 — Ardic et al. (2026), *How students use generative AI for software testing: An observational study*, https://doi.org/10.1007/s10664-026-10898-0 | Yes: 12 undergraduate students | No: ChatGPT-assisted unit testing, not manual EP-BVA/DT worksheets | No target worksheet comparison | Partial: mutation score/test smells, not PURE item coverage | 1/4 direct plus adjacent student context | The paper's abstract reports an observational study of 12 students using GPT-3.5 and says interaction strategy/prompting style did not significantly affect mutation score or test smells. Task and outcome differ from the target RQ. | Springer article abstract, published 20 June 2026; full-text section and page to be recorded if a limitation is used as author-stated. | Strong recent student-testing study, but not a contradiction of the exact RQ gap. |
| E45 — *Identifying testing behaviour patterns in conceptual modelling education* (2026), https://doi.org/10.1016/j.infsof.2026.108279 | Likely relevant student/education context; exact sample to verify | No target worksheet intervention identified | No target worksheet comparison identified | Partial: testing behaviour/coverage in conceptual-model validation | Pending full-text coding | Available publisher search result reports three testing-behaviour patterns and a relationship between feedback integration and coverage. Exact population, metrics and limitations require full-text verification. | Do not use an author-stated limitation until the full text is inspected. | Recent adjacent paper; include in novelty comparison as provisional, not as a verified full-text inclusion. |

## 3. Personal conclusion: has the RQ already been studied?

No paper in the two Member 1 final-included records directly matches all four P/I/C/O elements. The three recent candidates are also adjacent rather than exact matches based on the currently inspected abstracts/metadata. E43 is the closest in population/reference-suite concept; E44 is close in student testing but uses AI-assisted unit testing and different outcomes. This supports a provisional claim that the exact RQ has not been identified in the examined set, not an absolute claim that no such paper exists.

**Highest similarity:** E43 has approximately 2/4 elements when partial overlap in reference-suite comparison/outcome is counted; no paper currently identified matches 3/4 or 4/4. Reconfirm this count during team-level coding using one consistent P/I/C/O rubric.

## 4. Initial gap statement — recordkeeping warning

**Provisional reconstruction:** Within the literature currently assembled, no identified study directly compares students using a manual EP-BVA worksheet with students using a manual Decision-Table worksheet on the same 20 frozen functional requirements from PURE, with item coverage scored against the same instructor reference inventory.

**Primary type:** GAP-T (the exact worksheet comparison has not been evaluated in the currently examined set). **Related scope difference:** GAP-D (the target PURE dataset and student task are not jointly represented in the identified studies). For counting, use one primary gap type per row; do not count this one statement as two separate strong gaps.

**Important:** The review instructions require the initial gap to be recorded before paper-level counting. If no dated pre-count statement exists, label this a reconstruction; do not backdate it or claim it was preregistered.

## 5. Why might this gap remain open?

Current evidence does not establish the reason. It could be a narrow combination of intervention, population, dataset and outcome rather than an overlooked general topic. Until stronger evidence is found, use: “The reason this exact comparison remains open has not been established in the literature examined.” Do not claim that the method is too expensive or that nobody has noticed it without evidence.

## 6. Personal actions still required

1. Open SS001 full text and resolve the inconsistent 82 / 45 / 27 scenario counts against Table 3; record exact table/page.
2. Open SS084 full text and record the actual evaluation method, metric, and any author-stated limitation. If none, record `Not stated`.
3. Add exact limitation quotations and page/section references to the individual evidence table; do not quote paraphrases.
4. Confirm the final full-text inclusion decisions are aligned with IC1–IC7 and EC1–EC8.
5. Give the team the P/I/C/O coding above and keep E43–E45 as recent novelty-check candidates until full-text decisions are complete.

**Status:** Personal RQ check drafted; exact source quotations and the SS001 count discrepancy remain verification tasks.
