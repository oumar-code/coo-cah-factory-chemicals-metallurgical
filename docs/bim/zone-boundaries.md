# BIM Zone Boundaries (Gate 3 Spatial Master)

> **Factory:** Coo-Cah Metallurgical & Minerals Factory
> **Authority Level:** Authoritative for zone geometry references

---

## 1. Coordinate Reference Standard

| Field | Value |
| --- | --- |
| Primary CRS | `LCS-MET-001` local Cartesian grid |
| Local Origin | South-west survey control point of site (`X=0, Y=0, Z=0`) |
| Axis Convention | `+X` East, `+Y` North, `+Z` Up |
| Optional Geodetic Tie | WGS84 / UTM Zone 32N (`EPSG:32632`) |
| Unit | metres |

---

## 2. Required Zone Fields

Each zone row must include: `Zone ID`, `Zone Name`, `Min X`, `Min Y`, `Max X`, `Max Y`, `Base Z`, `Top Z`, and `Boundary Polygon Ref`.

---

## 3. Zone Boundary Register

| Zone ID | Zone Name | Min X | Min Y | Max X | Max Y | Base Z | Top Z | Boundary Polygon Ref |
| --- | --- | ---: | ---: | ---: | ---: | ---: | ---: | --- |
| Z1 | Raw Material Receiving & Scrap Yard | 0 | 0 | 140 | 110 | 0 | 12 | POLY-Z1 |
| Z2 | EAF & Primary Melting Bay | 150 | 0 | 290 | 120 | 0 | 28 | POLY-Z2 |
| Z3 | Ladle Furnace & Secondary Refining | 300 | 0 | 420 | 120 | 0 | 26 | POLY-Z3 |
| Z4 | Continuous Casting Bay | 430 | 0 | 580 | 130 | 0 | 24 | POLY-Z4 |
| Z5 | Steel Rolling & Finishing | 590 | 0 | 860 | 150 | 0 | 22 | POLY-Z5 |
| Z6 | Aluminium Rolling & Extrusion | 590 | 160 | 860 | 300 | 0 | 20 | POLY-Z6 |
| Z7 | Copper Rod & Wire Drawing | 430 | 160 | 580 | 300 | 0 | 20 | POLY-Z7 |
| Z8 | Lead Alloy Casting | 300 | 130 | 420 | 240 | 0 | 18 | POLY-Z8 |
| Z9 | Mineral Processing | 150 | 130 | 290 | 300 | 0 | 20 | POLY-Z9 |
| Z10 | Utilities & Energy | 0 | 120 | 140 | 250 | 0 | 16 | POLY-Z10 |
| Z11 | ETP & Environmental | 0 | 260 | 140 | 340 | 0 | 15 | POLY-Z11 |
| Z12 | Quality Control Laboratory | 150 | 310 | 290 | 380 | 0 | 12 | POLY-Z12 |
| Z13 | DCS/SCADA/IT Control Room | 300 | 250 | 420 | 340 | 0 | 12 | POLY-Z13 |
| Z14 | Maintenance, Stores & Emergency | 430 | 310 | 580 | 390 | 0 | 14 | POLY-Z14 |

---

## 4. Governance

Owner: BIM Coordinator  
Reviewer: Process Engineering Lead  
Change Control: update only through Gate 3 spatial review workflow.
