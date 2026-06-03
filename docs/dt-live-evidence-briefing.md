# DT Live-Evidence Briefing

> **Audience:** MES Product Owner, OT Integration Lead, OT Instrumentation Lead, Energy Systems Lead
> **Purpose:** Assign owners and acceptance criteria for the first live DT evidence capture window

---

## Subject

CCH-MET DT readiness sprint — required live-evidence pack for first capture window

---

## Briefing message

The two-week DT readiness sprint has opened Track B for live-system evidence. Repository artifacts are being published in parallel, but DT-ready status remains blocked until critical-asset connectivity and reproducible simulation evidence are captured.

Please treat the following evidence items as mandatory for the first commissioning capture window.

---

## Assigned owners

| Evidence Item | Primary Owner | Supporting Owner | Due Date |
| --- | --- | --- | --- |
| Data-quality scorecard baseline | OT Instrumentation Lead | MES Product Owner | 2026-06-14 |
| EAF Z2 OT → MES → DT trace pack | OT Integration Lead | MES Product Owner | 2026-06-14 |
| Wire Draw Z7 OT → MES → DT trace pack | MES Product Owner | OT Integration Lead | 2026-06-14 |
| BESS Z10 OT → MES → DT trace pack | Energy Systems Lead | OT Integration Lead | 2026-06-14 |

---

## Acceptance criteria extracted from `mes-integration.md`

### 1. Data contract checks

All captured points must include:

- Canonical `DT-MET-*` asset keys
- Canonical `Z1`-`Z14` zone keys
- UTC ISO 8601 timestamps with millisecond precision
- SI unit field
- Quality flag (`good`, `bad`, `uncertain`)

### 2. Critical telemetry coverage

| Process Domain | Minimum Signals Required for First Baseline |
| --- | --- |
| Steel (Z2-Z5) | Melt temp, casting speed, rolling speed, gauge, torque, downtime |
| Aluminium (Z6) | Billet temp, ram pressure, profile speed, gauge |
| Copper (Z7) | Rod diameter, draw speed, wire tension, break count |
| Environmental (Z11) | ETP pH/flow, NOx/SO2/PM trends |
| Utilities (Z10) | Power import, PV output, BESS SoC, compressed air pressure |

### 3. Minimum trace-pack contents

Each critical-asset trace pack must include:

1. Source timestamp from OT system
2. MES receipt timestamp or event record
3. DT state-store or simulation-trigger timestamp
4. Asset ID, zone ID, signal name, and quality flag
5. Screenshot or log extract showing the same event across the chain

### 4. Event triggers that must be visible when available

- Work-order start/stop
- Equipment state change (`run`, `idle`, `fault`)
- Quality out-of-spec event
- Energy threshold breach
- Environmental threshold breach

---

## Escalation rule

If commissioning windows slip, keep the repository artifacts current and update the affected evidence item status to `Planned` or `Stub`. Do not mark any live-evidence item `Live` until timestamped proof is committed.
