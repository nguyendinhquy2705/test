# PRISMA Flow

> **Counting rule:** The main screening flow uses records with `source = search`. The snowballing branch uses records with `source` beginning with `snowball-`. The final included count is the sum of the main search branch and the snowballing branch.

## MAIN SCREENING FLOW

[Records identified from search sources (N = **97**)]

↓

[After deduplication (N = **19**)]  
← = number of rows with `source = search` in `01_all_records.csv`

↓

[Excluded at V1 (N = **9**)]  
← = search records with `v1_decision = EXCLUDE` in `02_after_screening_v1.csv`

↓

[Full-text assessed (N = **10**)]  
← = 19 − 9

↓

[Excluded at V2 (N = **3**)]  
← = 10 − 3

↓

[Final included from main search (N = **7**)]  
← = rows with `v2_decision = INCLUDE` and `source = search` in `03_final_included_updatedd_v2_reason_revised.csv`


## SNOWBALLING BRANCH

[Records added through snowballing (N = **78**)]  
← = rows with `source = snowball-back` or `source = snowball-fwd` in `01_all_records.csv`

↓

[Excluded at V1 (N = **1**)]

↓

[Full-text assessed (N = **77**)]  
← = 78 − 1

↓

[Excluded at V2 (N = **58**)]  
← = 77 − 19

↓

[Included from snowballing (N = **19**)]  
← = rows with `v2_decision = INCLUDE` and `source = snowball-*` in `03_final_included_updatedd_v2_reason_revised.csv`


## FINAL TOTAL

**Final included = 7 + 19 = 26**

← = total number of `INCLUDE` rows in `03_final_included_updatedd_v2_reason_revised.csv`


## NUMERICAL CHECK

### Main screening flow

```text
19 − 9 = 10
10 − 3 = 7
```

### Snowballing

```text
78 − 1 = 77
77 − 58 = 19
```

### Final total

```text
7 + 19 = 26
```

## DATA CHECK

### `01_all_records.csv`

```text
search          = 19
snowball-back   = 32
snowball-fwd    = 46
snowball-*      = 78
total           = 97
```

### `02_after_screening_v1.csv`

```text
search:
  EXCLUDE = 9
  INCLUDE/UNSURE = 10

snowball:
  EXCLUDE = 1
  INCLUDE/UNSURE = 77
```

### `03_final_included_updatedd_v2_reason_revised.csv`

```text
main search included        = 7
snowball-back included      = 13
snowball-fwd included       = 6
total included              = 26
```
