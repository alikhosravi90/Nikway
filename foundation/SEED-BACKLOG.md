# NIKWAY SEED — Execution Backlog v0.1

Source: [NIKWAY-SEED.md](NIKWAY-SEED.md) (NKW-SEED-0001, proposed).
Status: PROPOSED. This is a planning backlog, not authorization to deploy or alter production.
Priority: P0 foundation; P1 prototype; P2 acceptance. Each task requires an owner, evidence and review before closure.

| ID | Priority | Deliverable | Acceptance criteria | Dependency |
|---|---|---|---|---|
| SEED-01 | P0 | Cross-repository conceptual and ADR audit | Sources, conflicting definitions, versions and unresolved decisions linked; no inferred approvals | None |
| SEED-02 | P0 | Founder review and authority charter | Explicit owner, approval status and change-control authority recorded | SEED-01 |
| SEED-03 | P0 | Source-of-record/authority/evidence policy | Per-domain record authority, precedence, conflict process and provenance defined | SEED-02 |
| SEED-04 | P0 | Versioned foundation ontology | Concepts, relationships, definitions, examples and competency questions reviewed | SEED-01 |
| SEED-05 | P0 | Claim/evidence/provenance contract | Epistemic and approval states independent; missing sources and conflicts represented | SEED-03,04 |
| SEED-06 | P1 | Rule and inference contract | Explicit rule inputs, outputs, explanations, conflicts and deterministic authorization tests | SEED-05 |
| SEED-07 | P1 | Memory scope and lifecycle design | Individual/team/organizational/institutional/federated scopes; access, time, retention and deletion tests | SEED-05 |
| SEED-08 | P1 | Competency, method and tool registry design | Knowledge/skill/method/tool/evidence separated; BABOK/BIZBOK/EFQM/Baldrige/Shingo mapped with licensing notes | SEED-04 |
| SEED-09 | P1 | Agent authority and execution contracts | Roles, least privilege, tool grants, audit and approval gates defined | SEED-03,06 |
| SEED-10 | P1 | Reflection and governed method-change loop | Proposals, independent evaluation, approval, version and rollback demonstrated | SEED-07,09 |
| SEED-11 | P1 | First-/second-/third-order benchmark | Repeatable synthetic scenario, baseline, provenance, error and unauthorized-action metrics | SEED-06,10 |
| SEED-12 | P2 | Architecture acceptance and decision record | Evidence-based GO/PILOT/HOLD/NO-GO with gaps, owner and next actions | SEED-11 |

## First sprint (no production change)
1. SEED-01: inventory foundation documents and conflicting definitions in the accessible NIKWAY repositories.
2. SEED-02: prepare founder decision record; do not self-ratify.
3. SEED-03: draft domain source-of-truth and authority matrix.
4. SEED-04: draft minimal ontology and competency questions.
5. SEED-05: validate claim/evidence/provenance schema with synthetic examples.

## Definition of done
- Traceable source link and version.
- Named responsible role and reviewer.
- Explicit assumptions and unresolved conflicts.
- Reproducible evidence or test for testable claims.
- Recorded approval decision; no silent promotion of hypotheses to verified facts.

## Safety / scope
- No automatic production writes, no migrations, no secret or private customer data.
- Keep architecture and operational source-of-record boundaries separate.
- Do not infer that a successful commit ratifies the SEED.
