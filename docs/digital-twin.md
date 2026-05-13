# Digital Twin

> **Factory:** Coo-Cah Metallurgical & Minerals Factory — Warri / Ovwian-Aladja, Delta State
> **Factory ID (Canonical):** `CCH-MET`
> **Digital Twin Asset ID Pattern (Canonical):** `DT-MET-<AREA>-<NNN>`
> **Phase Context:** Factory is Phase 2 in the group rollout

---

## 1. Digital Twin Scope

The metallurgical digital twin provides:

1. **Operational visibility:** real-time equipment state, throughput, energy, and quality status.
2. **Root-cause analysis:** cross-line diagnostics for yield, downtime, and quality drift.
3. **Simulation readiness:** data contracts and topology to run capacity and energy scenarios.

---

## 2. Canonical Naming (Frozen for Gate 3)

| Item | Canonical Value |
| --- | --- |
| Factory ID | `CCH-MET` |
| Zone Schema | `Z1` to `Z14` (see `floor-plan.md`) |
| Asset ID Schema | `DT-MET-<AREA>-<NNN>` |
| Anchor Ref Schema | `ANC-MET-<AREA>-<NNN>` |
| Sensor ID Schema | `SM-<AREA>-<TYPE>-<NNN>` |

---

## 3. Primary Asset Registry (Authoritative for BIM and Sensors)

| Asset ID | Asset Name | Zone ID | DT Phase | Core Data Streams |
| --- | --- | --- | --- | --- |
| DT-MET-EAF-001 | Electric Arc Furnace | Z2 | Phase 2 | Bath temperature, electrode current, power draw, off-gas composition |
| DT-MET-LF-001 | Ladle Furnace | Z3 | Phase 2 | Melt temperature, stir gas flow, power draw |
| DT-MET-CC-001 | Continuous Caster Line 1 | Z4 | Phase 2 | Casting speed, mould temperature, cooling flow |
| DT-MET-CC-002 | Continuous Caster Line 2 | Z4 | Phase 2 | Casting speed, mould temperature, cooling flow |
| DT-MET-SRM-001 | Steel Rolling Mill | Z5 | Phase 2 | Stand torque, strip thickness, line speed |
| DT-MET-SGL-001 | Galvanising Line | Z5 | Phase 2 | Bath temperature, coating weight, strip speed |
| DT-MET-ALR-001 | Aluminium Rolling Mill | Z6 | Phase 2 | Gauge, line speed, roll force |
| DT-MET-AEX-001 | Aluminium Extrusion Press | Z6 | Phase 2 | Ram pressure, billet temperature, profile speed |
| DT-MET-CCR-001 | Copper Continuous Cast & Roll | Z7 | Phase 2 | Melt temperature, rod diameter, line speed |
| DT-MET-WDR-001 | Wire Drawing Line 1 | Z7 | Phase 2 | Capstan speed, wire tension, break events |
| DT-MET-WDR-002 | Wire Drawing Line 2 | Z7 | Phase 2 | Capstan speed, wire tension, break events |
| DT-MET-LAC-001 | Lead Alloy Casting Line | Z8 | Phase 2 | Kettle temperature, alloy chemistry, casting cycle |
| DT-MET-CRS-001 | Primary Crusher | Z9 | Phase 2 | Motor current, throughput, vibration |
| DT-MET-BML-001 | Ball Mill | Z9 | Phase 2 | Feed rate, mill power, bearing vibration |
| DT-MET-FLT-001 | Flotation Bank | Z9 | Phase 2 | Air flow, slurry density, reagent feed |
| DT-MET-THK-001 | Thickener | Z9 | Phase 2 | Underflow density, rake torque, level |
| DT-MET-SUB-001 | Main Substation | Z10 | Phase 2 | Incoming power, PF, breaker events |
| DT-MET-PV-001 | Solar PV Field | Z10 | Phase 2 | PV power, inverter status, yield |
| DT-MET-BESS-001 | BESS Plant | Z10 | Phase 2 | SoC, charge/discharge power, alarms |
| DT-MET-AIR-001 | Compressor Station | Z10 | Phase 2 | Header pressure, compressor load, dew point |
| DT-MET-ETP-001 | Effluent Treatment Plant | Z11 | Phase 2 | pH, flow, turbidity |
| DT-MET-CEMS-001 | Stack Emissions CEMS | Z11 | Phase 2 | NOx, SO2, PM, O2 |
| DT-MET-LAB-001 | QC Lab Instrument Cluster | Z12 | Phase 2 | Chemistry results, tensile results, hardness |
| DT-MET-DCS-001 | DCS/SCADA Core | Z13 | Phase 2 | Tag health, historian ingest, alarm rates |
| DT-MET-MNT-001 | Maintenance Workshop Systems | Z14 | Phase 2 | Work-order status, critical spares status |

---

## 4. Gate 3 Readiness Interfaces

- BIM placement source: `docs/bim/asset-anchors.md`
- Zone geometry source: `docs/bim/zone-boundaries.md`
- Sensor registry source: `docs/sensor-map.md`
- All three files are controlled master data for Phase 2 execution.
