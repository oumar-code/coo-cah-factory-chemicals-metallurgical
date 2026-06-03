# DT KPI Dictionary

> **Factory:** Coo-Cah Metallurgical & Minerals Factory
> **Purpose:** Locked KPI formulas and proof thresholds for the first 3 DT simulation tracks
> **Rule:** These formulas must be frozen before any simulation run is accepted as evidence

---

## KPI register

| KPI | Formula | Numerator | Denominator | Frequency | Owner | Target | Minimum Proof Threshold |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Rolling throughput rate | Total good rolled tonnes / runtime hour | Good rolled tonnes from Z5 orders | Runtime hours with valid rolling-speed telemetry | Shift | DT Engineering Lead | Improvement vs. baseline window | Statistically valid uplift vs. matched-control or baseline window |
| Copper draw output rate | Good copper output kg / runtime hour | Good copper output kg from Z7 production records | Runtime hours with valid draw-speed telemetry | Shift | DT Engineering Lead | Improvement vs. baseline window | Statistically valid uplift vs. matched-control or baseline window |
| Rolling yield loss rate | Yield loss tonnes / total input tonnes | Scrap, trim, and yield-loss tonnes from Z2-Z5 genealogy | Total input tonnes processed | Daily | MES Product Owner | Reduction vs. baseline | Statistically valid reduction vs. matched-control or baseline window |
| Dimensional conformance rate | In-spec coils or lots / total inspected coils or lots | Count of in-spec gauge or diameter results | Total inspected coils or lots | Shift | QA Lead | Improvement vs. baseline | Statistically valid improvement with no adverse drift in other critical quality KPIs |
| Defect event rate | Quality defect events / 1,000 units or lots | Out-of-spec defect event count | Units or lots produced × 1,000 | Daily | QA Lead | Reduction vs. baseline | Statistically valid reduction vs. matched-control or baseline window |
| Peak-shaving effectiveness | Baseline peak kW - simulated peak kW | Baseline site peak demand in comparable window | Simulated or intervention peak demand in matched window | Daily | Energy Systems Lead | Lower peak demand | Peak reduction demonstrated with no unplanned production curtailment |
| Grid-import intensity | Grid kWh / good tonne | Grid-import kWh from Z10 utility metering | Good tonnes produced in matched period | Daily | Energy Systems Lead | Reduction vs. baseline | Statistically valid reduction with production output held within control bounds |
| BESS dispatch adherence | Planned dispatch intervals executed / total planned intervals | Intervals where BESS followed approved dispatch plan | Total planned dispatch intervals | Daily | Energy Systems Lead | ≥ 95% adherence in approved windows | Threshold met while preserving battery SoC and production continuity |

---

## KPI-to-simulation mapping

| Simulation Track | Primary KPIs | Supporting Telemetry |
| --- | --- | --- |
| Throughput | Rolling throughput rate, Copper draw output rate, Rolling yield loss rate | Melt temp, casting speed, rolling speed, gauge, torque, rod diameter, draw speed, wire tension, break count |
| Quality | Dimensional conformance rate, Defect event rate | Gauge, rod diameter, wire tension, break count, quality out-of-spec events |
| Energy | Peak-shaving effectiveness, Grid-import intensity, BESS dispatch adherence | Power import, PV output, BESS SoC, compressed-air pressure |

---

## Lock rule

Any change to these formulas, thresholds, or owners requires change control through the weekly DT governance review before simulation evidence can be accepted.
