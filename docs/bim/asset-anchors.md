# BIM Asset Anchors (Gate 3 Spatial Master)

> **Factory:** Coo-Cah Metallurgical & Minerals Factory
> **Authority Level:** Authoritative for asset placement in BIM and sensor linking

---

## 1. Required Asset Anchor Fields

`Anchor Ref`, `Asset ID`, `Asset Name`, `Zone ID`, `X`, `Y`, `Z`, `Yaw Deg`, `Pitch Deg`, `Roll Deg`.

---

## 2. Asset Anchor Register

| Anchor Ref | Asset ID | Asset Name | Zone ID | X | Y | Z | Yaw Deg | Pitch Deg | Roll Deg |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: | ---: | ---: |
| ANC-MET-EAF-001 | DT-MET-EAF-001 | Electric Arc Furnace | Z2 | 220 | 60 | 0 | 90 | 0 | 0 |
| ANC-MET-LF-001 | DT-MET-LF-001 | Ladle Furnace | Z3 | 350 | 58 | 0 | 90 | 0 | 0 |
| ANC-MET-CC-001 | DT-MET-CC-001 | Continuous Caster Line 1 | Z4 | 470 | 42 | 0 | 90 | 0 | 0 |
| ANC-MET-CC-002 | DT-MET-CC-002 | Continuous Caster Line 2 | Z4 | 520 | 86 | 0 | 90 | 0 | 0 |
| ANC-MET-SRM-001 | DT-MET-SRM-001 | Steel Rolling Mill | Z5 | 700 | 70 | 0 | 90 | 0 | 0 |
| ANC-MET-SGL-001 | DT-MET-SGL-001 | Galvanising Line | Z5 | 790 | 118 | 0 | 90 | 0 | 0 |
| ANC-MET-ALR-001 | DT-MET-ALR-001 | Aluminium Rolling Mill | Z6 | 690 | 205 | 0 | 90 | 0 | 0 |
| ANC-MET-AEX-001 | DT-MET-AEX-001 | Aluminium Extrusion Press | Z6 | 780 | 250 | 0 | 45 | 0 | 0 |
| ANC-MET-CCR-001 | DT-MET-CCR-001 | Copper Continuous Cast & Roll | Z7 | 480 | 208 | 0 | 90 | 0 | 0 |
| ANC-MET-WDR-001 | DT-MET-WDR-001 | Wire Drawing Line 1 | Z7 | 510 | 255 | 0 | 90 | 0 | 0 |
| ANC-MET-WDR-002 | DT-MET-WDR-002 | Wire Drawing Line 2 | Z7 | 548 | 255 | 0 | 90 | 0 | 0 |
| ANC-MET-LAC-001 | DT-MET-LAC-001 | Lead Alloy Casting Line | Z8 | 360 | 180 | 0 | 0 | 0 | 0 |
| ANC-MET-CRS-001 | DT-MET-CRS-001 | Primary Crusher | Z9 | 205 | 185 | 0 | 0 | 0 | 0 |
| ANC-MET-BML-001 | DT-MET-BML-001 | Ball Mill | Z9 | 245 | 232 | 0 | 0 | 0 | 0 |
| ANC-MET-FLT-001 | DT-MET-FLT-001 | Flotation Bank | Z9 | 260 | 272 | 0 | 0 | 0 | 0 |
| ANC-MET-THK-001 | DT-MET-THK-001 | Thickener | Z9 | 192 | 272 | 0 | 0 | 0 | 0 |
| ANC-MET-SUB-001 | DT-MET-SUB-001 | Main Substation | Z10 | 72 | 170 | 0 | 180 | 0 | 0 |
| ANC-MET-PV-001 | DT-MET-PV-001 | Solar PV Field | Z10 | 38 | 226 | 0 | 180 | 0 | 0 |
| ANC-MET-BESS-001 | DT-MET-BESS-001 | BESS Plant | Z10 | 112 | 215 | 0 | 180 | 0 | 0 |
| ANC-MET-AIR-001 | DT-MET-AIR-001 | Compressor Station | Z10 | 90 | 145 | 0 | 180 | 0 | 0 |
| ANC-MET-ETP-001 | DT-MET-ETP-001 | Effluent Treatment Plant | Z11 | 74 | 298 | 0 | 0 | 0 | 0 |
| ANC-MET-CEMS-001 | DT-MET-CEMS-001 | Stack Emissions CEMS | Z11 | 121 | 315 | 0 | 0 | 0 | 0 |
| ANC-MET-LAB-001 | DT-MET-LAB-001 | QC Lab Instrument Cluster | Z12 | 210 | 345 | 0 | 0 | 0 | 0 |
| ANC-MET-DCS-001 | DT-MET-DCS-001 | DCS/SCADA Core | Z13 | 360 | 300 | 0 | 0 | 0 | 0 |
| ANC-MET-MNT-001 | DT-MET-MNT-001 | Maintenance Workshop Systems | Z14 | 498 | 346 | 0 | 0 | 0 | 0 |

---

## 3. Governance

Owner: Digital Twin Engineer  
Reviewer: OT Integration Lead  
Change Control: any asset move must update this file and `docs/sensor-map.md` in same change set.
