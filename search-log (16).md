# SEARCH LOG - MEMBER 3 (IEEE XPLORE)

> **Current search run (2026-10-15):** The revised search below supersedes the earlier IEEE-01/IEEE-02 run for new screening work. The earlier run and IEEE-03 remain retained for audit only and must not be combined with this revised record set.

## IEEE-R1 — Revised Official String A (P/I/O)

### Exact query

```text
("black-box test design" OR "requirements-based testing" OR
 "functional testing" OR "user acceptance testing" OR
 "test case generation")
AND
("equivalence partitioning" OR "boundary value analysis" OR
 "decision table testing")
AND
("test coverage" OR "requirements coverage" OR
 "test effectiveness" OR "test case quality")
```

- Search date: 2026-10-15
- Search field: All (default IEEE Xplore search field)
- Filters: None
- Results returned: 5
- Evidence screenshot: not yet available in the submission folder; recapture the revised P/I/O page showing 5 results before submission.
- Adaptation: Fewer than 20 records; the Outcome block was removed under the protocol's too-few-results rule.

## IEEE-R2 — Revised Expanded Search (P/I)

### Exact query

```text
("black-box test design" OR "requirements-based testing" OR
 "functional testing" OR "user acceptance testing" OR
 "test case generation")
AND
("equivalence partitioning" OR "boundary value analysis" OR
 "decision table testing")
```

- Search date: 2026-10-15
- Search field: All (default IEEE Xplore search field)
- Filters: None
- Results returned: 40
- Export raw was normalized into `01_all_records.csv` for submission.
- Exported from Zotero: 39 records. The remaining platform hit was the Packt book *Software Test Design*; it is recorded as IEEE040 and excluded at title/abstract screening under EC6.
- Deduplication: No duplicate DOI or title groups among the 39 Zotero records.
- Evidence screenshot: `screenshots/IEEE_R2_revised_PI_40_results.png`
- Screening file: `screening-v1-revised.md`
- Full-text screening: `fulltext-screening-revised.csv` — 25 assessed; 23 excluded (EC8) and 2 included.
- Snowballing: `snowballing-log.md` — one backward and one forward discovery round from seed IEEE020; no candidate added without full-text verification.

---

## Research Topic

Comparing EP-BVA and Decision-Table Worksheets for Student Test Design on PURE

## Reviewer Information

- Reviewer: Member 3
- Database: IEEE Xplore
- Search mode: Command Search
- Search field: All (default IEEE Xplore search field)
- Search date: 2026-10-08
- Protocol: team-synthesis/protocol.md
- Criteria: team-synthesis/ie_criteria.md

---

## IEEE-01 - Official Search String A

### Official Query

("black-box test design" OR "requirements-based testing" OR "user acceptance testing" OR PURE)
AND
("equivalence partitioning" OR "boundary value analysis" OR "decision table testing" OR "student experiment")
AND
("coverage item" OR "requirements coverage" OR "test coverage")

### IEEE Search Query

(("black-box test design" OR "requirements-based testing" OR "user acceptance testing" OR PURE)
AND
("equivalence partitioning" OR "boundary value analysis" OR "decision table testing" OR "student experiment")
AND
("coverage item" OR "requirements coverage" OR "test coverage"))

- Results returned: 0
- Filters: None
- Screenshot: screenshots/IEEE_StringA_original_0results.png
- Search URL: https://ieeexplore.ieee.org/search/searchresult.jsp?action=search&matchBoolean=true&newsearch=true&queryText=((%22black-box%20test%20design%22%20OR%20%22requirements-based%20testing%22%20OR%20%22user%20acceptance%20testing%22%20OR%20PURE)%20AND%20(%22equivalence%20partitioning%22%20OR%20%22boundary%20value%20analysis%22%20OR%20%22decision%20table%20testing%22%20OR%20%22student%20experiment%22)%20AND%20(%22coverage%20item%22%20OR%20%22requirements%20coverage%22%20OR%20%22test%20coverage%22))
- Notes: No results found using the official P/I/O search string.

---

## IEEE-02 - Search String A Without Outcome Block

### Exact Query

("black-box test design" OR "requirements-based testing" OR "user acceptance testing" OR PURE)
AND
("equivalence partitioning" OR "boundary value analysis" OR "decision table testing" OR "student experiment")

- Results returned: 1
- Filters: None
- Reason for adaptation: IEEE-01 returned fewer than 20 results. Outcome block removed according to Review Protocol.
- Screenshot: screenshots/IEEE_StringA_without_O_results.png
- Search URL: https://ieeexplore.ieee.org/search/searchresult.jsp?action=search&matchBoolean=true&newsearch=true&queryText=((%22black-box%20test%20design%22%20OR%20%22requirements-based%20testing%22%20OR%20%22user%20acceptance%20testing%22%20OR%20PURE)%20AND%20(%22equivalence%20partitioning%22%20OR%20%22boundary%20value%20analysis%22%20OR%20%22decision%20table%20testing%22%20OR%20%22student%20experiment%22))

### Candidate Record

- Record ID: IEEE001
- Title: Combinatorial Test Suites Generation Strategy Utilizing the Whale Optimization Algorithm
- Authors: Ali Abdullah Hassan; Salwani Abdullah; Kamal Z. Zamli; Rozilawati Razali
- Year: 2020
- Venue: IEEE Access, Volume 8, pp. 192288-192303
- DOI: 10.1109/ACCESS.2020.3032851
- URL: https://ieeexplore.ieee.org/document/9234407/
- Title/Abstract Screening: UNSURE
- Full-text Screening: EXCLUDE (EC3)
- Reason: Focuses on WOA-based combinatorial t-way test generation, not direct EP-BVA or Decision Table test design.

---

## IEEE-03 - Supplementary Search

### Exact Query

("All Metadata":"equivalence partitioning" OR "All Metadata":"boundary value analysis" OR "All Metadata":"decision table testing")

- Results returned: 102
- Results displayed per page: 25
- Filters: None
- Screenshot: screenshots/IEEE_03_supplementary_results.png
- Search URL: https://ieeexplore.ieee.org/search/searchresult.jsp?action=search&matchBoolean=true&newsearch=true&queryText=((%22All%20Metadata%22:%22equivalence%20partitioning%22%20OR%20%22All%20Metadata%22:%22boundary%20value%20analysis%22%20OR%20%22All%20Metadata%22:%22decision%20table%20testing%22))
- Reason for expansion: Official String A returned 0 records; removing Outcome returned only 1. Supplementary search focuses on relevant black-box test design techniques.
- Protocol status: Exploratory only; not part of the primary protocol search.
- Exported records: Not exported.
- Screening: Not performed for the primary evidence set.

Important: IEEE-03 removes the P and O blocks. The frozen protocol permits removal of the Outcome block only when a search has fewer than 20 records; therefore IEEE-03 is retained only as an exploratory logged search and is not eligible for the official record set, screening, Evidence Table, or PRISMA counts without a documented protocol amendment.

---

## Export Summary

| Search ID | Search Results | Exported Records | Status |
|---|---:|---:|---|
| IEEE-01 | 0 | 0 | Completed |
| IEEE-02 | 1 | 1 manually recorded | Completed |
| IEEE-03 | 102 | 0 | Exploratory only; not eligible for official data |

---

## Screening Summary

- IEEE001: Round 1 UNSURE; Round 2 EXCLUDE (EC3)
- IEEE-03 records: Not screened because the query is outside the frozen search-modification rule
- Final included studies: 0

---

## Snowballing

- Seed paper: Not applicable — no included study is available for seed selection.
- Seed DOI: Not applicable.
- Citation count: Not applicable.
- Backward records: Not performed.
- Forward records: Not performed.
- New included papers: 0

---

## Notes

1. All search counts are based on IEEE Xplore results.
2. IEEE-03 is an exploratory supplementary search outside the primary protocol search.
3. All included papers must satisfy the official IC/EC criteria.
4. PRISMA counts are finalized for Member 3's personal IEEE dataset: one stored record, no duplicates, one full-text exclusion (EC3), and zero included studies.
