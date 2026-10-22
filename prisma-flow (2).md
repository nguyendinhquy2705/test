[Uploading prisma_flow.md…]()

# PRISMA Flow

> **Counting rule:** The main screening flow uses records with `source = search`. The snowballing branch uses records with `source` beginning with `snowball-`. The final included count is the sum of the main search branch and the snowballing branch.
>
> **Data limitation:** `01_all_recors.csv` has 122 records, all with `source = search` (database = OpenAlex, `seed` empty). `02_screening.csv` has screening decisions for only 14 of them. The other 108 records have no recorded decision, so they are shown as a separate box and are not counted as excluded.

## MAIN SCREENING FLOW

[Records identified from search sources (N = **122**)]  
← = rows with `source = search` in `01_all_recors.csv` (OpenAlex)

↓

[Records with no screening decision in `02_screening.csv` (N = **108**)]  
← = 122 − 14 (**to be confirmed by the authors**)

↓

[Records screened at V1 (N = **14**)]  
← = rows in `02_screening.csv`

↓

[Excluded at V1 (N = **5**)]  
← = `Stage 1` = EXCLUDE/exclude: OA001 (EC6), OA012 (EC1), OA021 (EC7, duplicate of OA020), OA037 (EC2), OA052 (EC3)

↓

[Full-text assessed (N = **9**)]  
← = 14 − 5

↓

[Excluded at V2 (N = **2**)]  
← = `Stage 2` = EXCLUDE: OA002 (EC3), OA020 (EC3)

↓

[Final included from main search (N = **7**)]  
← = `Final Decision` = INCLUDE: OA007, OA008, OA016, OA017, OA018, OA019, OA034


## SNOWBALLING BRANCH

[Records added through snowballing (N = **0**)]  
← = rows with `source = snowball-back` or `snowball-fwd` in `01_all_recors.csv` (none; all 122 rows are `search`)

↓

[Included from snowballing (N = **0**)]


## FINAL TOTAL

**Final included = 7 + 0 = 7**

← = total number of `INCLUDE` rows in `02_screening.csv`


## NUMERICAL CHECK

### Main screening flow

```text
122 − 108 = 14
14 − 5 = 9
9 − 2 = 7
```

### Snowballing

```text
0 − 0 = 0
```

### Final total

```text
7 + 0 = 7
```

## DATA CHECK

### `01_all_recors.csv`

```text
search          = 122
snowball-back   = 0
snowball-fwd    = 0
snowball-*      = 0
total           = 122
unique record_id = 122
duplicate titles = 1 pair (OA020 / OA021: ACM TOSEM version vs arXiv version, different DOIs)
```

### `02_screening.csv`

```text
rows                         = 14
Stage 1 EXCLUDE/exclude      = 5
Stage 1 INCLUDE              = 9
Stage 2 EXCLUDE              = 2
Stage 2 INCLUDE              = 7
Final INCLUDE                = 7
Final EXCLUDE                = 7
```

### Exclusion reasons (all 7 final exclusions)

```text
EC1 (Indonesian language)                  = 1  (OA012)
EC2 (Out of domain)                        = 1  (OA037)
EC3 (Secondary / non-peer-reviewed / overview) = 3  (OA002, OA020, OA052)
EC6 (Missing abstract / full text)         = 1  (OA001)
EC7 (Duplicate)                            = 1  (OA021)
```
