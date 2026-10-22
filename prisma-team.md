# PRISMA Flow — Team Reconciliation Audit

**Audit date:** 2026-10-22  
**Status:** Provisional reconciliation. Member-specific screening exports have different search populations and stages. Counts below must not be summed into a single PRISMA diagram until every record is assigned to one deduplicated team record and one final decision.

## Member-level counts available in supplied files

| Member | Raw records | Title/abstract decision counts | Full-text / final decisions | Pending / integrity issue |
|---|---:|---|---|---|
| M1 — Nguyễn Đình Quý | 151 | 27 EXCLUDE, 5 INCLUDE, 119 UNSURE | 2 V2 INCLUDE in `03_final_included.csv` | 122 records carried forward without a V2 decision; no snowball records in raw CSV. |
| M2 — Phan Trọng Nguyên | 97 | 10 EXCLUDE, 11 INCLUDE, 76 UNSURE | 26 V2 INCLUDE in `03_final_included.csv` | Search log says 51 ACM results and 19 preliminarily filtered, while raw file has 97 records; document how the 97-row set was constructed. |
| M3 — Hoàng Văn Tài | 40 revised IEEE records | 15 EXCLUDE, 25 UNSURE | 23 full-text EXCLUDE and 2 INCLUDE in `fulltext-screening-revised.csv` | Older search runs are retained for audit and must not be added to the revised run. Snowballing found no verified additions. |
| M4 — Trần Thiên Mỹ | 122 raw records | 14 screened in current `02.screening.csv`: 5 first-stage EXCLUDE, 9 carried to full text | 7 final INCLUDE, 2 final EXCLUDE among the 14 screened | 108 records have no recorded screening decision. Original screening CSV had a blank first line and extra empty columns; normalized file is saved in the same path. |

## Team include-record reconciliation

A normalized team file `03_final_included_team.csv` has been created from the member-specific final-included records and the seven explicit M4 final INCLUDE decisions. It preserves the source member and local record IDs, applies title/DOI-based deduplication, and should be used as the starting point for the final team include count.

**Do not assume that the number of rows in the merged evidence table equals the PRISMA included count.** Each included study must map to a final record ID and each excluded full-text study must have one primary EC1–EC8 reason.

## Flow accounting rules

1. Use only the current revised search run for each database; earlier search runs remain audit-only.
2. Keep records from primary databases (IEEE Xplore, ACM Digital Library, OpenAlex) separate from Google Scholar/Semantic Scholar seed and snowballing records as specified in the protocol.
3. Deduplicate using DOI first, then normalized title, authors, and year. Preserve all source record IDs in the deduplication log.
4. A V1 `UNSURE` is not an INCLUDE. It must have a full-text decision or remain pending.
5. A final INCLUDE must satisfy IC1–IC7 and have a documented reason; background relevance alone must be justified against the protocol.
6. Each full-text EXCLUDE must have one primary EC1–EC8 reason.
7. Snowballing candidates without a verified source/full text are not included.
8. The final PRISMA diagram must reconcile exactly with the canonical team CSV and the final-included CSV.

## Current conclusion

The supplied files show more than 12 recorded member-level INCLUDE decisions before reconciliation, but the final team PRISMA count should be copied from `03_final_included_team.csv` only after the team validates relevance and duplicate handling. M1 and M4 still have substantial pending screening populations. The PRISMA flow is not fully closed until those pending records are screened or explicitly excluded according to the protocol.
