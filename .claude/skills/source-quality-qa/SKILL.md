---
name: source-quality-qa
description: Independently checks a completed CanDo source-page draft against product truth, claims, SEO/page strategy, retailer routes, links, live evidence, stramien and output completeness. Use after source build and before localization.
---
# Source Quality QA

Read ../../../09-QA-GATE.md and review the full draft independently.

Check:
- routing/orchestration;
- product truth;
- page strategy;
- audience/brand;
- stramien;
- links;
- web delta-check;
- output completeness;
- retailer/route governance.

Output PASS/PARTIAL/FAIL per section, every defect with the violated rule/source, `CRITICAL DEFECT` when applicable and an exact fix instruction.

If there is a FAIL, return `NEEDS_FIX`. After one correction round, run once more.
Only return `READY FOR HUMAN REVIEW` when no FAIL or critical defect remains.
