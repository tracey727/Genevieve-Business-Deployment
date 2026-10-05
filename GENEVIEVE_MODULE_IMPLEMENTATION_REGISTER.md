# GENEVIEVE Module Implementation Register

**Started:** 5 October 2026  
**Purpose:** master control matrix for reusable GENEVIEVE capabilities.  
**Allowed states:** PRESENT | PARTIAL | CONFIG-ONLY | MISSING | NOT-APPLICABLE | PROHIBITED

This register is deliberately evidence-based. A module is not marked PRESENT merely because a dashboard label exists. PRESENT means the current repository evidence shows a real implementation; portfolio acceptance still requires tests, infrastructure and configuration to agree.

## Initial proving-ground matrix

| Module | Shared Core / active Healthcare engine (`genevieve-core-platform`) | Westmead configuration | Coomera configuration | Burnie configuration | Verification / next action |
|---|---|---|---|---|---|
| Identity / authentication / role permissions | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H9.04 documents Cloudflare Access + Neon site RBAC. Re-run acceptance tests before production claim. |
| Tenant / organisation / site isolation | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | Site-scoped RBAC and least-privilege Neon runtime are documented. Keep fail-closed isolation tests in acceptance gate. |
| Universal alert engine: RED / AMBER / GREEN / HOLD | PARTIAL | PARTIAL | CONFIG-ONLY | CONFIG-ONLY | Universal vocabulary exists, but end-to-end propagation/display remains the current repair target. No GREEN claim until every applicable ledger/module reflects operational state. |
| Evidence ledger / immutable audit trail | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | Persistent record/history and action audit identity are implemented; verify append-only behaviour in acceptance pass. |
| Action ownership / due dates / escalation | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H9.02 action catalogue is live; verify due/escalation presentation against all operational modules. |
| Executive decision & commitment capture | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H8-series decision/work-capture capability is part of the active Healthcare build; verify configuration exposure. |
| Safety / security / incident controls | PARTIAL | PARTIAL | CONFIG-ONLY | CONFIG-ONLY | Current proving-ground priority. Safety/security must be wired to actual ledgers, evidence and alert states, not decorative cards. |
| Workforce / coverage / competency status | PARTIAL | PARTIAL | CONFIG-ONLY | CONFIG-ONLY | Module exists in Healthcare lineage; verify alert propagation, ownership and evidence end-to-end. |
| Facilities / utilities / preventive maintenance | PARTIAL | PARTIAL | CONFIG-ONLY | CONFIG-ONLY | Module exists; verify utilities/fault/readiness alert rules and evidence closure. |
| External review / submission tracking | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H7.8 lineage established; verify site configuration and evidence links. |
| Integration health / fail-closed bridges | PARTIAL | PARTIAL | CONFIG-ONLY | CONFIG-ONLY | Architecture requires fail-closed bridges; perform contract/error-state verification before PRESENT acceptance. |
| Export / reporting / evidence packs | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | Reporting/evidence-pack lineage exists; verify current routes and permissions. |
| Configuration registry / feature flags | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | Site/jurisdiction configuration is active; keep customer/site configuration separate from shared module source. |
| Data retention / deletion / privacy controls | PARTIAL | PARTIAL | CONFIG-ONLY | CONFIG-ONLY | Do not claim complete privacy lifecycle until retention/deletion tests and policy mapping are verified. |
| Operational readiness / commissioning / defects | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H8.38 readiness is live; verify downstream configuration propagation before cross-family reuse. |

## Interpretation

- **Shared Core / active Healthcare engine** currently lives in `genevieve-core-platform`; this is an architectural recovery state, not permission to clone the engine into new site repositories.
- **Westmead** is the first proving-ground configuration and must reach the acceptance gate before propagation.
- **Coomera** and **Burnie** are marked CONFIG-ONLY in this first pass where the configuration pattern is known but equivalent end-to-end runtime verification has not yet been completed.
- `Healthcare` is currently an empty reserved repository and is not treated as a second canonical runtime.
- `-genevieve-core-platform` is an empty placeholder and is not a Shared Core implementation.

## Next controlled pass

1. Audit the active Healthcare engine module-by-module, beginning with universal alerts, Safety, Security, Workforce and Facilities.
2. For each PARTIAL row, trace: source state → rule evaluation → alert state → ledger/card display → ownership/escalation → evidence/audit.
3. Repair only the broken link; do not redesign unrelated UI or modules.
4. Run tests/CI and verify the live or preview environment.
5. Promote a row from PARTIAL to PRESENT only after the acceptance evidence is recorded.
6. Once Westmead is GREEN, propagate the proven contracts to Coomera and Burnie, then extend this matrix to Council, Enterprise/Usher, Arena, Animals/Kennels, Emergency and other applicable families.
