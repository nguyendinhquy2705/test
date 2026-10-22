# PRISMA Flow — Member 01

> **Counting basis:** Counts below are computed from the current `01_all_records.csv`, `02_after_screening_v1.csv`, and `03_final_included.csv`. All records in `01` have `source = search`; no snowballing records are present.

## Study selection

```text
Records identified in 01_all_records.csv                         151
  Google Scholar                                                   133
  Semantic Scholar                                                  18

Records screened at title/abstract stage                          151
Records excluded at V1                                               27
  Duplicate records (EC7)                                            10
  Other V1 exclusions (EC1/EC2/EC3/EC6)                              17
Records retained for full-text assessment (5 INCLUDE + 119 UNSURE) 124

Final inclusion decisions recorded at V2                              2
  Included in 03_final_included.csv                                   2
  V2 decisions still pending                                         122
Full-text exclusions recorded at V2                                    0
```

## Flow equations

```text
151 screened − 27 excluded at V1 = 124 retained for full-text assessment
124 retained − 2 final includes = 122 candidates without a recorded V2 decision
```

The two V2 includes are `SS001` and `SS084`. The current `03_final_included.csv` contains included records only; it does not contain V2 decisions for the other 122 candidates. No V2 exclusions are recorded, so those candidates are pending rather than excluded.

## Screening counts

| Stage/decision | Count | Source |
|---|---:|---|
| Records in search set | 151 | `01_all_records.csv` |
| Title/abstract EXCLUDE | 27 | `02_after_screening_v1.csv` |
| Title/abstract INCLUDE | 5 | `02_after_screening_v1.csv` |
| Title/abstract UNSURE | 119 | `02_after_screening_v1.csv` |
| Retained for V2 (INCLUDE + UNSURE) | 124 | `02_after_screening_v1.csv` |
| Final V2 INCLUDE | 2 | `03_final_included.csv` |
| V2 decisions pending | 122 | Retained at V1 minus recorded V2 includes |
| V2 EXCLUDE recorded | 0 | `03_final_included.csv` |

V1 exclusions by primary reason: EC1 = 3, EC2 = 1, EC3 = 2, EC6 = 11, and EC7 = 10 (total = 27).

## Search source breakdown

| Database | Records in `01` | V1 EXCLUDE | V1 INCLUDE | V1 UNSURE |
|---|---:|---:|---:|---:|
| Google Scholar | 133 | 26 | 1 | 106 |
| Semantic Scholar | 18 | 1 | 4 | 13 |
| **Total** | **151** | **27** | **5** | **119** |

## Data status

The flow is not complete: 122 records retained at V1 do not yet have a recorded V2 decision. Update the PRISMA counts after those records receive full-text decisions. The current final included count of 2 reflects only the V2 includes already recorded in `03_final_included.csv`.
