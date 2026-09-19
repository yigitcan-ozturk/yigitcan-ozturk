# Yiğitcan Öztürk

**Systems & Reliability Engineer | Autonomous Systems · Evidence & Assurance · Telemetry Forensics · Open Source**

I build **evidence and assurance infrastructure for autonomous systems** — making complex technical behaviour deterministic, inspectable, explainable and reproducible.

## Proof at a glance

| Signal | Evidence |
| --- | --- |
| **Flagship** | **[PAMIR](https://github.com/yigitcan-ozturk/pamir)** — offline PX4 telemetry forensics and incident reconstruction |
| **Counter-UAS research** | **[PAMIR-CUAS](https://cuas.pamilanga.com/)** — vendor-neutral, post-test validation and incident reconstruction research prototype |
| **Autonomous defence R&D** | **PAMIR ARGUS** — evidence & assurance infrastructure for autonomous defence systems; v0.1 development lane |
| **Validated baseline** | PAMIR v0.1: **5/5 public incident ULogs**, **3/3 healthy controls**, timestamp validation **PASS**, SHA256-pinned inputs |
| **CUAS public evidence** | Synthetic CUAS-001 stale-evidence and CUAS-002 sensor-disagreement cases are automated-test-backed |
| **Upstream track record** | **13 merged PRs** across Apache SeaTunnel, OpenTelemetry C++, AIBrix/vLLM, Great Expectations, EFF Rayhunter and ROS 2 ecosystem projects · **Apache SeaTunnel: 5 merged upstream PRs** |
| **Public developer tooling** | **[impactctl](https://github.com/yigitcan-ozturk/impactctl)** v0.1.0 · **[bidlint](https://github.com/yigitcan-ozturk/bidlint)** v1.1.0 |
| **Current systems work** | Prefect/Dask, OpenTelemetry gRPC, Grafana Tempo, Apache SeaTunnel Zeta, lakeFS, xAI SDK |

> **PAMIR — Tell me what failed first. And prove it.**  
> **ARGUS — Every autonomous decision should be reconstructable, explainable and reproducible as evidence.**

[LinkedIn](https://www.linkedin.com/in/yigitcan-ozturk-7920213a3/) · [PAMILANGA](https://www.pamilanga.com) · [PAMIR-CUAS](https://cuas.pamilanga.com/) · **info@pamilanga.com**

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

## PAMIR-CUAS — evidence-grade Counter-UAS validation research

**Sensor / C2 evidence → temporal integrity → evidence graph → counterfactual replay → causal finding**

PAMIR-CUAS is a **research prototype** for vendor-neutral, post-test Counter-UAS validation and incident reconstruction. Given normalized sensor/C2 observations and independent ground truth, it reconstructs evidence lineage and tests whether timing faults, stale evidence, sensor disagreement, association or confidence transformation materially contributed to an incorrect outcome.

Current public prototype capabilities include:

- **Causal Evidence Graph** — trace observations, associations, transformations, fusion decisions and replay results through an inspectable evidence chain.
- **Temporal Integrity analysis** — identify stale, out-of-order and clock-offset evidence conditions.
- **Sensor disagreement analysis** — surface materially disagreeing observations for reconstruction.
- **Counterfactual Replay** — safely exclude or correct evidence offline and test whether the reconstructed outcome changes.
- **Causal attribution reporting** — distinguish evidence that materially changes an outcome from evidence that is merely correlated with it.

| Public synthetic case | Test-backed result |
| --- | --- |
| **CUAS-001** | Stale RF evidence reproduced a false-positive path; excluding the stale evidence changed the reconstructed outcome |
| **CUAS-002** | Sensor disagreement reproduced a false-positive path; excluding the disagreeing observation changed the reconstructed outcome |

These are **synthetic, automated-test-backed research results**. They are not claims of field validation, operational deployment, SSB approval or HARDKILL integration.

PAMIR-CUAS is validation infrastructure. It does **not** perform target selection, weapon control, engagement decisions, interceptor guidance, firing solutions or effector optimization.

**Technical portal:** [cuas.pamilanga.com](https://cuas.pamilanga.com/)  
**Technical / integration enquiries:** **cuas@pamilanga.com**

---

## PAMIR ARGUS — evidence & assurance infrastructure for autonomous defence systems

**Observation → provenance → fusion → decision → first divergence → causal evidence → reproducible replay**

PAMIR ARGUS is a separate R&D lane extending the PAMIR evidence philosophy toward assurance of autonomous defence-system decision chains.

Its core objective is simple:

> **Every autonomous decision should be reconstructable, explainable and reproducible as evidence.**

ARGUS v0.1 focuses on an inspectable synthetic **Radar + EO + RF → Tracker → Fusion → Decision** chain and the evidence required to reconstruct how a system reached a decision, where the first meaningful divergence occurred, what evidence supports the reconstruction, and what remains uncertain.

The project is currently under development. It is **not presented as field-validated, operationally deployed, certified, or integrated into any defence platform**.

ARGUS is an evidence and assurance layer. It does **not** perform weapon control, target engagement, interceptor guidance or firing-solution generation.

---

## Selected upstream contributions

| Project | Contribution |
| --- | --- |
| [Apache SeaTunnel #12274](https://github.com/apache/seatunnel/pull/12274) | S3 Redshift declarative validation for required JDBC options with focused regression coverage |
| [Apache SeaTunnel #12272](https://github.com/apache/seatunnel/pull/12272) | BigQuery declarative validation with nonblank identifiers, write-mode validation and regression coverage |
| [Apache SeaTunnel #12175](https://github.com/apache/seatunnel/pull/12175) | Typesense source/sink connection validation with regression coverage |
| [Apache SeaTunnel #12174](https://github.com/apache/seatunnel/pull/12174) | Nonblank validation for DataHub sink connection options |
| [Apache SeaTunnel #12148](https://github.com/apache/seatunnel/pull/12148) | Declarative nonblank validation for the Sentry connector |
| [OpenTelemetry C++ #4520](https://github.com/open-telemetry/opentelemetry-cpp/pull/4520) | Wildcard matching for Metrics SDK view instrument names |
| [AIBrix / vLLM #2669](https://github.com/vllm-project/aibrix/pull/2669) | Stabilised KVCache pod-triggered reconciliation integration tests |
| [AIBrix / vLLM #2652](https://github.com/vllm-project/aibrix/pull/2652) | Added RayClusterFleet integration test coverage |
| [Great Expectations #12184](https://github.com/fivetran/great_expectations/pull/12184) | Brought metric repository tests fully under mypy with focused typing cleanup |
| [Great Expectations #12149](https://github.com/fivetran/great_expectations/pull/12149) | Validator type-checking improvements |
| [EFF Rayhunter #1146](https://github.com/EFForg/rayhunter/pull/1146) | Reject oversized Wingtech admin passwords safely with regression coverage |
| [EFF Rayhunter #1134](https://github.com/EFForg/rayhunter/pull/1134) | Exposed CLI help and default values in the installer GUI |
| [ros2_lingua #20](https://github.com/purahan/ros2_lingua/pull/20) | Completed regression coverage for all `lingua::Tags` constants and kept C++ bindings aligned with Python schema tags |

## Current systems work

| Project | Problem |
| --- | --- |
| [Prefect #23024](https://github.com/PrefectHQ/prefect/pull/23024) | Reduce Prefect task retention in shared Dask schedulers |
| [OpenTelemetry C++ #4561](https://github.com/open-telemetry/opentelemetry-cpp/pull/4561) | Document nlohmann-json dependency maintenance |
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
- Counter-UAS validation and post-test incident reconstruction
- Evidence & assurance infrastructure for autonomous-system decision chains
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

I am open to selected collaborations involving **autonomous-system reliability, evidence & assurance, Counter-UAS validation, telemetry forensics, distributed systems, AI/data infrastructure, developer tooling and engineering automation**.

For general technical partnerships, external validation or collaboration: **info@pamilanga.com**  
For PAMIR-CUAS technical evaluation and integration dialogue: **cuas@pamilanga.com**
