# BIM Reference Index

> **Factory:** Coo-Cah Metallurgical & Minerals Factory
> **Purpose:** Canonical index for Gate 3 BIM and DT spatial master data

---

## Gate 3 BIM document set

| Document | Role in Gate 3 process | Authority |
| --- | --- | --- |
| [`zone-boundaries.md`](./zone-boundaries.md) | Defines the canonical zone geometry, coordinate ranges, and boundary references used by BIM placement and DT zone assignment. | Spatial master for zone geometry |
| [`asset-anchors.md`](./asset-anchors.md) | Defines the canonical anchor coordinates and orientation for DT assets placed in the BIM model. | Spatial master for asset placement |
| [`../sensor-map.md`](../sensor-map.md) | Links each sensor to its zone, asset, and anchor so telemetry can be mounted onto the BIM and DT topology. | Sensor master for BIM/DT linkage |

---

## Usage order

1. Confirm the zone geometry in [`zone-boundaries.md`](./zone-boundaries.md).
2. Confirm the asset anchor in [`asset-anchors.md`](./asset-anchors.md).
3. Confirm the sensor-to-asset-to-anchor mapping in [`../sensor-map.md`](../sensor-map.md).
4. Use the canonical IDs from [`../digital-twin.md`](../digital-twin.md) and [`../floor-plan.md`](../floor-plan.md) without local variation.

---

## Control rules

- `Z1` to `Z14` remain the only valid zone identifiers for this factory.
- `DT-MET-<AREA>-<NNN>` remains the only valid DT asset ID schema.
- `ANC-MET-<AREA>-<NNN>` remains the only valid BIM anchor schema.
- Any anchor move must be reflected in `asset-anchors.md` and `../sensor-map.md` in the same change set.

---

## Related DT readiness artifacts

| Artifact | Purpose |
| --- | --- |
| [`../dt-evidence-index.md`](../dt-evidence-index.md) | Maps hard release conditions to evidence artifacts and status |
| [`../dt-data-quality-scorecard.md`](../dt-data-quality-scorecard.md) | Tracks data completeness, freshness, and schema validity for DT-critical streams |
| [`../dt-governance-log.md`](../dt-governance-log.md) | Records weekly DT/MES/OT readiness reviews and blockers |
