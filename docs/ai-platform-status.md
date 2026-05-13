# Metallurgical — AI Platform Deployment Status

> **Gate 3 Artifact (AI Platform Readiness)**
> **Factory:** Coo-Cah Metallurgical & Minerals Factory | **Location:** Warri / Ovwian-Aladja Steel Corridor, Delta State
> **Document Version:** 1.0 | **Owner:** AI Platform / Digital Manufacturing Team
> **Status:** Mock/Stub Endpoints Active — Production endpoints pending hot commissioning

---

## 1. Deployment Overview

The Coo-Cah AI Platform hosts the inference and optimization services consumed by the Metallurgical factory MES and digital twin stack. At this stage, contract-valid stubs are active to support integration tests without live production data.

| Parameter | Value |
| --- | --- |
| Platform Host | `ai-platform.coo-cah.internal` (Warri edge) with Lagos DR fallback |
| API Base URL (stub) | `https://ai-stub.coo-cah.internal/api/v1` |
| Authentication | OAuth 2.0 service accounts (factory-scoped) |
| Transport Security | TLS 1.3 in transit; internal CA |
| Stub Deployment Window | 2026-Q1 pre-commissioning |
| Production Go-Live Target | Hot commissioning and controlled ramp-up |

---

## 2. Endpoint Status Register

| Endpoint | Method | Description | Stub Status | Prod Status |
| --- | --- | --- | --- | --- |
| `/api/v1/ai/rolling-yield-optimizer` | POST | Rolling pass and yield optimization recommendation | ✅ Active | ⏳ Pending |
| `/api/v1/ai/extrusion-die-health` | POST | Aluminium die wear and replacement forecast | ✅ Active | ⏳ Pending |
| `/api/v1/ai/copper-breakage-risk` | POST | Copper wire breakage probability and alerting | ✅ Active | ⏳ Pending |
| `/api/v1/ai/coating-thickness-control` | POST | Galvanising thickness control recommendations | ✅ Active | ⏳ Pending |
| `/api/v1/mes/oee/realtime` | GET | OEE rollup by process line and shift | ✅ Active | ⏳ Pending |
| `/api/v1/ai/predictive-maintenance` | POST | Bearing, motor, and gearbox anomaly scoring | ✅ Active | ⏳ Pending |
| `/api/v1/dt/machine-state` | GET | Digital twin state synchronization feed | ✅ Active | ⏳ Pending |
| `/api/v1/dt/simulation/run` | POST | Trigger throughput/energy simulation runs | ✅ Active | ⏳ Pending |
| `/api/v1/ai/energy-dispatch` | POST | BESS and peak-shaving dispatch recommendation | ✅ Active | ⏳ Pending |

---

## 3. Stub Behaviour Contract

All stubs conform to MES integration contracts in [`mes-integration.md`](./mes-integration.md).

- Responses are schema-valid JSON payloads matching production contracts.
- Deterministic outputs are used for repeatable integration tests.
- All responses include `"stub": true` flags.
- Status codes: `200` (valid), `422` (schema invalid), `503` (forced degradation mode).

---

## 4. Service Account Register (Non-Production)

| Service Account | Scope | Managed By |
| --- | --- | --- |
| `svc-met-mes-ai-stub` | Rolling, extrusion, copper, OEE, energy | AI Platform / IT Ops |
| `svc-met-dt-stub` | Digital twin state and simulation endpoints | Digital Manufacturing |
| `svc-met-maint-stub` | Predictive maintenance and asset alerts | Reliability Engineering |

Credential rotation schedule: 90 days in stub environments; 30 days in production.

---

## 5. Integration Test Coverage

| Test Suite | Coverage | Last Run | Result |
| --- | --- | --- | --- |
| MES → Rolling optimizer API | Contract and error handling tests | 2026-Q1 | ✅ Pass |
| MES → Extrusion die health API | Die health payload and threshold behavior | 2026-Q1 | ✅ Pass |
| MES → Copper breakage API | Draw-line events and alert threshold validation | 2026-Q1 | ✅ Pass |
| MES → OEE real-time API | Multi-line aggregation and shift filtering | 2026-Q1 | ✅ Pass |
| DT sync API | MQTT-to-REST bridge and timestamp alignment | 2026-Q1 | ✅ Pass |
| Full E2E (MES → AI → DT) | Event-to-simulation trigger chain | 2026-Q1 | ✅ Pass |

---

## 6. Open Items Before Production Go-Live

| Item | Owner | Target Date | Status |
| --- | --- | --- | --- |
| Production GPU node hardening and failover | AI Platform Team | 2026-Q2 | ⏳ Pending |
| Production TLS certificate issuance | IT Ops | 2026-Q2 | ⏳ Pending |
| API load test (sustained 800 req/min) | AI Platform / QA | 2026-Q2 | ⏳ Pending |
| Security validation of API surface | IT Security | See [`pentest-scoping.md`](./pentest-scoping.md) | ⏳ Pending |
| Controlled activation runbook approval | Digital Manufacturing | 2026-Q2 | ⏳ Pending |

---

## Related Documents

| Document | Purpose |
| --- | --- |
| [`mes-integration.md`](./mes-integration.md) | AI and integration contract baseline |
| [`pentest-scoping.md`](./pentest-scoping.md) | Security scope for AI and MES-facing interfaces |
| [`digital-twin.md`](./digital-twin.md) | Digital twin topology and simulation objectives |
| [`gap-closure-report.md`](./gap-closure-report.md) | Gap closure status and evidence mapping |
