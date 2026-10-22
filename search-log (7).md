# Research Search Log — Member 01: Nguyen Dinh Quy

## Review objective

Identify empirical and methodological evidence on black-box test design, Equivalence Partitioning (EP), Boundary Value Analysis (BVA), Decision Table Testing, requirements coverage, test effectiveness, and student test-design studies. The review question asks whether students using an EP-BVA worksheet or a Decision-Table worksheet achieve higher item coverage across the same 20 frozen PURE functional requirements than the instructor reference inventory.

## Search sources and stored records

The current `01_all_records.csv` contains 151 records, all marked `source = search`:

| Source | Stored records | Recorded retrieval date |
|---|---:|---|
| Google Scholar | 133 | Not recorded in the CSV |
| Semantic Scholar | 18 | 2026-10-14 for all 18 rows |
| **Total** | **151** | — |

No rows are marked as backward or forward snowballing, and the `seed` field is blank for every record. The current member 01 dataset therefore has no record-level snowballing branch.

## Search query and audit trail

The project protocol defines this official String A:

```text
("black-box test design" OR "requirements-based testing" OR "user acceptance testing" OR PURE)
AND
("equivalence partitioning" OR "boundary value analysis" OR "decision table testing" OR "student experiment")
AND
("coverage item" OR "requirements coverage" OR "test coverage")
```

The `query` field is blank for all 151 records. The CSV therefore does not verify the exact query actually run in either source. It also does not record initial result counts, Google Scholar retrieval date, or a saved search-results screenshot. Treat String A as the protocol query, not as a verified execution log, until those search records are supplied.

## Record processing and screening

All 151 rows in `01_all_records.csv` were transferred into `02_after_screening_v1.csv`, retaining the source metadata and adding `v1_decision` and `v1_reason`. The V1 decisions currently recorded are:

| Decision | Count |
|---|---:|
| INCLUDE | 5 |
| EXCLUDE | 27 |
| UNSURE | 119 |
| **Total screened** | **151** |

The 27 V1 exclusions comprise EC1 = 3, EC2 = 1, EC3 = 2, EC6 = 11, and EC7 = 10. The 124 records marked INCLUDE or UNSURE are candidates for full-text assessment. A large portion of the Google Scholar records lack abstracts, so they remain UNSURE where the title alone is insufficient to assess method and outcome.

The current `03_final_included.csv` records two V2 includes: `SS001` and `SS084`. No V2 exclusions are recorded. The other 122 V1-retained candidates do not yet have a V2 decision in the member 01 files and remain pending. The evidence table summarizes the two recorded final includes as indirect background evidence; neither directly compares the two target worksheets on PURE.

## Source-level screening counts

| Source | V1 INCLUDE | V1 EXCLUDE | V1 UNSURE | Total |
|---|---:|---:|---:|---:|
| Semantic Scholar | 4 | 1 | 13 | 18 |
| Google Scholar | 1 | 26 | 106 | 133 |
| **Total** | **5** | **27** | **119** | **151** |

## Research question and relevance

The review uses the team’s inclusion and exclusion criteria IC1–IC7 and EC1–EC8. Studies involving EP, BVA, Decision Table Testing, or a closely related black-box test-design method may provide relevant evidence. Studies that do not evaluate students using the target worksheets on the same PURE requirements are background evidence rather than direct evidence for the RQ.

The two current final includes provide applied evidence about EP/BVA and Decision Table Testing, but do not answer which worksheet yields higher PURE item coverage. The review’s own experiment must supply that comparison.

## Data-quality notes

- `01_all_records.csv`: 151 records; 13 columns; 133 Google Scholar and 18 Semantic Scholar records.
- `02_after_screening_v1.csv`: 151 records; 15 columns; every row has a V1 decision and reason.
- `03_final_included.csv`: 2 records; 17 columns; both have `v2_decision = INCLUDE`.
- 125 of the 151 records have a blank abstract in `01`; those candidates need abstract/full-text retrieval before final exclusion or inclusion can be determined reliably.
- Search dates and exact executed queries are incomplete, as described above. Do not report the database-specific initial yield or claim a fully reproducible search until the missing audit data are recovered.
