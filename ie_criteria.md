# Official Search String A

## String A

```text
("black-box test design" OR "requirements-based testing" OR "user acceptance testing" OR PURE)
AND
("equivalence partitioning" OR "boundary value analysis" OR "decision table testing" OR "student experiment")
AND
("coverage item" OR "requirements coverage" OR "test coverage")
```

## Search String Structure

| Block | Purpose                              | Terms                                                                                                 |
| ----- | ------------------------------------ | ----------------------------------------------------------------------------------------------------- |
| P     | Testing task / context               | "black-box test design", "requirements-based testing", "user acceptance testing", PURE                |
| I     | Test design technique / intervention | "equivalence partitioning", "boundary value analysis", "decision table testing", "student experiment" |
| O     | Outcome / metric                     | "coverage item", "requirements coverage", "test coverage"                                             |

## Rationale

The official search string follows the P-I-O structure of the research question.

The comparison condition (C), including terms such as "human", "baseline", or "manual", is intentionally excluded from the search string because these terms are broad and may eliminate relevant studies.

The comparison condition will instead be assessed during title/abstract and full-text screening using the predefined inclusion and exclusion criteria.

## Search String Modification Rule

String A is the predefined primary search string and should be used unchanged where the database supports the Boolean syntax.

If a database does not support the complete syntax, the search string may be adapted only to the database's search syntax while preserving the same conceptual P/I/O blocks.

Any modified version must be recorded in the individual `search-log.md`, including:

* Database
* Date
* Exact query used
* Reason for modification
* Number of results returned

## Search Expansion Rule

If the initial search returns fewer than 20 records, the team may remove the Outcome (O) block as specified in the research protocol.

If the search returns more than 500 records, the team may add the dataset name or another predefined context term.

Any change from String A must be recorded in the search log and must not be silently changed after seeing the final results.
# Official Inclusion and Exclusion Criteria

## Inclusion Criteria — IC

### IC1 — Relevant testing activity

The study investigates software testing activities related to **black-box testing, requirements-based testing, functional testing, or test design from functional requirements**.

### IC2 — Relevant test design technique

The study investigates at least one of the following:

* Equivalence Partitioning (EP)
* Boundary Value Analysis (BVA)
* Decision Table Testing (DT)
* Another closely related black-box test design technique that can be mapped to the research question.

### IC3 — Relevant population or testing context

The study involves or provides evidence relevant to:

* students learning software testing,
* software testers,
* software developers/engineers,
* requirements-based test design,
* functional requirements, or
* test-case design.

Studies that do not specifically use students may still be included when they provide direct methodological or empirical evidence supporting the test-design techniques in the RQ.

### IC4 — Relevant outcome

The study reports at least one outcome relevant to test-design quality or coverage, including:

* test coverage,
* requirements coverage,
* item coverage,
* test-case coverage,
* fault detection,
* test effectiveness,
* number/quality of generated test cases, or
* another measurable outcome that can inform the research question.

### IC5 — Sufficient research evidence

The study provides a documented research method and findings, such as:

* controlled experiment,
* empirical study,
* case study,
* comparative study,
* systematic literature review,
* mapping study, or
* another evidence-based research method.

### IC6 — Identifiable source

The study has sufficient bibliographic information and a reliable source, preferably including a DOI or stable publisher/repository URL.

### IC7 — Relevance to the RQ

The study directly supports at least **three of the four PICO elements (P/I/C/O)**, or provides strong methodological/background evidence for one or more elements of the research question.

---

# Exclusion Criteria — EC

### EC1 — Irrelevant testing domain

Exclude studies that are not related to software testing, functional testing, requirements-based testing, or black-box test design.

### EC2 — White-box only

Exclude studies that focus exclusively on white-box techniques such as:

* statement coverage,
* branch coverage,
* path coverage,
* code coverage,

without relevant black-box test-design evidence.

### EC3 — No relevant test design technique

Exclude studies that do not address EP, BVA, Decision Table Testing, or another relevant black-box test design technique.

### EC4 — No relevant outcome

Exclude studies that do not provide evidence related to test coverage, requirements coverage, item coverage, test effectiveness, fault detection, test-case quality, or another relevant measurable outcome.

### EC5 — Insufficient evidence

Exclude publications where the research method, data, or findings cannot be determined sufficiently.

### EC6 — Non-research material

Exclude:

* blogs,
* advertisements,
* commercial webpages,
* lecture slides,
* tutorials,
* opinion articles,

unless they are explicitly required as background sources rather than included evidence.

### EC7 — Duplicate

Exclude duplicate records representing the same study/publication.

When multiple versions of the same study are found, retain the most complete and appropriate version according to the team's protocol.

### EC8 — Inaccessible or unverifiable source

Exclude records for which the publication cannot be reliably identified or whose relevant evidence cannot be verified from an available source.

---

# Screening Decision Rules

Each record is assigned one of the following decisions during screening:

* **INCLUDE** — clearly satisfies the inclusion criteria.
* **EXCLUDE** — satisfies at least one exclusion criterion.
* **UNSURE** — insufficient information at title/abstract stage; proceed to full-text screening.

For every full-text exclusion, record the primary exclusion criterion (EC1–EC8).

The same IC/EC criteria must be applied to:

1. Records retrieved from the primary databases.
2. Records obtained through backward snowballing.
3. Records obtained through forward snowballing.

The criteria must be finalized before the main screening results are used for the final team synthesis.
