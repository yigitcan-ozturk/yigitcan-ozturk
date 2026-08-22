# Yiğitcan Öztürk

**Engineering software builder focused on technical compliance, procurement intelligence and explainable decision systems.**

I build deterministic tools that turn specifications, supplier evidence and engineering documents into decisions that can be reviewed, traced and reproduced.

My current work sits at the intersection of **engineering**, **procurement**, **document intelligence** and **developer tooling**.

## Selected work

### [bidlint](https://github.com/yigitcan-ozturk/bidlint)
**Technical bid compliance, with evidence before confidence.**

An open-source deterministic engine for comparing engineering specifications with vendor bids, datasheets and submittals. It preserves source provenance and produces explicit `PASS / DEVIATION / MISSING / REVIEW` findings across PDF, XLSX, IFC and multi-document vendor packages.

### [supplier-scorecard](https://github.com/yigitcan-ozturk/supplier-scorecard)
**Explainable supplier decision infrastructure.**

Combines quotation competitiveness, payment exposure, vendor risk and technical-compliance signals into transparent, policy-aware supplier recommendations.

### [rfqdiff](https://github.com/yigitcan-ozturk/rfqdiff)
**Structured quotation comparison for procurement workflows.**

A lightweight CLI for comparing supplier quotations and producing machine-readable commercial decision signals.

### [vendor-risk-engine](https://github.com/yigitcan-ozturk/vendor-risk-engine)
**Transparent supplier-risk scoring.**

Models delivery, quality, commercial, compliance and dependency risk without hiding the decision logic behind a black box.

## Engineering procurement toolchain

```text
currency-normalizer ──> rfqdiff ───────────────────────┐
                                                        │
payment-terms-parser ──────────────────────────────────┼──> supplier-scorecard
                                                        │
vendor-risk-engine ────────────────────────────────────┤
                                                        │
bidlint ──> technical compliance ──────────────────────┘
```

The projects are intentionally small at the boundaries and explicit about contracts between them. The goal is not to automate judgment away, but to make technical and procurement decisions more **auditable, deterministic and explainable**.

## Principles

- **Evidence before confidence** — decisions should point back to source evidence.
- **Deterministic where possible** — numeric and engineering rules belong in code, not model opinion.
- **Explicit uncertainty** — ambiguity should become review, not fabricated certainty.
- **Composable tools** — small stable interfaces are more useful than opaque monoliths.
- **Engineering first** — software should respect the technical context it operates in.

## Current direction

I am developing a broader engineering-software portfolio spanning specification intelligence, CAD workflows and procurement decision infrastructure, with selected work evolving under **PAMILANGA Labs**.

[GitHub projects](https://github.com/yigitcan-ozturk?tab=repositories) · [PAMILANGA](https://www.pamilanga.com)
