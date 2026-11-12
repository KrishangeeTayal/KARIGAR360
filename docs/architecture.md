# Proposed Architecture

> This is a conceptual architecture for the proposed product. It is not an implemented system diagram.

## High-level components

- **Jeweller web application:** job creation, material issue, oversight, discrepancy review and settlement.
- **Karigar mobile/PWA experience:** job acknowledgement, progress updates, return recording and reconciliation review.
- **Backend API:** authentication, role permissions, job lifecycle and event validation.
- **PostgreSQL:** structured job, party, material movement, event and approval records.
- **AI assistance layer:** optional voice/document extraction, structured capture, summaries and follow-up prompts.
- **Deterministic reconciliation service:** evaluates recorded quantities using explicit, agreed rules and decimal arithmetic.
- **Evidence storage:** stores supporting documents and references linked to job events.

## Separation of responsibilities

### AI assistance
AI may help extract or summarise information, but extracted values should be reviewed and confirmed before becoming authoritative records.

### Reconciliation
The reconciliation service should use deterministic arithmetic and explicit rules. It should account for applicable material categories and agreed terms rather than infer liability.

### Human decisions
Both parties should be able to review and dispute a proposed reconciliation. Settlement and job closure require explicit approval.

## Proposed technology

- Frontend: Next.js / React PWA
- Backend: Python FastAPI
- Database: PostgreSQL
- AI orchestration: Mastra
- Reconciliation: Python Decimal arithmetic
- Evidence: secure file storage

## Important future design considerations

- Role-based access and tenant isolation.
- Authentication and consent.
- Auditability and event provenance.
- Decimal precision and unit normalisation.
- Versioned reconciliation rules.
- Evidence access controls and retention.
- Idempotent event submission and conflict handling.
- Backup, recovery and data export.

These considerations must be addressed during prototype design and implementation.
