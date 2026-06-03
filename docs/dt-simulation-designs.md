# DT Simulation Designs

> **Factory:** Coo-Cah Metallurgical & Minerals Factory
> **Purpose:** Controlled experiment designs for the first 3 DT simulation evidence bundles
> **Standard:** Use pre/post + matched-control design with reproducibility package for every accepted run

---

## 1. Throughput simulation

| Field | Required Content |
| --- | --- |
| Design type | Pre/post + matched-control |
| Unit of analysis | Shift and line |
| Observation windows | Baseline window and intervention window must use comparable product mix and staffing profile |
| Confounder controls | Product mix, maintenance events, downstream constraints, planned stoppages, crew assignment |
| Data quality gates | Completeness ≥ 98%, freshness ≤ 60 s for critical telemetry, schema validity = 100% on required fields |
| Intervention log | Timestamped simulation version, constraint set, operator or planner action, approval record |
| Statistical method | Mean-difference comparison with matched-control validation and exception log for outlier shifts |
| Reproducibility package | Query references, input snapshot, simulation config, output tables, result hash, review sign-off |
| KPI linkage | Rolling throughput rate, Copper draw output rate, Rolling yield loss rate |

### Scope

- Steel line coverage: Z2-Z5
- Copper line coverage: Z7
- Use case: throughput, yield, and bottleneck analysis

---

## 2. Quality simulation

| Field | Required Content |
| --- | --- |
| Design type | Pre/post + matched-control |
| Unit of analysis | Lot, coil, or production batch |
| Observation windows | Baseline and intervention windows aligned to comparable SKUs and test plans |
| Confounder controls | Product grade, inspection frequency, maintenance activity, raw-material variance, staffing mix |
| Data quality gates | Completeness ≥ 98%, freshness ≤ 5 min for quality events, schema validity = 100% on required fields |
| Intervention log | Timestamped simulation version, quality rule change, operator acknowledgment, rollback trigger |
| Statistical method | Defect-rate and conformance-rate comparison with matched-control validation |
| Reproducibility package | Query references, sampled quality records, model inputs, output tables, result hash, review sign-off |
| KPI linkage | Dimensional conformance rate, Defect event rate |

### Scope

- Steel rolling gauge quality in Z5
- Copper rod and wire quality in Z7
- Use case: quality drift, breakage risk, and defect escape reduction

---

## 3. Energy simulation

| Field | Required Content |
| --- | --- |
| Design type | Pre/post + matched-control |
| Unit of analysis | Hour and shift |
| Observation windows | Comparable operating days with similar production load and tariff context |
| Confounder controls | Production schedule, utility interruptions, solar irradiance, maintenance outages, compressor demand |
| Data quality gates | Completeness ≥ 99%, freshness ≤ 30 s for utility telemetry, schema validity = 100% on required fields |
| Intervention log | Timestamped dispatch plan, BESS rule version, operator approval, exception or override record |
| Statistical method | Peak-demand and grid-import comparison with matched-control validation |
| Reproducibility package | Query references, load forecast snapshot, dispatch plan, output tables, result hash, review sign-off |
| KPI linkage | Peak-shaving effectiveness, Grid-import intensity, BESS dispatch adherence |

### Scope

- Utilities and energy domain in Z10
- Supporting process context from Z2-Z7 where production load drives demand
- Use case: energy cost and dispatch simulation

---

## Acceptance rule

No simulation run may be counted toward DT-ready status until its design stays frozen, its data-quality gates pass, and its reproducibility package is committed or archived with retrievable references.
