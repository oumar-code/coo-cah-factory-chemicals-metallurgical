# DT Evidence Index

> **Factory:** Coo-Cah Metallurgical & Minerals Factory
> **Purpose:** Single evidence registry for DT readiness hard-release conditions
> **Status scale:** `Planned` / `Stub` / `Live` / `Audited`

---

## 1. Hard release condition summary

| Condition | Current Status | Release Rule |
| --- | --- | --- |
| Mandatory DT artifacts complete and validated | Stub | Must be complete before DT-ready status can be claimed |
| Live data connectivity proven for critical assets | Planned | Must include timestamped OT → MES → DT evidence for critical assets |
| At least 3 simulations with reproducible evidence lineage | Planned | Must include reproducible inputs, outputs, and reviewable lineage |

---

## 2. Mandatory artifact register

| Hard Release Condition | Artifact | Current Status | Owner | Notes |
| --- | --- | --- | --- | --- |
| Mandatory artifacts complete | [`digital-twin.md`](./digital-twin.md) | Stub | Digital Twin Engineer | Core DT scope and asset registry documented |
| Mandatory artifacts complete | [`sensor-map.md`](./sensor-map.md) | Stub | OT Instrumentation Lead | Critical sensor registry documented |
| Mandatory artifacts complete | [`bim/README.md`](./bim/README.md) | Stub | BIM Coordinator | BIM index added in this sprint; pending review |
| Mandatory artifacts complete | [`bim/zone-boundaries.md`](./bim/zone-boundaries.md) | Stub | BIM Coordinator | Zone geometry defined |
| Mandatory artifacts complete | [`bim/asset-anchors.md`](./bim/asset-anchors.md) | Stub | Digital Twin Engineer | Anchor coordinates defined |
| Mandatory artifacts complete | [`mes-integration.md`](./mes-integration.md) | Stub | MES Product Owner | Integration design documented |
| Mandatory artifacts complete | [`dt-governance-log.md`](./dt-governance-log.md) | Stub | Factory CTO | Weekly governance log opened |
| Mandatory artifacts complete | [`dt-gonogo-checklist.md`](./dt-gonogo-checklist.md) | Stub | PMO | Current gate posture documented |

---

## 3. Live connectivity evidence register

| Hard Release Condition | Artifact | Current Status | Owner | Notes |
| --- | --- | --- | --- | --- |
| Live data connectivity proven | [`dt-live-evidence-briefing.md`](./dt-live-evidence-briefing.md) | Stub | MES Product Owner / OT Integration Lead | Briefing issued with acceptance criteria |
| Live data connectivity proven | [`dt-data-quality-scorecard.md`](./dt-data-quality-scorecard.md) | Stub | OT Instrumentation Lead | Baseline template published; live values pending commissioning |
| Live data connectivity proven | [`dt-connectivity-evidence/README.md`](./dt-connectivity-evidence/README.md) | Stub | MES Product Owner / OT Integration Lead | Connectivity pack structure created |
| Live data connectivity proven | [`dt-connectivity-evidence/eaf-z2.md`](./dt-connectivity-evidence/eaf-z2.md) | Planned | OT Integration Lead | Awaiting first timestamped EAF trace |
| Live data connectivity proven | [`dt-connectivity-evidence/wire-draw-z7.md`](./dt-connectivity-evidence/wire-draw-z7.md) | Planned | MES Product Owner | Awaiting first wire-draw trace |
| Live data connectivity proven | [`dt-connectivity-evidence/bess-z10.md`](./dt-connectivity-evidence/bess-z10.md) | Planned | Energy Systems Lead | Awaiting first BESS trace |

---

## 4. Simulation evidence register

| Hard Release Condition | Artifact | Current Status | Owner | Notes |
| --- | --- | --- | --- | --- |
| 3 reproducible simulations | [`dt-kpi-dictionary.md`](./dt-kpi-dictionary.md) | Stub | DT Engineering Lead | KPI formulas locked before runs |
| 3 reproducible simulations | [`dt-simulation-designs.md`](./dt-simulation-designs.md) | Stub | DT Engineering Lead / AI Data Lead | Experiment designs frozen before runs |
| 3 reproducible simulations | Simulation bundle 1 — Throughput | Planned | DT Engineering Lead | Run pack not yet captured |
| 3 reproducible simulations | Simulation bundle 2 — Quality | Planned | DT Engineering Lead | Run pack not yet captured |
| 3 reproducible simulations | Simulation bundle 3 — Energy | Planned | DT Engineering Lead | Run pack not yet captured |

---

## 5. Evidence promotion candidates

The following artifacts should be reviewed for promotion back to the master template after sprint close:

1. BIM README index pattern
2. DT evidence index pattern
3. KPI dictionary structure for factory-specific simulations
4. Simulation design package structure
