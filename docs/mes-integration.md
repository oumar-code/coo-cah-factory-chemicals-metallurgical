# MES Integration

> **Factory:** Coo-Cah Metallurgical & Minerals Factory
> **Factory ID:** `CCH-MET`
> **Integration Scope:** Metallurgical process lines, utilities, environment, and digital twin feed

---

## 1. Integration Architecture

```mermaid
flowchart TD
    subgraph OT[Factory OT Network]
      EAF[Z2 EAF PLC]
      LF[Z3 Ladle Furnace PLC]
      CC[Z4 Continuous Casting PLCs]
      ROLL[Z5 Steel Rolling DCS]
      AL[Z6 Aluminium Line PLCs]
      CU[Z7 Copper Line PLCs]
      LEAD[Z8 Lead Alloy PLC]
      MIN[Z9 Mineral Processing PLC]
      UTIL[Z10 Utilities EMS]
      ENV[Z11 ETP + CEMS]
      LAB[Z12 QC LIMS]
    end

    subgraph EDGE[Edge Integration Layer]
      OPC[OPC-UA Collectors]
      MQTT[MQTT Broker]
      MOD[Modbus TCP Gateways]
    end

    subgraph MES[MES + Historian]
      MESCORE[MES Core]
      HIST[Time-Series Historian]
      QMS[Quality and Genealogy]
    end

    subgraph DT[Digital Twin & Simulation]
      DTSTATE[DT State Store]
      SIM[Simulation Orchestrator]
    end

    EAF --> OPC
    LF --> OPC
    CC --> OPC
    ROLL --> OPC
    AL --> OPC
    CU --> OPC
    LEAD --> OPC
    MIN --> OPC
    UTIL --> MQTT
    ENV --> MOD
    LAB --> MESCORE

    OPC --> MESCORE
    MQTT --> MESCORE
    MOD --> MESCORE
    MESCORE --> HIST
    MESCORE --> QMS
    MESCORE --> DTSTATE
    HIST --> SIM
    QMS --> SIM
```

---

## 2. Canonical Data Contract Rules

| Rule | Requirement |
| --- | --- |
| Asset key | Must use `DT-MET-*` IDs from `digital-twin.md` |
| Zone key | Must use `Z1`-`Z14` IDs from `floor-plan.md` |
| Timestamp | UTC ISO 8601 with millisecond precision |
| Units | SI units only; unit field mandatory |
| Quality flag | Every point must include quality (`good`, `bad`, `uncertain`) |

---

## 3. Minimum Telemetry for Simulation Readiness

| Process Domain | Minimum Signals | Simulation Use |
| --- | --- | --- |
| Steel (Z2-Z5) | Melt temp, casting speed, rolling speed, gauge, torque, downtime | Throughput, yield, bottleneck analysis |
| Aluminium (Z6) | Billet temp, ram pressure, profile speed, gauge | Capacity and quality drift scenarios |
| Copper (Z7) | Rod diameter, draw speed, wire tension, break count | Breakage risk and output optimization |
| Environmental (Z11) | ETP pH/flow, NOx/SO2/PM trends | Compliance and constraint modeling |
| Utilities (Z10) | Power import, PV output, BESS SoC, compressed air pressure | Energy cost and dispatch simulation |

---

## 4. Event Triggers to Digital Twin

- Work-order start/stop
- Equipment state change (run, idle, fault)
- Quality out-of-spec event
- Energy threshold breach
- Environmental threshold breach

These trigger simulation jobs for what-if and corrective-action scenarios.
