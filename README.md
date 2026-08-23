# Yiğitcan Öztürk

**Engineering Software Builder — CAD Intelligence, Specification Automation, Procurement Systems & Explainable Decision Infrastructure.**

I build engineering software that turns drawings, specifications, supplier evidence and project requirements into decisions and technical outputs that can be reviewed, traced and reproduced.

My work currently spans three connected areas:

- **CAD & AEC Intelligence** — spatial reasoning, CAD automation, technical drawing workflows and architecture/construction tooling.
- **Specification Intelligence** — evidence-grounded compliance, document understanding and engineering review systems.
- **Procurement Intelligence** — quotation comparison, supplier evaluation, commercial normalization and explainable sourcing decisions.

## Current focus

### AXF — Architectural eXecution Framework
A CAD/BIM-native architectural intelligence platform under active development.

AXF is being designed to ingest existing project geometry and project requirements, reconstruct a semantic building model, generate and validate spatial layouts, and ultimately produce coordinated architectural documentation including plans, reflected ceiling plans, sections, elevations, details, schedules and DWG outputs.

The architecture is intentionally client-neutral: domain rules and client standards are isolated from the core engine so the same platform can support architecture, interiors, retail, exhibitions, offices, hospitality and construction workflows.

### PamiCAD
A technical CAD development line focused on engineering drawing, manufacturing-oriented workflows and structured CAD automation.

### SPEC AI
A specification-intelligence system focused on extracting, structuring and validating engineering requirements while preserving provenance and explicit uncertainty.

These projects are currently developed privately while their technical foundations, validation gates and production workflows mature.

## Open-source engineering tools

### [bidlint](https://github.com/yigitcan-ozturk/bidlint)
**Technical bid compliance, with evidence before confidence.**

A deterministic engine for comparing engineering specifications with vendor bids, datasheets and submittals. It preserves source provenance and produces explicit `PASS / DEVIATION / MISSING / REVIEW` findings across document packages.

### [supplier-scorecard](https://github.com/yigitcan-ozturk/supplier-scorecard)
**Explainable supplier decision infrastructure.**

Combines quotation competitiveness, payment exposure, vendor risk and technical-compliance signals into transparent, policy-aware supplier recommendations.

### [rfqdiff](https://github.com/yigitcan-ozturk/rfqdiff)
**Structured quotation comparison for procurement workflows.**

A lightweight tool for comparing supplier quotations and producing machine-readable commercial decision signals.

### [vendor-risk-engine](https://github.com/yigitcan-ozturk/vendor-risk-engine)
**Transparent supplier-risk scoring.**

Models delivery, quality, commercial, compliance and dependency risk without hiding the decision logic behind a black box.

### Supporting tools

- [currency-normalizer](https://github.com/yigitcan-ozturk/currency-normalizer) — commercial normalization for multi-currency comparisons.
- [payment-terms-parser](https://github.com/yigitcan-ozturk/payment-terms-parser) — structured interpretation of supplier payment terms.

## Engineering software stack

```text
                    ┌─────────────────────────────┐
                    │       CAD / AEC Layer       │
                    │    AXF • PamiCAD • DWG      │
                    └──────────────┬──────────────┘
                                   │
                    ┌──────────────▼──────────────┐
                    │ Specification Intelligence  │
                    │      SPEC AI • bidlint      │
                    └──────────────┬──────────────┘
                                   │
currency-normalizer ──> rfqdiff ──┼──────────────────┐
payment-terms-parser ──────────────┼──────────────────┤
vendor-risk-engine ────────────────┼──> supplier-scorecard
bidlint ──> technical compliance ──┘                  │
                                                      ▼
                                        Explainable Engineering Decisions
```

The goal is not to automate professional judgment away. The goal is to make engineering workflows more **deterministic, auditable, interoperable and explainable**.

## Principles

- **Evidence before confidence** — outputs should point back to source evidence.
- **Deterministic where possible** — measurable engineering rules belong in code, not model opinion.
- **Explicit uncertainty** — ambiguity becomes `REVIEW_REQUIRED`, not fabricated certainty.
- **Fail safely** — a system should be able to say that a valid solution cannot be produced.
- **Provenance by design** — geometry, requirements and decisions should remain traceable to their sources.
- **Composable architecture** — stable interfaces and isolated domain/client rules scale better than opaque monoliths.
- **Engineering first** — software must respect the technical and construction context in which it operates.

## Direction

I am building a broader engineering-software portfolio spanning **architectural intelligence, CAD automation, specification systems, technical compliance and procurement decision infrastructure**, with selected work evolving under **PAMILANGA Labs**.

The long-term direction is a connected engineering toolchain where drawings, specifications, technical requirements, supplier data and project constraints can move through one traceable decision pipeline — from design and review to sourcing and execution.

[GitHub projects](https://github.com/yigitcan-ozturk?tab=repositories) · [PAMILANGA](https://www.pamilanga.com)
