# Yiğitcan Öztürk

**Systems & Reliability Engineer | Autonomous Systems · Telemetry Forensics · Distributed Systems · Open Source**

I build systems that make complex technical failures **deterministic, inspectable and explainable**.

## Proof at a glance

| Signal | Evidence |
| --- | --- |
| **Flagship** | **[PAMIR](https://github.com/yigitcan-ozturk/pamir)** — offline PX4 telemetry forensics and incident reconstruction |
| **Validated baseline** | PAMIR v0.1: **5/5 public incident ULogs**, **3/3 healthy controls**, timestamp validation **PASS**, SHA256-pinned inputs |
| **Upstream track record** | **9 merged PRs** across Apache SeaTunnel, OpenTelemetry C++, AIBrix/vLLM, Great Expectations and EFF Rayhunter |
| **Public developer tooling** | **[impactctl](https://github.com/yigitcan-ozturk/impactctl)** v0.1.0 · **[bidlint](https://github.com/yigitcan-ozturk/bidlint)** v1.1.0 |
| **Current systems work** | Prefect/Dask, OpenTelemetry gRPC, Grafana Tempo, Apache SeaTunnel Zeta, lakeFS, xAI SDK |

> **PAMIR — Tell me what failed first. And prove it.**

[LinkedIn](https://www.linkedin.com/in/yigitcan-ozturk-7920213a3/) · [PAMILANGA](https://www.pamilanga.com) · **info@pamilanga.com**

---

## PAMIR — autonomous incident reconstruction

**PX4 ULog → material root event → causal sequence → timestamped evidence**

PAMIR is an offline forensic analysis engine for autonomous-system telemetry. It reconstructs an incident timeline, identifies the **earliest material root event**, and preserves evidence showing what happened next.

| Validation signal | v0.1 result |
| --- | --- |
| Public PX4 incident logs | **5 / 5** identified with a material root event |
| Healthy / control logs | **3 / 3** remained free of material root detections |
| Causal ordering | Timestamp-based validation **PASS** |
| Reproducibility | SHA256-pinned public benchmark inputs |
| Operation | Local / offline analysis |

**Release:** [PAMIR v0.1.0](https://github.com/yigitcan-ozturk/pamir/releases/tag/v0.1.0)  
**Repository:** [github.com/yigitcan-ozturk/pamir](https://github.com/yigitcan-ozturk/pamir)

Current direction: external validation against additional public PX4 ULogs and real-world telemetry, methodology review, and evidence-backed incident cases.

---

## Selected upstream contributions

| Project | Contribution |
| --- | --- |
| [Apache SeaTunnel #12272](https://github.com/apache/seatunnel/pull/12272) | BigQuery declarative validation with nonblank identifiers, write-mode validation and regression coverage |
| [Apache SeaTunnel #12175](https://github.com/apache/seatunnel/pull/12175) | Typesense source/sink connection validation with regression coverage |
| [Apache SeaTunnel #12174](https://github.com/apache/seatunnel/pull/12174) | Nonblank validation for DataHub sink connection options |
| [Apache SeaTunnel #12148](https://github.com/apache/seatunnel/pull/12148) | Declarative nonblank validation for the Sentry connector |
| [OpenTelemetry C++ #4520](https://github.com/open-telemetry/opentelemetry-cpp/pull/4520) | Wildcard matching for Metrics SDK view instrument names |
| [AIBrix / vLLM #2669](https://github.com/vllm-project/aibrix/pull/2669) | Stabilised KVCache pod-triggered reconciliation integration tests |
| [AIBrix / vLLM #2652](https://github.com/vllm-project/aibrix/pull/2652) | Added RayClusterFleet integration test coverage |
| [Great Expectations #12149](https://github.com/fivetran/great_expectations/pull/12149) | Validator type-checking improvements |
| [EFF Rayhunter #1134](https://github.com/EFForg/rayhunter/pull/1134) | Exposed CLI help and default values in the installer GUI |

## Current systems work

| Project | Problem |
| --- | --- |
| [Prefect #23024](https://github.com/PrefectHQ/prefect/pull/23024) | Reduce Prefect task retention in shared Dask schedulers |
| [OpenTelemetry C++ #4541](https://github.com/open-telemetry/opentelemetry-cpp/pull/4541) | Make OTLP gRPC functional teardown deterministic |
| [Grafana Tempo #7866](https://github.com/grafana/tempo/pull/7866) | Restore metadata intrinsic filtering in autocomplete |
| [Apache SeaTunnel Zeta #12118](https://github.com/apache/seatunnel/issues/12118) | Bound terminal-state notification delivery without dropping terminal events |
| [lakeFS #10525](https://github.com/treeverse/lakeFS/pull/10525) | Simplify Spark integration-test setup using shell and `lakectl` |
| [xAI SDK Python #205](https://github.com/xai-org/xai-sdk-python/pull/205) | Preserve explicit zero polling durations |

---

## Flagship tools

### [impactctl](https://github.com/yigitcan-ozturk/impactctl) — change-impact intelligence

**Know what your change can break before you merge it.**

A deterministic CLI that turns Git diffs and explicit dependency manifests into explainable system-risk signals.

- API contracts, database migrations, infrastructure, CI/CD and configuration signals
- `CODEOWNERS`-aware ownership boundaries and review hints
- service maps, OpenAPI / AsyncAPI relationships and downstream dependency paths
- human-readable, JSON and GitHub-flavoured Markdown output
- public cross-platform release with checksums

[Repository](https://github.com/yigitcan-ozturk/impactctl) · [Releases](https://github.com/yigitcan-ozturk/impactctl/releases)

### [bidlint](https://github.com/yigitcan-ozturk/bidlint) — engineering procurement intelligence

**Technical bid compliance, with evidence before confidence.**

A deterministic engine for comparing engineering specifications with vendor bids, datasheets and submittals while preserving provenance and explicit uncertainty.

- `PASS / DEVIATION / MISSING / REVIEW` findings
- PDF, XLSX and explicitly scoped IFC evidence
- JSON, CSV, Markdown, HTML and XLSX outputs
- production-adoption release gate and approved sanitized pilot
- stable v1.1.0 release

[Repository](https://github.com/yigitcan-ozturk/bidlint) · [Releases](https://github.com/yigitcan-ozturk/bidlint/releases)

## Engineering decision stack

| Tool | Purpose |
| --- | --- |
| [supplier-scorecard](https://github.com/yigitcan-ozturk/supplier-scorecard) | Explainable supplier decision infrastructure |
| [rfqdiff](https://github.com/yigitcan-ozturk/rfqdiff) | Structured quotation comparison |
| [currency-normalizer](https://github.com/yigitcan-ozturk/currency-normalizer) | Multi-currency commercial normalization |
| [vendor-risk-engine](https://github.com/yigitcan-ozturk/vendor-risk-engine) | Transparent supplier-risk scoring |
| [payment-terms-parser](https://github.com/yigitcan-ozturk/payment-terms-parser) | Structured supplier payment-term interpretation |

---

## Engineering focus

- Autonomous-system telemetry and incident forensics
- Distributed systems reliability and runtime failure modes
- Observability, telemetry and production diagnostics
- AI / data infrastructure and orchestration
- Developer tooling and change-impact analysis
- Engineering procurement and auditable technical decision systems
- Enterprise integration and architecture

## Engineering principles

**Evidence before confidence · Deterministic where possible · Explicit uncertainty · Fail safely · Provenance by design**

I prefer systems that make reasoning visible, preserve evidence, degrade safely under uncertainty and can be tested against real operating conditions.

## Background

Long-running work across **SAP architecture, enterprise transformation, integration, data governance, industrial operations and technical procurement** informs the systems I build today.

Relevant areas include S/4HANA & RISE, SAP MDG, BTP & Integration Suite, RFC/BAPI, IDoc, OData, REST/SOAP APIs, Clean Core, LeanIX, Signavio and architecture governance.

## Work with me

I am open to selected collaborations involving **autonomous-system reliability, telemetry forensics, distributed systems, AI/data infrastructure, developer tooling and engineering automation**.

For technical partnerships, external validation or collaboration: **info@pamilanga.com**
