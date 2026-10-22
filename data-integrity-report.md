# Data Integrity and Merge Report

Audit date: 2026-10-22

- Raw member records imported into canonical `01_all_records.csv`: 410.
- Canonical raw file uses a single 15-column header and consistent CSV quoting.
- Member source counts: M1 151, M2 97, M3 40, M4 122.
- Member-specific final INCLUDE rows before cross-member dedup: 2 + 26 + 2 + 7 = 37.
- Team-deduplicated final INCLUDE records in `03_final_included_team.csv`: 37. Title-based reconciliation currently maps 21/37 records to rows in the merged evidence table; see `evidence-table-inclusion-reconciliation.csv`.
- Member 4 screening CSV was normalized to remove a blank first line and empty trailing columns; all original screening fields relevant to decision were preserved in the normalized column names.
- The malformed root-level `01_all_records.csv` that contained a prose summary rather than record rows was preserved as `archive/01_all_records-original-malformed-summary.csv.txt`; the root path now contains a valid canonical merged record table.

## Caveats

1. This is a structural/record-level merge, not independent verification of every paper's scientific validity.
2. `03_final_included_team.csv` reflects member-level final INCLUDE decisions and deduplication. The team must still validate each inclusion against the shared IC/EC protocol.
3. The team evidence table contains 42 extracted studies; it is not automatically identical to the final included set. Reconcile every evidence row to the team include file before final PRISMA reporting.
4. Do not infer missing publication details or numerical results from abstracts when the protocol requires Table/Figure evidence.

- Protocol-standard copies are available under `data/01_all_records.csv`, `data/02_after_screening_v1.csv`, and `data/03_final_included.csv`.
