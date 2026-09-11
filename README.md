# Yiğitcan Öztürk

**Principal Systems & Enterprise Architect | Distributed Systems · Reliability · AI Infrastructure · Open Source**

I solve complex systems problems where **runtime behavior, integration, reliability, data flow and engineering decisions** need to become deterministic, testable and explainable.

My current open-source work spans **Apache SeaTunnel, OpenTelemetry, Prefect/Dask, Grafana Tempo, AIBrix/vLLM, lakeFS, Great Expectations, Gazebo, EFF Rayhunter and the xAI Python SDK**.

**Available for selected contract, fractional and advisory engagements across the UK / EMEA and internationally.**

[LinkedIn](https://www.linkedin.com/in/yigitcan-ozturk-7920213a3/) · [PAMILANGA](https://www.pamilanga.com) · **info@pamilanga.com**

## What I work on

- Distributed systems reliability and runtime failure modes
- Observability, telemetry and production diagnostics
- AI / data infrastructure and orchestration
- Developer tooling and change-impact analysis
- Enterprise integration and architecture
- Engineering procurement and auditable technical decision systems

## Open-source track record

| Signal | Evidence |
| --- | --- |
| **8 merged upstream PRs** | Accepted contributions across Apache SeaTunnel, OpenTelemetry C++, AIBrix/vLLM, Great Expectations and EFF Rayhunter |
| **3 Apache SeaTunnel merges** | Sentry, DataHub and Typesense connector validation improvements accepted into `dev` |
| **Active systems work** | Prefect/Dask scheduler retention, OpenTelemetry gRPC teardown, Grafana Tempo filtering and SeaTunnel Zeta delivery semantics |
| **Own tooling** | `impactctl`, `bidlint` and a deterministic procurement / engineering decision stack |

## Selected upstream contributions

| Project | Contribution |
| --- | --- |
| [Apache SeaTunnel #12175](https://github.com/apache/seatunnel/pull/12175) | Typesense source/sink connection validation with focused regression coverage |
| [Apache SeaTunnel #12174](https://github.com/apache/seatunnel/pull/12174) | Nonblank validation for DataHub sink connection options |
| [Apache SeaTunnel #12148](https://github.com/apache/seatunnel/pull/12148) | Declarative nonblank validation for the Sentry connector |
| [OpenTelemetry C++ #4520](https://github.com/open-telemetry/opentelemetry-cpp/pull/4520) | Wildcard matching for declarative Metrics SDK view instrument names |
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

## Flagship tools

### [impactctl](https://github.com/yigitcan-ozturk/impactctl) — change-impact intelligence

**Know what your change can break before you merge it.**

A deterministic CLI that turns Git diffs and explicit dependency manifests into explainable system-risk signals.

- API contracts, database migrations, infrastructure, CI/CD and configuration signals
- `CODEOWNERS`-aware ownership boundaries and review hints
- service maps, OpenAPI / AsyncAPI relationships and downstream dependency paths
- experimental enterprise / SAP dependency path
- human-readable, JSON and GitHub-flavoured Markdown output

[Repository](https://github.com/yigitcan-ozturk/impactctl) · [Releases](https://github.com/yigitcan-ozturk/impactctl/releases)

### [bidlint](https://github.com/yigitcan-ozturk/bidlint) — engineering procurement intelligence

**Technical bid compliance, with evidence before confidence.**

A deterministic engine for comparing engineering specifications with vendor bids, datasheets and submittals while preserving provenance and explicit uncertainty.

- `PASS / DEVIATION / MISSING / REVIEW` findings
- PDF, XLSX and explicitly scoped IFC evidence
- JSON, CSV, Markdown, HTML and XLSX outputs
- technical knockout, clarification and review workflows
- evidence provenance and supplier collaboration workflows

[Repository](https://github.com/yigitcan-ozturk/bidlint) · [Releases](https://github.com/yigitcan-ozturk/bidlint/releases)

## Engineering decision stack

| Tool | Purpose |
| --- | --- |
| [supplier-scorecard](https://github.com/yigitcan-ozturk/supplier-scorecard) | Explainable supplier decision infrastructure |
| [rfqdiff](https://github.com/yigitcan-ozturk/rfqdiff) | Structured quotation comparison |
| [currency-normalizer](https://github.com/yigitcan-ozturk/currency-normalizer) | Multi-currency commercial normalization |
| [vendor-risk-engine](https://github.com/yigitcan-ozturk/vendor-risk-engine) | Transparent supplier-risk scoring |
| [payment-terms-parser](https://github.com/yigitcan-ozturk/payment-terms-parser) | Structured supplier payment-term interpretation |

## Enterprise background

I also bring long-running experience across **SAP architecture, enterprise transformation, integration, data governance, industrial operations and technical procurement**.

Relevant areas include S/4HANA & RISE, SAP MDG, BTP & Integration Suite, RFC/BAPI, IDoc, OData, REST/SOAP APIs, Clean Core, LeanIX, Signavio and architecture governance.

That background informs the systems I build: software that makes complex technical and enterprise workflows more **deterministic, inspectable and explainable**.

## Engineering principles

**Evidence before confidence · Deterministic where possible · Explicit uncertainty · Fail safely · Provenance by design**

I prefer systems that make reasoning visible, preserve evidence, degrade safely under uncertainty and can be tested against real operating conditions.

## Work with me

I am open to selected engagements involving **distributed systems, reliability, AI/data infrastructure, developer tooling, enterprise integration and engineering automation**.

For collaboration, consulting or technical partnerships: **info@pamilanga.com**
