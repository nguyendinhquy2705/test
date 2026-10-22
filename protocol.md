# Review Protocol

## 1. Study Identification

**Research topic:**
Comparing EP-BVA and Decision-Table Worksheets for Student Test Design on PURE

**Research Question (RQ):**

> When designing black-box tests for 20 frozen functional requirements from PURE, do students using an EP-BVA worksheet or a Decision-Table worksheet achieve higher item coverage compared with the instructor reference inventory?

---

## 2. PICOS

| Element                    | Definition                                                                                                                                           |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| **P - Population/Problem** | Students designing black-box tests for functional requirements in the PURE requirement set                                                           |
| **I - Intervention**       | Manual EP-BVA worksheet or manual Decision-Table worksheet for black-box test design                                                                 |
| **C - Comparison**         | The alternative test-design worksheet, human/manual baseline, or another applicable black-box test-design approach                                   |
| **O - Outcome**            | Item coverage percentage, including applicable EP, BVA, DT, ST, and UC reference items                                                               |
| **S - Study Design**       | Empirical experiment, controlled experiment, comparative study, case study, systematic review, mapping study, or other relevant evidence-based study |

---

## 3. Search Strategy

### 3.1 Primary Databases

The review will search at least three bibliographic sources:

1. IEEE Xplore
2. ACM Digital Library
3. OpenAlex

Google Scholar and Semantic Scholar may be used to identify seed papers and support forward/backward snowballing. They will not be used as the primary source for PRISMA search-result counts.

---

## 4. Official Search String A

The official search string follows the P-I-O structure.

```text
("black-box test design" OR "requirements-based testing" OR "user acceptance testing" OR PURE)
AND
("equivalence partitioning" OR "boundary value analysis" OR "decision table testing" OR "student experiment")
AND
("coverage item" OR "requirements coverage" OR "test coverage")
```

### 4.1 Search String Components

| Block | Purpose                            | Search Terms                                                                                          |
| ----- | ---------------------------------- | ----------------------------------------------------------------------------------------------------- |
| **P** | Testing task/context               | "black-box test design", "requirements-based testing", "user acceptance testing", PURE                |
| **I** | Test-design technique/intervention | "equivalence partitioning", "boundary value analysis", "decision table testing", "student experiment" |
| **O** | Outcome/metric                     | "coverage item", "requirements coverage", "test coverage"                                             |

### 4.2 Comparison Terms

Comparison terms such as:

* human
* baseline
* manual

are intentionally **not included** in String A.

The comparison condition will be assessed during title/abstract and full-text screening because these terms are broad and may exclude relevant studies.

---

## 5. Search Adaptation Rules

String A is the predefined primary search string.

Where a database supports the Boolean syntax, String A will be executed without conceptual changes.

If a database requires syntax changes, the query may be adapted to the database's supported syntax while preserving the same P/I/O concepts.

Every adapted query must be recorded in the individual search log with:

* Database
* Search date
* Exact query
* Reason for adaptation
* Number of returned records

### 5.1 Too Many Results

If the search produces more than 500 records, an additional context term such as the dataset name may be added to improve precision.

The modification must be recorded in the search log.

### 5.2 Too Few Results

If the search produces fewer than 20 records, the Outcome (O) block may be removed as specified in the research assignment.

The resulting query must be recorded in the search log.

No search-string modification will be made silently.

---

## 6. Inclusion Criteria

### IC1 — Relevant Testing Activity

The study investigates black-box testing, requirements-based testing, functional testing, or test design based on functional requirements.

### IC2 — Relevant Test Design Technique

The study investigates at least one of:

* Equivalence Partitioning (EP)
* Boundary Value Analysis (BVA)
* Decision Table Testing (DT)
* Another closely related black-box test-design technique that can be mapped to the RQ.

### IC3 — Relevant Population or Testing Context

The study involves or provides evidence relevant to:

* students learning software testing,
* software testers,
* software developers/engineers,
* requirements-based test design,
* functional requirements, or
* test-case design.

Studies that do not specifically use students may still be retained when they provide relevant methodological or empirical evidence for the test-design techniques.

### IC4 — Relevant Outcome

The study reports at least one relevant outcome, including:

* test coverage,
* requirements coverage,
* item coverage,
* test-case coverage,
* fault detection,
* test effectiveness,
* number or quality of generated test cases, or
* another measurable outcome relevant to test-design quality.

### IC5 — Evidence-Based Study

The study provides documented research methods and findings, such as an:

* empirical study,
* controlled experiment,
* comparative study,
* case study,
* systematic literature review,
* mapping study, or
* other evidence-based research study.

### IC6 — Identifiable Source

The study has sufficient bibliographic information and a reliable source, preferably including a DOI or stable publisher/repository URL.

### IC7 — PICO Relevance

The study directly supports at least three of the four core PICO elements (P/I/C/O), or provides strong methodological/background evidence relevant to the RQ.

---

## 7. Exclusion Criteria

### EC1 — Irrelevant Testing Domain

Exclude studies that are unrelated to software testing, functional testing, requirements-based testing, or black-box test design.

### EC2 — White-Box Only

Exclude studies that focus exclusively on white-box testing, including:

* statement coverage,
* branch coverage,
* path coverage,
* code coverage,

without relevant black-box test-design evidence.

### EC3 — No Relevant Test Design Technique

Exclude studies that do not investigate EP, BVA, Decision Table Testing, or another relevant black-box test-design technique.

### EC4 — No Relevant Outcome

Exclude studies that provide no evidence related to test coverage, requirements coverage, item coverage, test effectiveness, fault detection, test-case quality, or another relevant measurable outcome.

### EC5 — Insufficient Research Evidence

Exclude studies where the research method, data, or findings cannot be sufficiently determined.

### EC6 — Non-Research Material

Exclude:

* blogs,
* advertisements,
* commercial webpages,
* lecture slides,
* tutorials,
* opinion articles,

unless explicitly retained as background material outside the final evidence set.

### EC7 — Duplicate

Exclude duplicate records representing the same study or publication.

When multiple versions of the same study exist, the most complete and appropriate version will be retained according to the team protocol.

### EC8 — Inaccessible or Unverifiable Source

Exclude records for which the publication cannot be reliably identified or whose relevant evidence cannot be verified.

---

## 8. Search and Record Management

All records retrieved from the primary databases will first be entered into:

```text
data/01_all_records.csv
```

Records will initially be treated as candidate records and will not be considered final included studies at this stage.

The following information should be recorded where available:

* Record ID
* Title
* Authors
* Year
* Venue
* Database/source
* Search ID
* DOI
* URL
* Search date
* Screening status

---

## 9. Deduplication

Duplicate records will be identified using available bibliographic information.

Priority for duplicate detection:

1. DOI
2. Exact title
3. Author/year combination
4. Other bibliographic metadata

Duplicate records will be removed before final screening.

The deduplication process must be documented so that PRISMA counts can be reconstructed.

---

## 10. Screening Procedure

Screening will be performed in two stages.

### Stage 1 — Title and Abstract Screening

Each candidate record will receive one of:

* **INCLUDE** — clearly relevant.
* **EXCLUDE** — clearly meets an exclusion criterion.
* **UNSURE** — insufficient information; move to full-text screening.

### Stage 2 — Full-Text Screening

Records marked INCLUDE or UNSURE will be assessed using the full text.

The final decision will be:

* **INCLUDE**
* **EXCLUDE**

For every full-text exclusion, one primary exclusion reason must be recorded using EC1–EC8.

The final included records will be stored in:

```text
data/03_final_included.csv
```

---

## 11. Snowballing

After the main screening, each group member will select one included seed paper.

Each member will perform:

* one backward snowballing round, and
* one forward snowballing round.

### 11.1 Seed Selection Criteria

A seed paper must:

1. Be INCLUDE after full-text screening.
2. Match at least 3 of the 4 PICO elements.
3. Have approximately 10–200 citations where citation information is available.
4. Not be selected as the seed by another group member.
5. Be sufficiently relevant to support backward and forward snowballing.

The seed selection and justification must be documented in the member's search log.

### 11.2 Backward Snowballing

References cited by the seed paper will be reviewed.

New candidate records will be screened using the same IC/EC criteria.

### 11.3 Forward Snowballing

Studies citing the seed paper will be identified using an appropriate citation index.

New candidate records will be screened using the same IC/EC criteria.

All snowballing records must record:

* Seed paper
* Direction
* Source
* Title
* Year
* DOI/URL
* Screening decision
* Exclusion reason where applicable

---

## 12. Data Extraction

For each included study, the following information will be extracted where available:

| Field            | Description                                |
| ---------------- | ------------------------------------------ |
| Study ID         | Unique identifier                          |
| Title            | Full publication title                     |
| Authors          | Publication authors                        |
| Year             | Publication year                           |
| Venue            | Journal/conference/workshop                |
| DOI/URL          | Stable source                              |
| P                | Population/problem                         |
| I                | Intervention/test technique                |
| C                | Comparison/baseline                        |
| O                | Outcome                                    |
| Method           | Research method                            |
| Sample           | Participants, requirements, projects, etc. |
| Dataset/context  | Dataset or testing context                 |
| Main result      | Main finding                               |
| Numerical result | Actual reported number                     |
| Limitation       | Study limitation                           |
| RQ relevance     | Relevance to the research question         |

---

## 13. Numerical Evidence Requirement

The final evidence table should contain actual numerical results for at least 50% of included studies when numerical results are available in the source.

Examples of numerical evidence include:

* percentages,
* coverage values,
* sample sizes,
* p-values,
* effect sizes,
* number of test cases,
* fault detection rates,
* accuracy values.

Qualitative statements such as "improved performance" or "was more effective" alone are not considered numerical evidence.

---

## 14. PRISMA Accounting

The team will maintain consistent record counts across:

```text
01_all_records.csv
        ↓
Deduplication
        ↓
02_after_screening_v1.csv
        ↓
Full-text screening
        ↓
03_final_included.csv
        ↓
PRISMA
```

The numbers reported in the PRISMA flow must match the actual records represented in the CSV files.

No PRISMA number will be invented or estimated.

---

## 15. Team Screening and Quality Check

After screening:

* Each member will select one seed paper.
* Each member will conduct one backward and one forward snowballing round.
* The second member will check at least 20% of the papers excluded in the first screening round.
* The second member will cross-check at least 20% of the Evidence Table.
* Any disagreement will be discussed and resolved before the final team synthesis.

---

## 16. Team Synthesis

After individual searches and screening, the project leader will merge the included evidence into:

```text
team-synthesis/evidence-table-merged.md
```

The team will also produce:

```text
team-synthesis/prisma-team.md
team-synthesis/rq-evidence-map.md
```

The final evidence table must contain at least 12 included papers after individual searching and snowballing.

If the team has fewer than 12 suitable papers after the individual snowballing stage, the team will report the shortage to the instructor and follow the instructor's direction rather than repeatedly performing uncontrolled snowballing.

---

## 17. Protocol Freeze

This protocol, including the main research question, String A, and IC/EC, will be finalized before the main search begins.

Changes made after observing search or screening results are not permitted unless they are explicitly documented with:

* the original rule,
* the changed rule,
* reason for change,
* date of change,
* and effect on the review.

The protocol will be committed to the repository before the first main search.
