# Sensor Map (Gate 3 Sensor Master)

> **Factory:** Coo-Cah Metallurgical & Minerals Factory
> **Authority Level:** Authoritative sensor registry for BIM and simulation

---

## 1. Required Sensor Fields

`Sensor ID`, `Sensor Model`, `Sensor Type`, `Zone ID`, `Asset ID`, `Anchor Ref`, `Protocol`, `Sample Rate`, `Calibration Interval`, `Simulation Use`.

---

## 2. Critical Sensor Registry (Wave A Baseline)

| Sensor ID | Sensor Model | Sensor Type | Zone ID | Asset ID | Anchor Ref | Protocol | Sample Rate | Calibration Interval | Simulation Use |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SM-EAF-TEMP-001 | PYRO-IR-900 | Bath temperature | Z2 | DT-MET-EAF-001 | ANC-MET-EAF-001 | OPC-UA | 1s | 30 days | Melt energy balance |
| SM-EAF-CURR-001 | ION-CT-20KA | Electrode current | Z2 | DT-MET-EAF-001 | ANC-MET-EAF-001 | OPC-UA | 1s | 90 days | Power and stability |
| SM-EAF-GAS-001 | GAS-QM-6 | Off-gas analyzer | Z2 | DT-MET-EAF-001 | ANC-MET-EAF-001 | Modbus TCP | 5s | 30 days | Carbon and oxygen trend |
| SM-LF-TEMP-001 | THM-K-1800 | Ladle temperature | Z3 | DT-MET-LF-001 | ANC-MET-LF-001 | OPC-UA | 1s | 30 days | Refining endpoint |
| SM-LF-FLOW-001 | FLOW-ARG-100 | Argon flow | Z3 | DT-MET-LF-001 | ANC-MET-LF-001 | OPC-UA | 2s | 90 days | Stirring efficiency |
| SM-CC-SPD-001 | ENC-CAST-01 | Casting speed | Z4 | DT-MET-CC-001 | ANC-MET-CC-001 | OPC-UA | 1s | 180 days | Throughput model |
| SM-CC-TEMP-001 | THM-MOULD-01 | Mould temp | Z4 | DT-MET-CC-001 | ANC-MET-CC-001 | OPC-UA | 1s | 30 days | Breakout risk |
| SM-CC-FLOW-001 | FLOW-WTR-01 | Cooling water flow | Z4 | DT-MET-CC-001 | ANC-MET-CC-001 | Modbus TCP | 2s | 90 days | Thermal stability |
| SM-CC-SPD-002 | ENC-CAST-02 | Casting speed | Z4 | DT-MET-CC-002 | ANC-MET-CC-002 | OPC-UA | 1s | 180 days | Throughput model |
| SM-CC-TEMP-002 | THM-MOULD-02 | Mould temp | Z4 | DT-MET-CC-002 | ANC-MET-CC-002 | OPC-UA | 1s | 30 days | Breakout risk |
| SM-SRM-GAUGE-001 | XRY-GAUGE-01 | Strip thickness | Z5 | DT-MET-SRM-001 | ANC-MET-SRM-001 | OPC-UA | 1s | 30 days | Yield and quality |
| SM-SRM-TORQ-001 | TORQ-ROLL-01 | Stand torque | Z5 | DT-MET-SRM-001 | ANC-MET-SRM-001 | OPC-UA | 1s | 90 days | Bottleneck model |
| SM-SRM-SPD-001 | ENC-ROLL-01 | Line speed | Z5 | DT-MET-SRM-001 | ANC-MET-SRM-001 | OPC-UA | 1s | 180 days | Throughput model |
| SM-SGL-TEMP-001 | THM-ZINC-01 | Zinc bath temp | Z5 | DT-MET-SGL-001 | ANC-MET-SGL-001 | OPC-UA | 2s | 30 days | Coating quality |
| SM-SGL-COAT-001 | COAT-XRF-01 | Coating weight | Z5 | DT-MET-SGL-001 | ANC-MET-SGL-001 | OPC-UA | 5s | 30 days | Quality compliance |
| SM-ALR-GAUGE-001 | XRY-AL-01 | Aluminium gauge | Z6 | DT-MET-ALR-001 | ANC-MET-ALR-001 | OPC-UA | 1s | 30 days | Product tolerance |
| SM-ALR-FORCE-001 | LOAD-ROLL-AL1 | Roll force | Z6 | DT-MET-ALR-001 | ANC-MET-ALR-001 | OPC-UA | 1s | 90 days | Pass schedule model |
| SM-AEX-PRES-001 | PRESS-5000T-01 | Ram pressure | Z6 | DT-MET-AEX-001 | ANC-MET-AEX-001 | OPC-UA | 1s | 90 days | Extrusion productivity |
| SM-AEX-TEMP-001 | THM-BILLET-01 | Billet temp | Z6 | DT-MET-AEX-001 | ANC-MET-AEX-001 | OPC-UA | 1s | 30 days | Surface defect risk |
| SM-CCR-DIA-001 | LASER-DIA-01 | Rod diameter | Z7 | DT-MET-CCR-001 | ANC-MET-CCR-001 | OPC-UA | 1s | 30 days | Dimensional control |
| SM-CCR-SPD-001 | ENC-CCR-01 | Line speed | Z7 | DT-MET-CCR-001 | ANC-MET-CCR-001 | OPC-UA | 1s | 180 days | Throughput model |
| SM-WDR-TEN-001 | TEN-WIRE-01 | Wire tension | Z7 | DT-MET-WDR-001 | ANC-MET-WDR-001 | OPC-UA | 1s | 30 days | Breakage prediction |
| SM-WDR-SPD-001 | ENC-WDR-01 | Capstan speed | Z7 | DT-MET-WDR-001 | ANC-MET-WDR-001 | OPC-UA | 1s | 180 days | Capacity model |
| SM-WDR-TEN-002 | TEN-WIRE-02 | Wire tension | Z7 | DT-MET-WDR-002 | ANC-MET-WDR-002 | OPC-UA | 1s | 30 days | Breakage prediction |
| SM-WDR-SPD-002 | ENC-WDR-02 | Capstan speed | Z7 | DT-MET-WDR-002 | ANC-MET-WDR-002 | OPC-UA | 1s | 180 days | Capacity model |
| SM-LAC-TEMP-001 | THM-PB-01 | Kettle temperature | Z8 | DT-MET-LAC-001 | ANC-MET-LAC-001 | OPC-UA | 2s | 30 days | Alloy quality |
| SM-LAC-CHEM-001 | OES-LAB-01 | Alloy chemistry | Z8 | DT-MET-LAC-001 | ANC-MET-LAC-001 | REST | per batch | 7 days | Composition control |
| SM-CRS-CURR-001 | CURR-CRUSH-01 | Crusher motor current | Z9 | DT-MET-CRS-001 | ANC-MET-CRS-001 | Modbus TCP | 1s | 90 days | Load and downtime |
| SM-BML-VIB-001 | VIB-MILL-01 | Mill vibration | Z9 | DT-MET-BML-001 | ANC-MET-BML-001 | OPC-UA | 1s | 30 days | Predictive maintenance |
| SM-BML-POW-001 | PWR-MILL-01 | Mill power draw | Z9 | DT-MET-BML-001 | ANC-MET-BML-001 | Modbus TCP | 1s | 90 days | Energy intensity |
| SM-FLT-DENS-001 | DENS-SLURRY-01 | Slurry density | Z9 | DT-MET-FLT-001 | ANC-MET-FLT-001 | OPC-UA | 2s | 30 days | Recovery simulation |
| SM-THK-LEVEL-001 | LVL-THK-01 | Thickener level | Z9 | DT-MET-THK-001 | ANC-MET-THK-001 | OPC-UA | 2s | 30 days | Water balance |
| SM-SUB-PWR-001 | MTR-11KV-01 | Incoming power | Z10 | DT-MET-SUB-001 | ANC-MET-SUB-001 | Modbus TCP | 1s | 90 days | Site energy model |
| SM-PV-PWR-001 | INV-PV-01 | PV output power | Z10 | DT-MET-PV-001 | ANC-MET-PV-001 | MQTT | 5s | 180 days | Renewable profile |
| SM-BESS-SOC-001 | BMS-SOC-01 | Battery SoC | Z10 | DT-MET-BESS-001 | ANC-MET-BESS-001 | MQTT | 5s | 30 days | Dispatch simulation |
| SM-AIR-PRES-001 | PRES-AIR-01 | Header pressure | Z10 | DT-MET-AIR-001 | ANC-MET-AIR-001 | OPC-UA | 2s | 90 days | Utility stability |
| SM-ETP-PH-001 | PH-ETP-01 | Effluent pH | Z11 | DT-MET-ETP-001 | ANC-MET-ETP-001 | Modbus TCP | 5s | 30 days | Compliance constraints |
| SM-ETP-FLOW-001 | FLOW-ETP-01 | Effluent flow | Z11 | DT-MET-ETP-001 | ANC-MET-ETP-001 | Modbus TCP | 5s | 90 days | Mass balance |
| SM-CEMS-NOX-001 | CEMS-NOX-01 | NOx concentration | Z11 | DT-MET-CEMS-001 | ANC-MET-CEMS-001 | Modbus TCP | 10s | 30 days | Emissions scenario |
| SM-CEMS-PM-001 | CEMS-PM-01 | PM concentration | Z11 | DT-MET-CEMS-001 | ANC-MET-CEMS-001 | Modbus TCP | 10s | 30 days | Emissions scenario |
| SM-LAB-CHEM-001 | LIMS-CHEM-01 | Chemistry assay stream | Z12 | DT-MET-LAB-001 | ANC-MET-LAB-001 | REST | per test | 7 days | Quality correlation |
| SM-DCS-HEALTH-001 | DCS-HLTH-01 | Tag health metric | Z13 | DT-MET-DCS-001 | ANC-MET-DCS-001 | OPC-UA | 10s | 30 days | Data completeness |
| SM-MNT-SPARE-001 | CMMS-SPR-01 | Critical spares status | Z14 | DT-MET-MNT-001 | ANC-MET-MNT-001 | REST | 60s | 30 days | Downtime risk |

---

## 3. Wave B Expansion Scope

Wave B expands this registry with additional quality, downtime, and energy detail sensors per line while preserving the same ID schemas and zone/asset/anchor links.

---

## 4. Governance

Owner: OT Instrumentation Lead  
Reviewer: Digital Twin Engineer  
Change Control: updates must preserve referential integrity with zone and anchor master files.
