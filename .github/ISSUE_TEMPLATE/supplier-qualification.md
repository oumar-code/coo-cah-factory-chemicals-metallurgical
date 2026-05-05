---
name: Supplier Qualification
about: Onboard and qualify a new semiconductor, component, or material supplier
title: "[SUPPLIER] Qualify <supplier name> for <component/material>"
labels: supplier, procurement, qualification
assignees: ''
---

## Supplier Details

| Field | Value |
|---|---|
| **Supplier Name** | |
| **Country / Location** | |
| **Component / Material** | <!-- e.g., "Power MOSFETs — Infineon IPP60R080CFD7" --> |
| **BOM Position(s)** | <!-- Which product(s) and PCB position(s) this component is used in --> |
| **Sourcing Type** | <!-- Primary / Alternate / Spot (spot-buy not preferred) --> |
| **Requested By** | |
| **Date Raised** | <!-- YYYY-MM-DD --> |
| **Priority** | <!-- Critical / High / Medium / Low --> |

---

## Qualification Checklist

### Documentation Review
- [ ] ISO 9001:2015 (or equivalent) certificate provided and current
- [ ] Product datasheet reviewed and component meets specification
- [ ] RoHS 3 / REACH compliance declaration provided
- [ ] MSDS / SDS provided (if applicable — chemicals, batteries, solvents)
- [ ] For semiconductors: authorised distribution certificate provided (no grey market)
- [ ] Export control status confirmed (ITAR / EAR, if applicable)

### Technical Qualification
- [ ] Component sample(s) received and inspected
- [ ] Incoming inspection passed (dimensional, electrical, solderability as applicable)
- [ ] SMT / assembly compatibility confirmed (land pattern, package, solderability)
- [ ] Functional test on production PCB confirmed (or simulation / equivalent confirmed)
- [ ] For semiconductors: thermal characterisation and safe operating area (SOA) reviewed
- [ ] Firmware / driver compatibility confirmed (for programmable or smart components)

### Logistics and Commercial
- [ ] Lead time confirmed and acceptable (document below)
- [ ] MOQ (minimum order quantity) acceptable
- [ ] Pricing agreed (attach quote)
- [ ] Incoterms and freight mode confirmed
- [ ] For air freight components (semiconductors): customs clearance route confirmed
- [ ] For DG goods (batteries): IMDG / IATA compliance confirmed

### Safety Stock Assessment
- [ ] Safety stock requirement determined (fill in below)
- [ ] Initial stock purchase order raised or approved

---

## Qualification Data

| Parameter | Value | Pass/Fail |
|---|---|---|
| Datasheet specification | | |
| Sample test result 1 | | |
| Sample test result 2 | | |
| Sample test result 3 | | |
| Lead time (weeks) | | |
| Safety stock requirement | | |
| Transport mode | | |
| Equivalent / alternate part number | | |

---

## Risk Assessment

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| Supply allocation | <!-- H/M/L --> | <!-- H/M/L --> | <!-- 90-day safety stock; dual-source --> |
| Quality variance vs. datasheet | | | |
| Currency / pricing risk | | | |
| Logistics disruption | | | |

---

## Decision

- [ ] **APPROVED** — Supplier added to Approved Supplier List (ASL)
- [ ] **CONDITIONALLY APPROVED** — Conditions: <!-- list conditions -->
- [ ] **REJECTED** — Reason: <!-- state reason -->

**Approver:** <!-- Name -->  
**Approval Date:** <!-- YYYY-MM-DD -->

---

## Supply Chain Document Updates

- [ ] [docs/supply-chain.md](../../docs/supply-chain.md) updated with new supplier
- [ ] Approved Supplier List (ASL) updated in MES
- [ ] Safety stock level entered in MES inventory system

---
*Supplier qualification follows the Coo-Cah Technologies Holdings supply chain doctrine. See master repo [oumar-code/Coo-Kah-Doks](https://github.com/oumar-code/Coo-Kah-Doks) → `docs/standards/supply-chain-doctrine.md`.*
