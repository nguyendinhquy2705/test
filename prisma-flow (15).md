# PRISMA Flow — Member 3 (IEEE Xplore)

> **Status: final for the available IEEE full-text corpus, 2026-10-19.** This file uses only the revised search run (`IEEE-R1`/`IEEE-R2`) in `search-log.md`. Earlier IEEE-01/IEEE-02/IEEE-03 entries are retained in the log for audit only and are not combined with these counts.

## Identification and Title/Abstract Screening

| Measure | Count | Evidence |
| --- | ---: | --- |
| Records identified by revised P/I/O search | 5 | `search-log.md` — IEEE-R1 |
| Records identified by revised P/I expanded search | 40 | `search-log.md` — IEEE-R2 |
| Records carried forward | 40 | P/I supersets P/I/O; do not add the 5 results again |
| Duplicate records removed | 0 | No duplicate DOI or title group among the 39 Zotero records |
| Records screened at title/abstract | 40 | `02_after_screening_v1.csv` |
| Excluded at title/abstract | 15 | EC1=3; EC2=3; EC3=7; EC6=2 |
| Reports awaiting full-text assessment | 0 | All 25 title/abstract `UNSURE` records received a documented round-2 decision |

## Full-text Screening and Snowballing

| Measure | Count |
| --- | ---: |
| Full-text reports assessed | 25 |
| Full-text exclusions | 23 |
| Final included from IEEE Xplore | 2 |
| Backward-snowballing records | 0 |
| Forward-snowballing records | 0 |

Seed selected: **IEEE020** — *Comparing the Effectiveness of Equivalence Partitioning, Branch Testing and Code Reading by Stepwise Abstraction Applied by Subjects* (DOI `10.1109/ICST.2012.113`). Its OpenAlex citation count is 30, within the team seed criterion of 10–200. One backward and one forward snowballing discovery round are recorded in `snowballing-log.md`: 61 backward and 30 forward candidates, with zero added because no candidate full text was retrieved and verified.

## Numerical Check

```text
40 title/abstract records = 15 excluded + 25 full-text assessments
25 full-text assessments = 23 EC8 exclusions + 2 included
```

## Required Next Steps

1. Obtain lawful full-text access for the 25 `UNSURE` records.
2. Record a final `INCLUDE` or `EXCLUDE` decision with a primary EC code for each full text.
3. If an `INCLUDE` is available, select one seed and log one backward plus one forward snowballing round.
4. Extract Table/Figure evidence only for final `INCLUDE` studies, then update all counts above.
