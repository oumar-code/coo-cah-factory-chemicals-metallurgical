# DT Go / No-Go Checklist

> **Factory:** Coo-Cah Metallurgical & Minerals Factory
> **Purpose:** Current hard-gate posture for DT readiness and later Tier 1 release review
> **Status date:** 2026-06-03

---

## Current posture summary

| Item | Status | Evidence |
| --- | --- | --- |
| Data quality and completeness thresholds met | RED | [`dt-data-quality-scorecard.md`](./dt-data-quality-scorecard.md) exists, but live values are not yet captured |
| Statistically valid KPI improvements vs. baseline and matched-control | RED | No completed simulation evidence bundles yet |
| No hidden manual rework burden or critical operational regressions | AMBER | Governance and review structure opened, but no live operational evidence yet |
| Financial ROI threshold met and signed by Finance | RED | No DT intervention outcomes yet |
| Full evidence pack reproducible by independent reviewer | RED | Evidence index and simulation design pack exist, but run lineage is not yet captured |
| Group CTO + PMO sign-off complete | RED | No final gate review yet |

---

## Template checklist with current status

- [ ] Data quality and completeness thresholds met  
  **Current status:** RED  
  **Next evidence needed:** First live baseline in [`dt-data-quality-scorecard.md`](./dt-data-quality-scorecard.md)

- [ ] Statistically valid KPI improvements vs. baseline and matched-control  
  **Current status:** RED  
  **Next evidence needed:** 3 completed simulation bundles aligned to [`dt-kpi-dictionary.md`](./dt-kpi-dictionary.md) and [`dt-simulation-designs.md`](./dt-simulation-designs.md)

- [ ] No hidden manual rework burden or critical operational regressions  
  **Current status:** AMBER  
  **Next evidence needed:** Weekly governance logs, exception tracking, and first intervention review

- [ ] Financial ROI threshold met and signed by Finance  
  **Current status:** RED  
  **Next evidence needed:** Benefit-cost model after first validated simulation outcomes

- [ ] Full evidence pack reproducible by independent reviewer  
  **Current status:** RED  
  **Next evidence needed:** Query references, input snapshots, output hashes, and reviewer sign-off

- [ ] Group CTO + PMO sign-off complete  
  **Current status:** RED  
  **Next evidence needed:** Final go/no-go memo after all prior items are green

---

## Decision rule

Do not claim DT-ready status for CCH-MET until:

1. Mandatory artifacts are complete and validated.
2. Live data connectivity is proven for critical assets.
3. At least 3 simulations have reproducible evidence lineage.
