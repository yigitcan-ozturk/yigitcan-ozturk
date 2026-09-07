# Yiğitcan Öztürk

**Principal SAP Enterprise & Technology Architect | S/4HANA · RISE · SAP MDG · BTP · Enterprise Integration | Engineering Systems**

I solve complex **enterprise transformation, integration, data-governance and engineering-workflow problems** — from architecture and diagnosis through executable delivery decisions.

**Available for selected contract, fractional and short advisory engagements across the UK / EMEA and internationally.**

[LinkedIn](https://www.linkedin.com/in/yigitcan-ozturk-7920213a3/) · [PAMILANGA](https://www.pamilanga.com) · [Architecture evidence](SAP_ARCHITECTURE_EVIDENCE.md) · **info@pamilanga.com**

## What I can be brought in to solve

- **S/4HANA & RISE architecture** — target-state architecture, readiness, migration/conversion, cutover, rollback and stabilisation
- **SAP MDG & enterprise data** — Business Partner, supplier/vendor, customer and material governance; ownership, quality, migration and reconciliation
- **BTP & integration architecture** — Integration Suite, Cloud Connector, RFC/BAPI, IDoc, OData, REST/SOAP APIs and dependency governance
- **Architecture governance** — AS-IS / TO-BE, roadmaps, operating models, Clean Core, LeanIX, Signavio and transformation decision structures
- **Change-impact & technical diagnostics** — trace a change across systems, interfaces, owners and business processes before delivery risk becomes production risk
- **Engineering procurement intelligence** — turn specifications, supplier evidence and commercial inputs into auditable technical decisions

### Fast engagement formats

- **Architecture diagnostic** — focused review of a transformation, integration or governance problem with an actionable decision map
- **S/4HANA / integration impact sprint** — short engagement to expose dependencies, risks, ownership and delivery actions
- **Technical procurement / compliance review** — structured comparison of specifications, bids, supplier evidence and unresolved deviations

## Evidence

| Signal | Evidence |
| --- | --- |
| **20 years** | Progression from multinational logistics and procurement into ERP-enabled operations, transformation and enterprise architecture |
| **50+ partners** | International manufacturing, technology and specialist delivery ecosystem |
| **30+ requirements** | Industrial / project requirements coordinated end to end |
| **30–40% faster** | RFQ clarification cycles through standardised scope, evidence, ownership and decision points |
| **194 PRs / 160 merged** | Authored pull requests across own and external GitHub projects |
| **7 upstream merges** | Code accepted into OpenTelemetry C++, Apache SeaTunnel, AIBrix / vLLM, Great Expectations and EFF Rayhunter |
| **5 active upstream PRs** | Current external contributions under review across Apache SeaTunnel, Prefect, lakeFS and xAI SDK |

I have worked in **multi-country, audit-controlled and confidentiality-critical environments**. Specific employer, programme, end-client and system details are withheld where required by contractual confidentiality.

## Upstream open-source contributions

### Merged upstream

| Project | Contribution | Status |
| --- | --- | --- |
| [OpenTelemetry C++ #4520](https://github.com/open-telemetry/opentelemetry-cpp/pull/4520) | Added wildcard matching for declarative Metrics SDK view instrument names, preserving implementation boundaries requested in review | **Merged upstream** |
| [Apache SeaTunnel #12174](https://github.com/apache/seatunnel/pull/12174) | Added nonblank validation and focused factory coverage for DataHub sink connection options | **Merged upstream** |
| [Apache SeaTunnel #12148](https://github.com/apache/seatunnel/pull/12148) | Added declarative nonblank validation and focused factory coverage for the Sentry connector | **Merged upstream** |
| [AIBrix / vLLM #2669](https://github.com/vllm-project/aibrix/pull/2669) | Stabilised flaky KVCache pod-triggered reconciliation integration tests | **Merged upstream** |
| [AIBrix / vLLM #2652](https://github.com/vllm-project/aibrix/pull/2652) | RayClusterFleet integration test coverage | **Merged upstream** |
| [Great Expectations #12149](https://github.com/fivetran/great_expectations/pull/12149) | Validator type-checking improvements | **Merged upstream** |
| [EFF Rayhunter #1134](https://github.com/EFForg/rayhunter/pull/1134) | Installer GUI argument help and defaults | **Merged upstream** |

### Active upstream review

| Project | Contribution | Status |
| --- | --- | --- |
| [Apache SeaTunnel #12175](https://github.com/apache/seatunnel/pull/12175) | Validate Typesense source and sink connection options with focused factory coverage | **Active review** |
| [Prefect #23024](https://github.com/PrefectHQ/prefect/pull/23024) | Fix Prefect task retention in shared Dask schedulers | **Active review** |
| [lakeFS #10525](https://github.com/treeverse/lakeFS/pull/10525) | Simplify Spark integration-test setup using shell and lakectl | **Active review** |
| [lakeFS #10530](https://github.com/treeverse/lakeFS/pull/10530) | Remove WebUI login config exhaustive-deps suppression | **Active review** |
| [xAI SDK Python #205](https://github.com/xai-org/xai-sdk-python/pull/205) | Preserve explicit zero polling durations | **Active review** |

## Flagship engineering software

### [impactctl](https://github.com/yigitcan-ozturk/impactctl) — change-impact intelligence

**Know what your change can break — before you merge it.**

A deterministic change-impact CLI that turns Git diffs — and experimentally explicit SAP / enterprise dependency manifests — into explainable system-risk signals.

- API contract, database migration, infrastructure, CI/CD and configuration signals
- `CODEOWNERS`-aware ownership boundaries and review hints
- service maps, OpenAPI / AsyncAPI relationships and downstream dependency paths
- experimental SAP path: changed component → integration → application → business process
- human-readable, JSON and GitHub-flavoured Markdown output

[Repository](https://github.com/yigitcan-ozturk/impactctl) · [Releases](https://github.com/yigitcan-ozturk/impactctl/releases)

### [bidlint](https://github.com/yigitcan-ozturk/bidlint) — engineering procurement intelligence

**Technical bid compliance, with evidence before confidence.**

A deterministic engine for comparing engineering specifications with vendor bids, datasheets and submittals while preserving provenance and explicit uncertainty.

- `PASS / DEVIATION / MISSING / REVIEW` findings
- PDF, XLSX and explicitly scoped IFC evidence
- JSON, CSV, Markdown, HTML and XLSX outputs
- technical knockout, clarification and review workflows
- supplier collaboration and evidence-provenance workflows under active pilot development

[Repository](https://github.com/yigitcan-ozturk/bidlint) · [Releases](https://github.com/yigitcan-ozturk/bidlint/releases)

## Open-source procurement decision stack

| Tool | Purpose |
| --- | --- |
| [supplier-scorecard](https://github.com/yigitcan-ozturk/supplier-scorecard) | Explainable supplier decision infrastructure |
| [rfqdiff](https://github.com/yigitcan-ozturk/rfqdiff) | Structured quotation comparison |
| [currency-normalizer](https://github.com/yigitcan-ozturk/currency-normalizer) | Multi-currency commercial normalization |
| [vendor-risk-engine](https://github.com/yigitcan-ozturk/vendor-risk-engine) | Transparent supplier-risk scoring |
| [payment-terms-parser](https://github.com/yigitcan-ozturk/payment-terms-parser) | Structured supplier payment-term interpretation |

## Current engineering direction

The active engineering path is converging around three connected areas:

- **enterprise change-impact intelligence** — making architecture dependencies and delivery risk explicit before change reaches production;
- **evidence-driven procurement systems** — turning technical, commercial and supplier evidence into auditable decisions;
- **industrial agentic systems** — building deterministic, fail-closed workflows where AI assists analysis without hiding provenance, uncertainty or human decision boundaries.

## Engineering principles

**Evidence before confidence · Deterministic where possible · Explicit uncertainty · Fail safely · Provenance by design**

The common thread across my SAP architecture work and engineering software is simple: make complex enterprise and engineering workflows more **deterministic, auditable and explainable**.

**Relevant conversations:** Principal / Lead SAP Architecture · S/4HANA / RISE · SAP MDG · BTP / integration · enterprise change impact · transformation advisory · technical procurement intelligence · engineering software.
