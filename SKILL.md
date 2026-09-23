---
name: source-quality-qa
description: Independent final gate for the benchmark worktop page. Checks product truth, claims, page strategy, links, web evidence, stramien use and traceability.
---
# Source Quality QA
Read `09-QA-GATE.md`. Review the full draft independently.
Output PASS/PARTIAL/FAIL per section A-H, every defect with violated rule/source, `CRITICAL DEFECT` when applicable and exact fix instruction.
If there is a FAIL, return `NEEDS_FIX`. After one correction round, run once more.
Only return `READY FOR HUMAN REVIEW` when no FAIL or critical defect remains.
