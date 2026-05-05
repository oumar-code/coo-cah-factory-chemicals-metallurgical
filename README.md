# Coo-Cah Garage & Power Electronics Factory

![Status: PLANNED](https://img.shields.io/badge/Status-PLANNED-yellow)
![Tier: 1 — Critical Infrastructure](https://img.shields.io/badge/Tier-1%20Critical%20Infrastructure-red)
![Phase: 1](https://img.shields.io/badge/Phase-1-blue)
![Location: Sagamu, Ogun State, Nigeria](https://img.shields.io/badge/Location-Sagamu%2C%20Ogun%20State-green)
![Vertical: Power Electronics](https://img.shields.io/badge/Vertical-Power%20Electronics-purple)

> **Repository:** `coo-cah-factory-electronics-power`
> **Master Repo:** [oumar-code/Coo-Kah-Doks](https://github.com/oumar-code/Coo-Kah-Doks) — Single source of truth for strategy, architecture, blueprints, and group-wide standards.
> See [MASTER_REPO_REF.md](./MASTER_REPO_REF.md) for full traceability.

---

## Factory Overview

| Attribute | Value |
| --- | --- |
| **Factory Name** | Coo-Cah Garage & Power Electronics Factory |
| **Repository** | `coo-cah-factory-electronics-power` |
| **Location** | Sagamu Industrial Estate, Ogun State, Nigeria |
| **Vertical** | Electronics — Power Electronics Sub-vertical |
| **Tier** | Tier 1 — Critical Infrastructure |
| **Phase** | Phase 1 (Planning / Development) |
| **Status** | PLANNED |
| **Facility Area** | ~12,000 m² |
| **Employees** | ~280 direct, ~60 indirect (Phase 1 target) |
| **Peak Power Load** | ~400 kW |
| **Solar PV** | 600 kWp ground-mount |
| **BESS** | 700 kWh LFP (CATL/BYD containerised) |
| **Backup Generator** | 1 × Perkins 400 kVA diesel (1,500 L tank) |
| **Quality Standards** | ISO 9001:2015 · ISO 45001:2018 · SON NIS · IEC 62040 · IEC 61683 |

---

## Strategic Role — Why This Is Tier 1 Critical

This factory manufactures the **energy resilience products that every other Coo-Cah factory depends upon**. Without it operational, the group's energy independence strategy relies entirely on imported products at unpredictable lead times and prices.

Every Coo-Cah factory in the network requires:

| Product | Recipient Factories | Priority |
| --- | --- | --- |
| Pure Sine Wave Inverters (3 kVA, 5 kVA) | All Coo-Cah factories — backup power | CRITICAL |
| UPS (1 kVA rack-mount) | MES server rooms at every factory site | CRITICAL |
| MPPT Solar Charge Controllers | Coo-Cah energy/infrastructure team — all solar installs | HIGH |
| Smart Surge-Protected Power Strips | All Coo-Cah factories — IT and production workstations | HIGH |
| Power Tools (Drill + Angle Grinder) | All factory maintenance workshops | MEDIUM |

**Internal allocation priority:** All Coo-Cah factories are served before external commercial sales commence. External B2B and retail sales begin when Phase 1 ramp exceeds internal demand.

**Nigerian market context:** Nigeria's inverter + solar market exceeds 2 million units per year and is growing at 15–20% annually. Grid instability (8–12 h/day supply in Sagamu) means virtually every household and business needs backup power. Coo-Cah brand positioning: **premium performance + mid-market price + local warranty**. A 2-year local warranty with a factory-direct aftersales centre in Sagamu creates a durable competitive moat against imported products.

---

## Products (Phase 1)

| SKU Code | Product | Variants | Phase |
| --- | --- | --- | --- |
| CCG-INV-PSW | Pure Sine Wave Inverter | 300VA / 500VA / 1kVA / 2kVA / 3kVA / 5kVA | Phase 1 |
| CCG-INV-MSW | Modified Sine Wave Inverter | 300VA / 500VA / 1kVA / 2kVA | Phase 1 |
| CCG-SCC-MPPT | MPPT Solar Charge Controller | 20A / 40A / 60A / 100A | Phase 1 |
| CCG-SCC-PWM | PWM Solar Charge Controller | 10A / 20A / 30A | Phase 1 |
| CCG-SPK | Solar Panel Kit (packaged) | 100W / 200W / 400W | Phase 1 |
| CCG-BC | Smart Multi-Stage Battery Charger | 12V / 24V / 48V systems | Phase 1 |
| CCG-PS | Surge-Protected Smart Power Strip (Wi-Fi) | 4-way / 6-way / 8-way | Phase 1 |
| CCG-UPS | Line Interactive UPS | 600VA / 1kVA / 2kVA | Phase 1 |
| CCG-PT-DRILL | Electric Drill | Corded 500W/750W · Cordless 18V | Phase 1 |
| CCG-PT-AG | Angle Grinder | 115mm / 125mm (700W–1000W) | Phase 1 |
| CCG-PT-CS | Circular Saw | 165mm / 185mm (1200W–1600W) | Phase 1 |

### Phase 1 Starting Focus (Early Revenue + Internal Demand)

| SKU | Rationale |
| --- | --- |
| CCG-INV-PSW (2kVA + 3kVA) | Highest internal and external demand; flagship product |
| CCG-SCC-MPPT (40A + 60A) | Required by Coo-Cah energy systems team immediately for all solar installs |
| CCG-PS smart power strips | High volume, simple to manufacture, fast production ramp-up |

All other products follow as capacity and workforce scale through Phase 1.

---

## Production Capacity Targets

| Product Line | Phase 1 (2025–2026) | Phase 2 (2027–2028) | Phase 3 (2029–2031) |
| --- | --- | --- | --- |
| Inverters (all sizes) | 200,000 units/year | 450,000 units/year | 700,000 units/year |
| Solar Charge Controllers | 150,000 units/year | 320,000 units/year | 500,000 units/year |
| Battery Chargers | 80,000 units/year | 165,000 units/year | 250,000 units/year |
| Smart Power Strips | 500,000 units/year | 1,000,000 units/year | 1,500,000 units/year |
| UPS | 50,000 units/year | 150,000 units/year | 250,000 units/year |
| Power Tools | 100,000 units/year | 300,000 units/year | 500,000 units/year |

---

## Dependency Map

### This Factory Supplies (Outbound — Internal Priority First)

```text
Coo-Cah Garage & Power Electronics Factory

        |
        |---> ALL Coo-Cah Factories       --> PSW Inverters (3kVA, 5kVA), backup power units
        |---> ALL Factory MES Server Rooms --> UPS (1kVA rack-mount)
        |---> Coo-Cah Energy/Infra Team   --> MPPT Solar Charge Controllers (all solar installs)
        |---> ALL Coo-Cah Factories        --> Smart Power Strips (workstations & equipment)
        |---> ALL Factory Workshops        --> Power Tools (drill, angle grinder)
        '---> External B2B & Retail        --> All products (after internal demand satisfied)
```

### This Factory Receives (Inbound)

```text
Coo-Cah Plastics & Polymers Factory (Agbara, Lagos)
        '--> Plastic enclosures, inverter housings, SCC casings, power strip bodies
             [~60km road; daily delivery; 1-2 day lead time; 7-day safety stock]

External Suppliers

        |---> Infineon / ON Semiconductor (Germany/USA) -- Power MOSFETs, IGBTs [AIR FREIGHT]
        |---> Texas Instruments (USA) -- Gate Driver ICs [AIR FREIGHT]
        |---> Nichicon / Rubycon (Japan) -- Electrolytic capacitors [Air/Sea mixed]
        |---> Baoding Tianwei (China) -- Transformer cores [Sea freight, Tin Can Island]
        |---> Kabelmetal Nigeria + India suppliers -- Magnet wire [Local + import]
        '---> CSB Battery / Vision (Taiwan/HK) -- VRLA batteries for UPS [Sea freight, DG class]
```

---

## Energy Profile Summary

| Parameter | Value |
| --- | --- |
| Facility Area | ~12,000 m² |
| Estimated Peak Load | ~400 kW |
| Daily Energy Consumption | ~2,800 kWh/day |
| Solar PV | 600 kWp — Ground-mount (Sagamu east land; also provides car park shade) |
| BESS | 700 kWh LFP — CATL/BYD containerised |
| Solar Irradiance | 4.7 PSH/day average; 4.5 PSH/day worst month |
| Target Solar Self-Sufficiency | >= 80% |
| Grid Supply (Sagamu DISCO) | ~8–12 h/day — factory designed to operate grid-independently |
| Backup Generator | 1 × Perkins 400 kVA diesel; 1,500 L tank (~60 h at 40% load) |

> Ground-mount solar is preferred over rooftop at this site: Sagamu has available land to the east of the building, avoiding rooftop structural loading. The array also provides covered car parking for staff.

---

## Phase 1 Milestone Checklist

- [ ] **Q2 2025** — Factory site acquisition confirmed, Sagamu Industrial Estate
- [ ] **Q3 2025** — NESREA EIA submission and approval
- [ ] **Q3 2025** — NIPC Pioneer Status application filed (5-year CIT holiday target)
- [ ] **Q3 2025** — Architectural drawings and MEP design completed
- [ ] **Q4 2025** — Main building civil works commenced
- [ ] **Q1 2026** — SMT line equipment ordered and shipping confirmed
- [ ] **Q1 2026** — 600 kWp ground solar + 700 kWh BESS procurement tendered
- [ ] **Q2 2026** — Building shell complete; electrical and HVAC installation
- [ ] **Q2 2026** — SMT line installed and commissioned
- [ ] **Q3 2026** — Ground solar + BESS commissioned; generator on standby
- [ ] **Q3 2026** — MES platform deployed across all factory zones
- [ ] **Q3 2026** — AMR fleet (12 units) deployed
- [ ] **Q3 2026** — Transformer winding cells operational (manual Phase 1)
- [ ] **Q4 2026** — First CCG-INV-PSW (2kVA) load bank tested and passed
- [ ] **Q4 2026** — First CCG-SCC-MPPT (40A) production run
- [ ] **Q4 2026** — SON NIS certification application submitted for Phase 1 SKUs
- [ ] **Q1 2027** — Phase 1 internal supply obligations met (inverters, UPS, controllers to sister factories)
- [ ] **Q2 2027** — External commercial sales launched
- [ ] **Q2 2027** — SON NIS certification received; C-Mark on packaging

---

## Documentation

| Document | Description |
| --- | --- |
| [MASTER_REPO_REF.md](./MASTER_REPO_REF.md) | Link to Coo-Kah-Doks master repo; standards traceability |
| [docs/machinery.md](./docs/machinery.md) | Full equipment register — SMT, winding, assembly, test, AMR, packaging |
| [docs/energy-profile.md](./docs/energy-profile.md) | 600 kWp solar, 700 kWh BESS, energy cost model, grid independence |
| [docs/floor-plan.md](./docs/floor-plan.md) | 12,000 m² factory layout — all zones, solar yard, BESS pad |
| [docs/automation-roadmap.md](./docs/automation-roadmap.md) | Phase 1 to Phase 3 automation strategy |
| [docs/supply-chain.md](./docs/supply-chain.md) | Semiconductor sourcing, intra-group supply, DG logistics, market sizing |
| [docs/regulatory.md](./docs/regulatory.md) | SON, NCC, IEC standards, NESREA, Pioneer Status |
| [docs/capex-opex.md](./docs/capex-opex.md) | CapEx plan, unit economics, BOM cost model, payback analysis |
| [docs/digital-twin.md](./docs/digital-twin.md) | Asset registry, SMT + winding DT, load bank integration, energy monitoring |
| [docs/mes-integration.md](./docs/mes-integration.md) | Serial traceability, IEC 62040 test records, load bank Ethernet, SON label printing |

---

*Part of the Coo-Cah Technologies Holdings Manufacturing Ecosystem. All documents in this repository are consistent with and traceable to the master orchestration repository [oumar-code/Coo-Kah-Doks](https://github.com/oumar-code/Coo-Kah-Doks).*
