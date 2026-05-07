# Master Repository Reference

## Orchestrating Repository

| Attribute | Value |
|---|---|
| **Repository** | <a href="https://github.com/oumar-code/Coo-Kah-Doks">oumar-code/Coo-Kah-Doks</a> |
| **Purpose** | Single source of truth for Coo-Cah Technologies Holdings — strategy, architecture, blueprints, and group-wide standards |
| **Template Version Used** | v1.0 |
| **Factory Registration** | `orchestration/factory-status-registry.md` → entry: `CCH-MET` |

---

## Factory Blueprint Source

This repository was seeded from the following master repo paths:

| Master Repo Path | Content Used |
|---|---|
| `factories/chemicals/metallurgical/` | Factory-level blueprints — product specs, capacity targets, equipment lists, energy profile, regulatory requirements |
| `factories/_template/` | Standard document template formats — section structures, table conventions, Mermaid diagram styles |

---

## Group-Wide Standards Applied

| Standard Area | Master Repo Document | Applied In |
|---|---|---|
| ISO 9001:2015 — Quality Management | `docs/standards/iso-requirements.md` | `docs/regulatory.md` |
| ISO 14001:2015 — Environmental | `docs/standards/iso-requirements.md` | `docs/regulatory.md` |
| ISO 45001:2018 — Health &amp; Safety | `docs/standards/iso-requirements.md` | `docs/regulatory.md` |
| ISO 50001:2018 — Energy | `docs/standards/iso-requirements.md` | `docs/energy-profile.md` |
| Automation Phases Framework | `docs/standards/automation-phases.md` | `docs/automation-roadmap.md` |
| Supply Chain Doctrine | `docs/standards/supply-chain-doctrine.md` | `docs/supply-chain.md` |
| Energy Strategy | `docs/standards/energy-strategy.md` | `docs/energy-profile.md` |
| AI Platform Standards | `docs/standards/ai-platform.md` | `docs/digital-twin.md`, `docs/automation-roadmap.md` |
| MES Integration Standards | `docs/standards/mes-integration-standards.md` | `docs/mes-integration.md` |
| Factory Blueprint Template | `factories/_template/` | All `docs/` files |
| Metallurgical Factory Blueprint | `factories/chemicals/metallurgical/` | All `docs/` files |

---

## Confirmation of Compliance

1. **Standards Compliance:** All documents follow group-wide standards as defined in `oumar-code/Coo-Kah-Doks`. Any deviation requires an approved RFC in the master repo before implementation.
2. **Template Version:** Document structure follows template v1.0. When the master repo releases a new template version, this factory repo must be updated within 30 days via a dedicated PR.
3. **Factory Status Registry:** This factory (`CCH-MET`) is registered in `orchestration/factory-status-registry.md` with status `PLANNED`. The registry must be updated whenever factory status changes.
4. **Cross-Factory Dependencies:** All intra-group supply relationships documented in `docs/supply-chain.md` are mirrored in the master repo's `orchestration/supply-chain-map.md`.
5. **Energy Strategy Alignment:** The 1,000 kWp + 1,200 kWh BESS configuration is registered in the group energy master plan. The high BESS capacity reflects the 2,500 kW peak load from electric arc furnace and rolling mill inrush demands.
6. **MES Platform:** This factory uses the group-standard MES platform. No proprietary MES modifications are made without master repo RFC approval.
7. **NESREA Heavy Industry Compliance:** Full EIA, ETP discharge monitoring, acid/rinse neutralisation tracking, and NESREA monthly compliance reports are tracked in the MES Environmental Module — mandatory for metals processing in Nigeria.

---

## Related Repositories

| Repository | Relationship |
|---|---|
| <a href="https://github.com/oumar-code/Coo-Kah-Doks">oumar-code/Coo-Kah-Doks</a> | Master orchestrating repo |
| `coo-cah-factory-electronics-power` | Primary intra-group customer — copper wire rod (transformer/inductor windings) |
| `coo-cah-factory-electronics-kitchen` | Intra-group customer — aluminium sheet (appliance bodies, heat exchangers) |
| `coo-cah-factory-electronics-personal` | Intra-group customer — aluminium extrusion profiles (device chassis) |
| `coo-cah-factory-chemicals-plastics` | Intra-group customer — lead-acid battery grid alloy |
| `coo-cah-factory-chemicals-fine-chemicals` | Sister factory (Chemicals vertical) |

---

## Version History

| Date | Version | Change | Author |
|---|---|---|---|
| 2025-Q2 | 1.0.0 | Initial factory repository created from master repo blueprint | Coo-Cah Factory Dev Team |

---

*For questions about master repo standards or template updates, open an issue in <a href="https://github.com/oumar-code/Coo-Kah-Doks">oumar-code/Coo-Kah-Doks</a>.*
