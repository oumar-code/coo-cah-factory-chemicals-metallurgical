# DT Connectivity Evidence Pack

> **Factory:** Coo-Cah Metallurgical & Minerals Factory
> **Purpose:** Trace-pack index for proving OT → MES → DT connectivity on critical assets

---

## Required trace packs

| Asset | Zone | Evidence File | Owner | Current Status |
| --- | --- | --- | --- | --- |
| Electric Arc Furnace | Z2 | [`eaf-z2.md`](./eaf-z2.md) | OT Integration Lead | Planned |
| Wire Drawing Line 1 | Z7 | [`wire-draw-z7.md`](./wire-draw-z7.md) | MES Product Owner | Planned |
| BESS Plant | Z10 | [`bess-z10.md`](./bess-z10.md) | Energy Systems Lead | Planned |

---

## Minimum acceptance rule

Each trace pack must show the same event or telemetry sample across:

1. OT source
2. MES receipt or historian entry
3. DT state-store or simulation-trigger record

No file in this folder may be treated as `Live` until the timestamps, asset IDs, and signal names are visible in committed evidence.
