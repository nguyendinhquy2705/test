# GapList — Team Candidate Gaps

**Target RQ:** When designing black-box tests for 20 frozen functional requirements from PURE, do students using an EP-BVA worksheet or a Decision-Table worksheet achieve higher item coverage compared with the instructor reference inventory?

## Gap-counting rules

- Count a paper only when the same paper supports the same specific limitation; do not combine claims from different papers.
- Count distinct studies, not duplicate records or multiple versions of one study.
- A strong gap requires at least 3 independent papers explicitly naming the same limitation, after checking whether another paper in the examined set resolves it.
- A weak gap has 1–2 such papers.
- A gap inferred by the team but not stated in a paper is a team hypothesis, not a paper-supported limitation.
- Every limitation used in a final gap statement needs an exact quotation and section/page. If no limitation is stated, write `Not stated`.
- Current counts below are deliberately marked unverified where the ZIP does not contain enough source quotations. Do not replace these with guessed counts.

## GapList

| ID | Specific proposed gap | Type | Paper evidence currently available | Papers that may resolve it | Verified remaining count | Strength | Decision |
|---|---|---|---|---|---:|---|---|
| G01 | No identified study directly compares manual EP-BVA and Decision-Table worksheets for students on the same frozen 20 PURE requirements using item coverage scored against one instructor reference inventory. | GAP-T (primary); dataset scope can be noted as context but not double-counted as another gap | RQ evidence map identifies E41 as the only student-participant paper in the merged set; it studies EP vs branch testing/code reading on C programs. Recent E43–E45 are adjacent, not exact matches based on inspected abstracts/metadata. | No exact resolver identified in the current set; full-text verification and consistent PICO coding remain required. | Not yet countable as a limitation-frequency gap; currently a bounded novelty observation | Candidate central gap; not yet “strong” by limitation count | Retain provisionally; confirm after all records are screened and recent papers are full-text checked. |
| G02 | The target task combines student worksheet choice with a fixed requirement inventory and a common item-coverage score. | GAP-D (scope/dataset) | No identified paper in the current map uses the same 20 PURE requirements and scoring inventory. | No exact resolver identified so far. | Not yet countable | Candidate scope gap; strength not established | Treat as a defining condition of G01, not a second gap unless evidence and RQ justify it. |
| G03 | Existing papers report heterogeneous outcomes such as fault detection, mutation score, test-case counts, code coverage, or qualitative feedback rather than the team's exact item-coverage outcome. | GAP-M (outcome) | The merged evidence map explicitly states that generic coverage, fault detection, or test effectiveness is not the same as PURE item coverage. | Recent student studies use code coverage or mutation score but not this exact outcome. | Not a verified frequency count of author-stated limitations | Candidate outcome gap; currently a synthesis observation | Retain as an explanatory dimension of G01, not a separate strong gap until limitations are sourced. |
| G04 | Some methods rely on automation, LLMs, or formalized input models rather than a manual student worksheet. | GAP-T (method condition) | Many merged papers investigate tools or automated generation, while E41 uses manual EP but not the target comparison. | Manual EP/BVA application studies partially address the general automation-only limitation, but not the target worksheet comparison. | Not countable without exact limitation coding | Weak as a standalone gap; not a direct limitation of the exact RQ | Do not use as the central gap. |
| G05 | Some evidence comes from one system or narrow case-study settings. | GAP-D | Several application studies use one website, form, system, or test object. | Other papers use multiple applications or broader surveys, so the general “single case” limitation may already be addressed by other evidence. | Not countable until each claim is verified and resolved | Likely weak/overgeneralized as currently worded | Do not use as central gap; split into specific dataset limitations only when relevant. |

## Provisional gap statement for the current RQ

“Within the literature examined by the team, no identified study directly compares students using manual EP-BVA and Decision-Table worksheets on the same 20 frozen PURE functional requirements, with item coverage scored against the same instructor reference inventory.”

This is a *scope-bounded novelty statement*, not a strong-gap-by-frequency statement. Do not write “x of N papers explicitly reported this limitation” until the source quotations and denominator have been audited.

## Why this gap may remain open

The reason is not established by the current evidence. The team has not yet identified a source-supported explanation such as cost, lack of ground truth, or a failed prior attempt. Use “not established within the literature examined” until a targeted negative-result search and the limitations sections of near-RQ papers have been checked.

## Gap decision

- Keep the current RQ as a candidate while feasibility is tested.
- Do not claim the gap is strong solely because no exact paper was found.
- Do not change the RQ to a different gap unless the team has a stronger evidence-backed gap and reports the proposed change to the instructor before lock.
