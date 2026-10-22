# Evidence Table Quality Audit (RBL-1 five gates)

**Audit date:** 2026-10-22  
**Source:** `team-synthesis/evidence-table-merged.md` in the supplied ZIP.  
**Scope:** Mechanical checks of the existing merged table plus source-verification issues visible in the files. This is not a substitute for reading original full texts.

## Five-gate status

| Gate | Rule | Current check | Status | Required action |
|---|---|---|---|---|
| P1 | At least 12 papers included in the merged evidence base | Current member files yield 37 final INCLUDE rows and 37 team-deduplicated records in `03_final_included_team.csv`. A title-based reconciliation found 21 of those records match a merged evidence-table row by the current exact/substring check; remaining records require manual ID/title mapping. The numerical threshold of 12 is met in the team include file, but table-to-CSV reconciliation is incomplete. | **Count threshold passes; reconciliation incomplete** | Map each of the 37 include records to the merged evidence table or document why it is not in the table. Keep the included count and evidence-row count separate. |
| P2 | Tool/LLM has data in ≥90% of rows | 42 rows; 41 contain a tool/approach value other than `N/S` (97.6%). Explicit `N/S` is an acceptable honest value but does not identify a tool. | **Pass for field completeness; content verification remains** | Check that names are accurate and not inferred from titles. Keep `Not reported` when the source is silent. |
| P3 | Result column has a number in ≥50% of rows | 42 rows require at least 21 with verified numerical results. The current extraction includes `N/A` in 22 rows and `†` flags for results whose original Table/Figure is not recorded; the gate cannot be called passed until at least 21 results are verified. | **Not yet demonstrated** | Verify all `†` entries against original tables/figures; count only supported numeric results. Replace unsupported numbers with `N/A`. |
| P4 | Limitation column has data in ≥50% of rows | All 42 rows have text in the limitation column, but some entries include team interpretation or claims that another paper “partly addresses” a limitation. | **Text-complete, source validation pending** | For each row distinguish `Author-stated limitation` from `Team interpretation`; record exact quotation and section/page where available. If no limitation is stated, use `Not stated`. |
| P5 | Metric is specific, not generic “accuracy” | All 42 rows have a metric description, but some are broad or need a formula/operational definition. | **Partial** | Give each metric a name, unit, numerator/denominator or calculation, and source table/figure. Do not equate code coverage, fault detection, test count, and PURE item coverage. |

## Concrete integrity issue

Member 1's SS001 extraction reports 82 total scenarios, 45 passed, and 27 failed, while also reporting a 67.1% success rate. These values do not reconcile arithmetically: 45/82 is not 67.1%, and 45 + 27 is 72. The paper's 27/82 failure figure corresponds to approximately 32.9%, but the pass count must be checked against the original Table 3. The merged evidence table must not state a definitive pass count or success rate until that discrepancy is resolved.

## Mechanical counts from the current merged table

- Extracted evidence rows: 42.
- Tool/approach not marked `N/S`: 41/42 = 97.6%.
- Result rows containing `N/A`: 22/42. This does not itself determine the numerical-result pass count because some remaining values are qualitative or marked `†`.
- Limitation cells with text: 42/42; source support is not yet established for every cell.
- Metric cells with text: 42/42; specificity needs row-by-row verification.

**Current overall decision:** Do not mark all five gates passed yet. P1 meets the numerical threshold in the team include CSV but still needs row mapping; P2 passes mechanically; P3 is unproven; P4 and P5 need source-level quality checks.
