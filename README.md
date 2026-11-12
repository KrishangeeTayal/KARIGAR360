# KARIGAR360

**Every Gram Accounted For. Every Job Traceable. Every Settlement Transparent.**

KARIGAR360 is a proposed AI-powered, two-sided job-work management and gold-accountability platform for jewellers and independent karigars.

It is designed to create a shared, evidence-backed record of each job—from material issuance and acknowledgement through production, returns, reconciliation and mutually approved settlement.

> **Project status:** Concept and proposal stage for Tech4Bharat 2026, Problem Statement PS 2.2 — Jeweltech. The prototype and implementation are planned for a subsequent stage. This repository currently contains project documentation and the pitch presentation; it does not claim that the product is deployed or implemented.

## The problem

Jewellery job-work can involve gold and other materials moving between jewellers and independent karigars. Records may be spread across paper registers, messages, verbal confirmations and weighing slips. This can make it difficult for both parties to see one consistent history of material movement, job progress, returns and settlement.

KARIGAR360 focuses on the shared record of responsibility throughout the job lifecycle—not simply on tracking gold.

## Proposed solution

A shared digital workflow for both sides:

- **Digital job ledger:** a unique, traceable record for each job.
- **Material acknowledgement:** record material issued and confirm receipt.
- **Job tracking:** capture progress, deadlines and partial returns.
- **Intelligent reconciliation:** compare recorded material flows against agreed rules and flag differences for review.
- **Transparent settlement:** prepare a statement for review and approval by both parties.

## How it works

1. **Create job** — the jeweller records material details, agreed terms, the karigar and expected completion date.
2. **Issue and acknowledge** — the jeweller records material issued; the karigar acknowledges receipt.
3. **Track production** — the karigar records progress and production events.
4. **Record returns** — partial and final returns are recorded with relevant weights and evidence.
5. **Reconcile** — the system compares the material flow against agreed rules and flags differences for review.
6. **Approve and close** — both parties review the reconciliation and approve settlement before closure.

## AI and trust safeguards

KARIGAR360 separates AI-assisted capture from authoritative calculations and decisions.

- Proposed AI assistance includes voice-to-record, document extraction, job summaries and follow-up reminders.
- Material reconciliation is intended to use deterministic arithmetic and agreed business rules—not LLM-generated estimates.
- Relevant factors may include gross/net weight, purity, stones and non-gold components, agreed allowances, recoverable scrap, partial returns, units and measurement precision.
- A discrepancy is a request for review, not an accusation.
- Both parties can dispute a proposed reconciliation.
- Corrections should remain traceable in an append-only history.
- Settlement and job closure require explicit human approval.

## Proposed technology foundation

| Layer | Proposed technology |
|---|---|
| Frontend | Next.js / React PWA |
| Backend | Python FastAPI |
| Database | PostgreSQL |
| AI orchestration | Mastra |
| Reconciliation | Python `Decimal` arithmetic |
| Evidence | Secure file storage |

These are proposed technologies, not claims of completed implementation.

## Differentiation hypothesis

The proposed distinction is a shared, evidence-backed job lifecycle with two-sided acknowledgement, mutual reconciliation and approval. This is a hypothesis to validate with jewellers and karigars. The project does not claim that existing jewellery software lacks job-work or gold-ledger functionality.

## Business model hypothesis

A potential SaaS model could include starter, professional and multi-user business tiers, with optional premium analytics, integrations and document intelligence. Pricing, market sizing and willingness to pay have not yet been established.

## Validation plan

The next discovery step is to interview jewellers and, where possible, karigars to understand current workflows, reconciliation practices, adoption barriers and the value of a shared record. No customer interviews, deployments or pilot results are claimed in this repository.

See:
- [Problem statement](docs/problem-statement.md)
- [Solution overview](docs/solution-overview.md)
- [Architecture](docs/architecture.md)
- [User workflows](docs/user-workflows.md)
- [Interview guide](research/interview-guide.md)
- [Validation scorecard](research/validation-scorecard.md)

## Pitch presentation

The 10-slide Tech4Bharat 2026 presentation is available at [`docs/KARIGAR360_Tech4Bharat2026_Pitch_Deck.pptx`](docs/KARIGAR360_Tech4Bharat2026_Pitch_Deck.pptx).

## Current scope

**Included now:** project concept, proposed workflows, architecture direction, validation plan and pitch deck.

**Not included yet:** working frontend, backend APIs, database implementation, AI agents, integrations or a deployed prototype. These are planned for a later stage.

---

**KARIGAR360 — Trust should not depend on memory.**
