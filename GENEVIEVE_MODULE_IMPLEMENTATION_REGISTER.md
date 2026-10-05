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
| Universal alert engine: RED / AMBER / GREEN / HOLD | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H9.13 repaired governed-record authority; H9.16 verifies state → resolver → dashboard → ownership/escalation/evidence for Westmead. |
| Evidence ledger / immutable audit trail | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | Persistent record/history and action audit identity are implemented; verify append-only behaviour in acceptance pass. |
| Action ownership / due dates / escalation | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H9.02 action catalogue is live; verify due/escalation presentation against all operational modules. |
| Executive decision & commitment capture | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H8-series decision/work-capture capability is part of the active Healthcare build; verify configuration exposure. |
| Safety / security / incident controls | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H9.16 verifies shared Safety/Security operational contracts, governed alert state, owners and closure evidence; prohibited autonomous/tactical actions remain excluded. |
| Workforce / coverage / competency status | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H9.16 verifies Workforce alert propagation plus governed competency/staff-safety ownership and evidence requirements. |
| Facilities / utilities / preventive maintenance | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H9.16 verifies Facilities alert path; governed work orders require owner/due/status/alert and evidence-backed closure. |
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

1. Westmead H9.13/H9.16 has closed the first proving-ground alert/Safety/Security/Workforce/Facilities pass.
2. Verify Coomera and Burnie inherit the proven contracts strictly by configuration, without claiming live customer deployment or external approval.
3. Continue the remaining Healthcare PARTIAL rows: integration health/fail-closed bridges and data retention/deletion/privacy controls.
4. Run tests/CI and record acceptance evidence before any promotion to PRESENT.
5. Then extend the verified Shared Core contracts to Council, Enterprise/Usher, Arena, Animals/Kennels, Emergency and other applicable families.
