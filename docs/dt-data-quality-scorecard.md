# DT Data Quality Scorecard

> **Factory:** Coo-Cah Metallurgical & Minerals Factory
> **Purpose:** Baseline scorecard for DT-critical telemetry streams
> **Status:** Partial — awaiting first live capture window
> **Owner:** OT Instrumentation Lead

---

## Scoring fields

Every critical stream category must report:

- Completeness %
- Freshness (last-seen lag)
- Schema validity %
- Capture date
- Reviewer

---

## Baseline scorecard

| Process Domain | Critical Signals | Completeness % | Freshness | Schema Validity % | Capture Date | Reviewer | Current Status |
| --- | --- | ---: | --- | ---: | --- | --- | --- |
| Steel (Z2-Z5) | Melt temp, casting speed, rolling speed, gauge, torque, downtime | — | Awaiting first live capture | — | Pending | OT Instrumentation Lead | Stub |
| Aluminium (Z6) | Billet temp, ram pressure, profile speed, gauge | — | Awaiting first live capture | — | Pending | OT Instrumentation Lead | Stub |
| Copper (Z7) | Rod diameter, draw speed, wire tension, break count | — | Awaiting first live capture | — | Pending | OT Instrumentation Lead | Stub |
| Environmental (Z11) | ETP pH/flow, NOx/SO2/PM trends | — | Awaiting first live capture | — | Pending | OT Instrumentation Lead | Stub |
| Utilities (Z10) | Power import, PV output, BESS SoC, compressed-air pressure | — | Awaiting first live capture | — | Pending | OT Instrumentation Lead | Stub |

---

## Acceptance thresholds for first live baseline

| Metric | Threshold |
| --- | --- |
| Completeness | ≥ 98% for Steel, Aluminium, Copper, and Environmental domains; ≥ 99% for Utilities |
| Freshness | ≤ 60 s for Steel, Aluminium, Copper, and Environmental domains; ≤ 30 s for Utilities |
| Schema validity | 100% on required canonical fields |

---

## Notes

- Replace `—` values only after the first timestamped live capture is committed.
- Any stream below threshold remains non-green and must have a corrective action in [`dt-governance-log.md`](./dt-governance-log.md).
