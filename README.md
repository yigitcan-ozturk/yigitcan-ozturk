# Yiğitcan Öztürk

**Open-source systems engineer · Tool builder · Enterprise architecture practitioner**

I build and contribute to software around **developer tooling, distributed systems, reliability, change-impact analysis, engineering intelligence and evidence-driven workflows**.

My current open-source work spans **Apache SeaTunnel, OpenTelemetry, Prefect/Dask, AIBrix/vLLM, lakeFS, Great Expectations, EFF Rayhunter and the xAI Python SDK**.

[LinkedIn](https://www.linkedin.com/in/yigitcan-ozturk-7920213a3/) · [PAMILANGA](https://www.pamilanga.com) · [Architecture evidence](SAP_ARCHITECTURE_EVIDENCE.md) · **info@pamilanga.com**

## Open-source track record

| Signal | Evidence |
| --- | --- |
| **8 merged upstream PRs** | Accepted contributions across Apache SeaTunnel, OpenTelemetry C++, AIBrix/vLLM, Great Expectations and EFF Rayhunter |
| **3 Apache SeaTunnel merges** | Sentry, DataHub and Typesense connector validation improvements accepted into `dev` |
| **4 active upstream PRs** | Prefect, lakeFS and xAI SDK contributions currently under review |
| **Runtime/reliability track** | Active work around Prefect/Dask scheduler retention and SeaTunnel Zeta terminal-state delivery |
| **Own tooling** | `impactctl`, `bidlint` and a growing deterministic procurement/engineering decision stack |

## Merged upstream contributions

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

## Active upstream work

| Project | Contribution | State |
| --- | --- | --- |
| [Prefect #23024](https://github.com/PrefectHQ/prefect/pull/23024) | Fix Prefect task retention in shared Dask schedulers | **Active review / runtime regression work** |
| [lakeFS #10525](https://github.com/treeverse/lakeFS/pull/10525) | Simplify Spark integration-test setup using shell and `lakectl` | **Active review** |
| [lakeFS #10530](https://github.com/treeverse/lakeFS/pull/10530) | Remove WebUI login-config exhaustive-deps suppression | **Active review** |
| [xAI SDK Python #205](https://github.com/xai-org/xai-sdk-python/pull/205) | Preserve explicit zero polling durations | **Active review** |

### Current distributed-systems track

I am also working through [Apache SeaTunnel Zeta #12118](https://github.com/apache/seatunnel/issues/12118), focused on bounding terminal-state notification delivery without dropping terminal events. The design space includes worker/master delivery semantics, bounded dispatch, retry/backoff, idempotency and failover-safe convergence.

## Flagship tools

### [impactctl](https://github.com/yigitcan-ozturk/impactctl) — change-impact intelligence

**Know what your change can break — before you merge it.**

A deterministic CLI that turns Git diffs and explicit dependency manifests into explainable system-risk signals.

- API contracts, database migrations, infrastructure, CI/CD and configuration signals
- `CODEOWNERS`-aware ownership boundaries and review hints
- service maps, OpenAPI / AsyncAPI relationships and downstream dependency paths
- experimental enterprise/SAP dependency path
- human-readable, JSON and GitHub-flavoured Markdown output

[Repository](https://github.com/yigitcan-ozturk/impactctl) · [Releases](https://github.com/yigitcan-ozturk/impactctl/releases)

### [bidlint](https://github.com/yigitcan-ozturk/bidlint) — engineering procurement intelligence

**Technical bid compliance, with evidence before confidence.**

A deterministic engine for comparing engineering specifications with vendor bids, datasheets and submittals while preserving provenance and explicit uncertainty.

- `PASS / DEVIATION / MISSING / REVIEW` findings
- PDF, XLSX and explicitly scoped IFC evidence
- JSON, CSV, Markdown, HTML and XLSX outputs
- technical knockout, clarification and review workflows
- evidence-provenance and supplier collaboration workflows

[Repository](https://github.com/yigitcan-ozturk/bidlint) · [Releases](https://github.com/yigitcan-ozturk/bidlint/releases)

## Engineering decision stack

| Tool | Purpose |
| --- | --- |
| [supplier-scorecard](https://github.com/yigitcan-ozturk/supplier-scorecard) | Explainable supplier decision infrastructure |
| [rfqdiff](https://github.com/yigitcan-ozturk/rfqdiff) | Structured quotation comparison |
| [currency-normalizer](https://github.com/yigitcan-ozturk/currency-normalizer) | Multi-currency commercial normalization |
| [vendor-risk-engine](https://github.com/yigitcan-ozturk/vendor-risk-engine) | Transparent supplier-risk scoring |
| [payment-terms-parser](https://github.com/yigitcan-ozturk/payment-terms-parser) | Structured supplier payment-term interpretation |

## Systems and enterprise background

Alongside software engineering, I bring long-running experience across **enterprise transformation, SAP architecture, integration, data governance, industrial operations and technical procurement**.

Areas include:

- **S/4HANA & RISE architecture** — target state, readiness, migration/conversion, cutover and stabilisation
- **SAP MDG & enterprise data** — Business Partner, supplier/vendor, customer and material governance
- **BTP & integration architecture** — Integration Suite, Cloud Connector, RFC/BAPI, IDoc, OData, REST/SOAP APIs
- **Architecture governance** — AS-IS / TO-BE, roadmaps, Clean Core, LeanIX, Signavio and transformation decision structures
- **Engineering procurement intelligence** — specifications, supplier evidence, commercial inputs and auditable technical decisions

This background informs the systems I build: software that makes complex engineering and enterprise workflows more **deterministic, inspectable and explainable**.

## Engineering principles

**Evidence before confidence · Deterministic where possible · Explicit uncertainty · Fail safely · Provenance by design**

I prefer tools and systems that make reasoning visible, preserve evidence, degrade safely under uncertainty and can be tested against real operating conditions.
