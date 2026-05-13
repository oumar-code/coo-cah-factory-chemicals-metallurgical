# Metallurgical Factory — Phase 2 Implementation Plan

> **Project Coo-Cah | AI-Powered Manufacturing Ecosystem**
> **Factory:** Coo-Cah Metallurgical & Minerals Factory | **Location:** Warri / Ovwian-Aladja Steel Corridor, Delta State | **Phase:** Phase 2
> **Document Version:** 1.0 | **Owner:** Programme Management Office

---

## 1. Strategy Overview

The implementation strategy is to run all non-equipment dependencies in parallel so that commissioning windows for steel, aluminium, copper, and lead-alloy lines are not delayed by digital, regulatory, workforce, or supply-chain blockers.

All workstreams execute on a two-week sprint cadence with weekly site execution reviews and bi-weekly steering decisions.

| Workstream | Name | Owner | Key Milestone |
| --- | --- | --- | --- |
| WS1 | Metallurgical MES + OT Integration | Digital Manufacturing / OT Team | M2.4 — MES live with rolling/extrusion/wire-drawing data (2026-Q1) |
| WS2 | Regulatory and Environmental Permits | Regulatory Affairs / HSE Team | M2.6 — NESREA + Delta approvals in place for hot commissioning |
| WS3 | Digital Twin + AI Model Readiness | AI Platform / Process Engineering | M2.8 — simulation pack for investor and operations readiness |
| WS4 | Workforce and Safety Competency | HR / Coo-Cah Academy | ~280 phase-1 staff certified pre-startup |
| WS5 | Supply Chain and Intra-Group Offtake | Procurement / Group Supply Chain | Copper cathode, aluminium ingot, billet contracts locked |
| WS6 | Energy and Utilities Commissioning | Energy / Infrastructure Team | M2.9 — 1,000 kWp PV + 1,200 kWh BESS integrated to MES |

---

## 2. Workstream 1 — Metallurgical MES + OT Integration

*Owner: Digital Manufacturing / OT Team*

### 2.1 Weeks 1–2 — Foundation and Environments

| Task | Detail |
| --- | --- |
| MES stack provisioning | Deploy on-site primary and cloud-synced DR instance for Warri operations |
| Edge historian nodes | Provision line-level edge gateways for steel rolling, aluminium extrusion, copper drawing, and utility plants |
| Asset and SKU registry | Seed all phase-1 SKUs (`CCH-MET-001` to `CCH-MET-008`) and critical assets in MES master data |

### 2.2 Weeks 3–6 — Module Configuration

Configure and validate modules in sequence:

1. Production order management
2. Batch/coil traceability
3. Quality non-conformance tracking
4. Environmental and ETP compliance logging
5. Utility and energy metering
6. CMMS and spare parts planning

### 2.3 Weeks 7–10 — Integration Plumbing (Machine-Ready)

| Integration Surface | Protocol | Objective |
| --- | --- | --- |
| Rolling mill PLC/DCS tags | OPC-UA | Real-time process and quality capture |
| Wire drawing line telemetry | OPC-UA / Modbus TCP | Throughput, tension, and defect signal capture |
| Galvanising and annealing lines | OPC-UA | Temperature, coating thickness, and alarm context |
| Laboratory quality systems | REST | Chemistry and mechanical test result ingestion |
| MES ↔ ERP | REST / secure API | Order, inventory, costing, and dispatch synchronization |
| MES ↔ Digital Twin / AI platform | MQTT + REST | Closed-loop analytics and simulation triggers |

### 2.4 Weeks 11–12 — UAT and Go-Live Readiness

| Test | Acceptance Criterion |
| --- | --- |
| End-to-end simulated order flow | Steel, aluminium, copper, and lead-alloy order flows pass with no P1 defects |
| Traceability integrity | Full heat/lot/coil trace from inbound material to outbound dispatch |
| Cybersecurity baseline | TLS 1.3 in-transit and AES-256 at-rest controls verified |
| Failover readiness | DR failover and historian replay validated |

---

## 3. Workstream 2 — Regulatory and Environmental Permits

*Owner: Regulatory Affairs / HSE Team*

### 3.1 Priority Permits and Compliance Stack

| Requirement | Authority / Standard | Target |
| --- | --- | --- |
| Environmental Impact Assessment (EIA) | NESREA + Delta State agencies | Pre-civil completion |
| Effluent treatment and discharge monitoring approval | NESREA | Before wet commissioning |
| Air emissions and stack monitoring program | NESREA | Before furnace/hot-process startup |
| Factory licensing and worker safety obligations | Factories Act + NSITF | Before production ramp |
| Management systems readiness | ISO 9001, 14001, 45001, 50001 | Phase 2 readiness gate |

### 3.2 Execution Sequence

1. Submit EIA and process hazard dossier for steel/aluminium/copper/lead-alloy operations.
2. Complete ETP neutrality and heavy-metal discharge control validation.
3. Confirm hazardous waste transport/disposal partner agreements.
4. Load all permit conditions into MES compliance workflows.

---

## 4. Workstream 3 — Digital Twin + AI Model Readiness

*Owner: AI Platform / Process Engineering*

### 4.1 AI/DT Scope for Metallurgical Operations

| Domain | Primary Use Cases |
| --- | --- |
| Steel processing | Rolling pass optimization, yield loss prediction, coil defect risk scoring |
| Aluminium operations | Extrusion die wear prediction, profile tolerance drift alerts |
| Copper wire production | Draw speed optimization, breakage risk and conductivity conformance |
| Utilities and energy | Furnace peak-load smoothing, BESS dispatch, compressed-air efficiency |

### 4.2 Readiness Deliverables

| Deliverable | Description |
| --- | --- |
| Canonical data contracts | MES and AI payload definitions for process, quality, and maintenance |
| Stub endpoint verification | Contract-consistent endpoint behavior for pre-production integration tests |
| Simulation evidence pack | Throughput, quality, downtime, and energy scenarios for steering reviews |
| Governance controls | Model lifecycle ownership, approval, and rollback controls |

---

## 5. Workstream 4 — Workforce and Safety Competency

*Owner: HR / Coo-Cah Academy*

### 5.1 Training Tracks

| Track | Audience | Core Topics |
| --- | --- | --- |
| Process operations | Rolling, extrusion, wire-drawing teams | SOPs, process limits, quality checkpoints |
| HSE and emergency response | All plant staff | Hot-work controls, chemical handling, lockout/tagout |
| Digital and MES operations | Supervisors, planners, data officers | Production order control, traceability, deviation handling |
| Maintenance reliability | Mechanical/electrical teams | Condition monitoring, planned shutdowns, spare strategy |

### 5.2 Workforce Gate Criteria

- 100% induction completion for Phase 1 workforce.
- Competency sign-off for critical line roles before hot commissioning.
- Incident reporting and near-miss logging fully active in MES.

---

## 6. Workstream 5 — Supply Chain and Intra-Group Offtake

*Owner: Procurement / Group Supply Chain*

### 6.1 Critical Inputs

| Input Category | Source Strategy | Risk Control |
| --- | --- | --- |
| Steel billet and heavy scrap | Delta Steel Company / DSIL + backup scrap yards | Long-term offtake + safety inventory |
| Aluminium ingot | NALCO + import fallback | Dual-source and 60-day cover |
| ETP copper cathode | LME-linked imports via Apapa/Tin Can | 90-day cover and FX planning |
| Lead feedstock | Domestic recycler network + certified suppliers | Batch assay and contamination controls |

### 6.2 Intra-Group Output Alignment

- Copper wire rod allocations synchronized with Power Electronics demand plans.
- Aluminium sheet/extrusion allocations synchronized with Kitchen and Personal Electronics ramps.
- Lead-alloy commitments synchronized with Plastics/energy-storage programs.

---

## 7. Workstream 6 — Energy and Utilities Commissioning

*Owner: Energy / Infrastructure Team*

| Utility Area | Target |
| --- | --- |
| Electrical interconnect | Stable BEDC 33/11 kV feed and protected internal distribution |
| Solar and storage | 1,000 kWp PV and 1,200 kWh LFP BESS integrated to EMS |
| Process utilities | Industrial water, compressed air, and treatment systems commissioned |
| Energy KPIs | Peak shaving, energy intensity tracking, and self-sufficiency reporting active |

---

## 8. Governance and Milestone Gates

| Gate | Trigger | Evidence |
| --- | --- | --- |
| G1 — Foundations complete | WS1 and WS2 startup complete | Environments online + permit submissions logged |
| G2 — Integration ready | WS1 machine-ready integration complete | Stub and interface test pass records |
| G3 — Regulatory readiness | Permit and compliance preconditions met | Approvals and MES compliance controls active |
| G4 — Workforce readiness | Critical role certifications complete | Training and competency register signed |
| G5 — Commissioning go decision | Utilities + digital + supply chain aligned | Steering sign-off pack approved |

---

*For automation sequencing, refer to [`docs/automation-roadmap.md`](./docs/automation-roadmap.md).*  
*For architecture and control integration, refer to [`docs/mes-integration.md`](./docs/mes-integration.md).*  
*For environmental and statutory obligations, refer to [`docs/regulatory.md`](./docs/regulatory.md).*  
*For supply commitments and sourcing posture, refer to [`docs/supply-chain.md`](./docs/supply-chain.md).*  
*For AI/DT posture and closure status, refer to [`docs/ai-platform-status.md`](./docs/ai-platform-status.md) and [`docs/gap-closure-report.md`](./docs/gap-closure-report.md).*
