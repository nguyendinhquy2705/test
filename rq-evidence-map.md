# RQ Evidence Map (Team Synthesis)

**RQ:** When designing black-box tests for 20 frozen functional requirements from PURE, do students using an EP-BVA worksheet or a Decision-Table worksheet achieve higher item coverage compared with the instructor reference inventory?

**Mapping rule:** P = students; I = manual EP-BVA or Decision Table worksheet; C = alternative worksheet or instructor reference inventory; O = item coverage across the same 20 PURE requirements. Generic coverage, test effectiveness, or fault detection is not treated as the target O unless it measures this outcome.

## PICO coverage

| RQ element | Evidence in merged set | Assessment |
|---|---|---|
| P — students learning test design | E41 | One paper studies student testers, but its task is EP vs branch testing/code reading on C programs. It does not study the PURE task. |
| I — manual EP-BVA worksheet | E39, E41 and related EP/BVA studies in E01–E17, E42 | Evidence covers methods or automated tools, but no study evaluates the specified student worksheet. |
| I — manual Decision-Table worksheet | E03, E05, E40 and related requirements-based studies | Evidence concerns automated decision tables or an applied BVA/DT case; no student worksheet evaluation. |
| C — alternative worksheet / instructor reference inventory | No study in the merged set | Some papers compare tools, generation strategies, or manual and automated methods, but none uses the target comparison. |
| O — item coverage on 20 frozen PURE requirements | No study in the merged set | Papers report other coverage levels, fault detection, test counts, or qualitative findings. |

## Evidence clusters

| Cluster | Study IDs | P/I/C/O contribution | Use in synthesis |
|---|---|---|---|
| Requirements-based EP/BVA/Decision Table and black-box design | E01–E17, E39–E42 | Mainly I; some generic O; E41 contributes P | Methodological/background evidence. Results cannot be interpreted as PURE item-coverage effects. |
| Combinatorial coverage and test-suite construction | E18–E33 | Related test-design methods and generic coverage/fault outcomes; some tool/baseline comparisons | Context and counter-evidence on coverage strategies; not the target worksheets. |
| Fault localization / out-of-domain candidates | E34–E38 | Mostly generic testing outcomes; weak or indirect P/I/C/O match | Recheck against IC/EC before treating these as final included evidence. |

## Synthesis

No study in the current merged set directly supports all required elements. E41 is the only study with student participants, but it does not compare EP-BVA with Decision Table Testing, use PURE requirements, or measure coverage against the instructor inventory. The review's own experiment remains necessary to answer the RQ.

**Open evidence gaps:** target worksheet comparison; shared PURE requirement set; instructor reference inventory; consistent item-coverage outcome; broader student replication.
