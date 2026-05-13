# Metallurgical — Intra-Group Supply Coordination

> **Gate 3 Artifact (Supply Chain Readiness)**
> **Factory:** Coo-Cah Metallurgical & Minerals Factory | **Location:** Warri / Ovwian-Aladja Steel Corridor, Delta State
> **Document Version:** 1.0 | **Owner:** Supply Chain & Procurement Team
> **Counter-parties:** Power Electronics | Kitchen Electronics | Personal Electronics | Plastics & Polymers

---

## 1. Purpose

This document records formal intra-group supply commitments for Phase 1 readiness and aligns with the sourcing and logistics strategy in [`supply-chain.md`](./supply-chain.md).

---

## 2. Outbound Supply Commitments

### 2.1 Power Electronics Factory — Copper Wire Rod and Drawn Wire

| Parameter | Value |
| --- | --- |
| Supplier Factory | Coo-Cah Metallurgical & Minerals Factory (Warri) |
| Buyer Factory | Coo-Cah Power Electronics Factory |
| Agreement Reference | `INTRA-MET-PWR-2026-001` |
| Product Scope | ETP copper wire rod + drawn winding wire |
| Commitment Horizon | Rolling quarterly plan with monthly freeze |

| SKU | Product | Committed Volume / Month | Lead Time | Status |
| --- | --- | --- | --- | --- |
| CCH-MET-005 | Copper wire rod (ETP) | 650 tonnes | 7 business days | ✅ Confirmed |
| CCH-MET-005A | Drawn winding wire | 220 tonnes | 7 business days | ✅ Confirmed |

### 2.2 Kitchen + Personal Electronics — Aluminium Feedstock

| Buyer | Product | Committed Volume / Month | Lead Time | Status |
| --- | --- | --- | --- | --- |
| Kitchen Electronics | Aluminium sheet/coil (1050, 3003, 5052) | 420 tonnes | 8 business days | ✅ Confirmed |
| Personal Electronics | Aluminium extrusion profiles (6060/6063) | 180 tonnes | 8 business days | ✅ Confirmed |

### 2.3 Plastics & Polymers — Lead-Alloy Supply

| Buyer | Product | Committed Volume / Month | Lead Time | Status |
| --- | --- | --- | --- | --- |
| Plastics & Polymers | Pb-Sb / Pb-Ca lead battery grid alloy | 110 tonnes | 6 business days | ✅ Confirmed |

---

## 3. Capacity Buffer and Escalation

| Condition | Protocol |
| --- | --- |
| Demand increase above 15% vs monthly freeze | 10-business-day advance notice and joint capacity review |
| Critical input constraint (copper cathode/aluminium ingot/billet) | Escalation to Group Supply Chain Director within 24 hours |
| Quality hold on outbound lot | MES quality hold alert + replacement plan within 48 hours |
| Port/logistics disruption on import-dependent inputs | Activate contingency inventory and revised dispatch schedule |

---

## 4. Quality and Acceptance Criteria

| Product Family | Acceptance Baseline |
| --- | --- |
| Copper rod/wire | Conductivity and mechanical conformance to internal ETP specification |
| Aluminium sheet/extrusion | Alloy chemistry and dimensional tolerances per approved SKU datasheets |
| Lead alloy | Chemistry window and contamination controls per battery-grid alloy standard |
| Steel structural products | Grade and coating checks per approved customer QA criteria |

All deliveries include COC, lot traceability ID, and linked quality certificate in MES.

---

## 5. MES-to-MES Integration for Intra-Group Flows

| Data Exchange | Direction | Frequency |
| --- | --- | --- |
| Dispatch schedule and confirmed quantities | Metallurgical MES → Recipient MES | Hourly |
| Order forecast updates | Recipient MES → Metallurgical MES | Hourly |
| Quality hold/release notifications | Bidirectional | Real-time |
| Delivery ETA and POD confirmation | Bidirectional | Real-time |

Integration contracts follow the architecture in [`mes-integration.md`](./mes-integration.md).

---

## Related Documents

| Document | Purpose |
| --- | --- |
| [`supply-chain.md`](./supply-chain.md) | Core sourcing strategy and risk posture |
| [`mes-integration.md`](./mes-integration.md) | API and data exchange model for intra-group coordination |
| [`gap-closure-report.md`](./gap-closure-report.md) | Readiness closure evidence for supply coordination artifacts |
