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
| Integration health / fail-closed bridges | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H4 synthetic E2E verifies tenant/site isolation and fail-closed bridge behaviour; H9.17 adds explicit revocable bridge authorisation to the runtime contract/validator. Customer-specific adapters remain separately gated. |
| Export / reporting / evidence packs | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | Reporting/evidence-pack lineage exists; verify current routes and permissions. |
| Configuration registry / feature flags | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | Site/jurisdiction configuration is active; keep customer/site configuration separate from shared module source. |
| Data retention / deletion / privacy controls | PRESENT | PRESENT | CONFIG-ONLY | CONFIG-ONLY | H7.1/H7.2 framework is implemented and tested: legal hold blocks deletion, reason + authorised execution are required, automatic deletion is prohibited, and the synthetic deletion drill is GREEN. Customer-specific privacy/retention approval remains HOLD and is not implied by PRESENT platform capability. |
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
3. H4/H9.17 closes the platform-level integration/fail-closed bridge row; H7.1/H7.2 closes the platform-level retention/deletion/privacy-control row while customer approvals remain external HOLD gates.
4. Run/retain CI and acceptance evidence for all promoted rows.
5. Healthcare proving-ground platform rows are now closed; next extend the verified Shared Core contracts to Council, Enterprise/Usher, Arena, Animals/Kennels, Emergency and other applicable families.


## Cross-family adoption pass — 5 October 2026

| Family / canonical repository | Adoption state | Verified position |
|---|---|---|
| Council Operations Centre | PRESENT | Canonical four-state alerts, evidence-gated closure, accountable RED/AMBER ownership, fail-closed versioned bridge, tamper-evident audit contract and Council-specific retention/deletion controls are implemented. Customer/live deployment approvals remain external gates. |
| Enterprise / Usher demo | PARTIAL | Alert vocabulary aligned to RED/AMBER/GREEN/HOLD and actionable items fail closed to HOLD without owner + due time. Static synthetic demo remains intentionally non-persistent; live enterprise integrations are not claimed. |
| Gold Coast Arena | PRESENT | Strong evidence/readiness/work-order controls already existed; issued/progressed work now requires accountable ownership. Public-prototype/live-data HOLD boundary preserved. |
| Animals — Kennels / Catteries | PARTIAL | Facility isolation, roles, audit, safety and evidence controls exist. Legacy YELLOW state migrated to canonical AMBER. Live Neon/Hyperdrive, retention/recovery and external legal/veterinary/WHS/privacy gates remain HOLD. |
| Animals — Dog Park | PARTIAL | Existing RLS, local-first privacy, encrypted storage and fail-closed provider behaviour preserved. Shared status concepts are adopted selectively; emergency “hold 3 seconds” gesture is explicitly not the HOLD alert state. |
| Emergency — Nature Has No Borders | PRESENT | Shared governance pattern already mature: organisation isolation, human authority, evidence, append-only chronology and fail-closed states. External accreditation/agency operating authority remains HOLD. |
| Government Financial Integrity / ON TRACK Australia | PARTIAL | Architecture correctly declares Shared Core capabilities and strict product isolation. Runtime adapters remain HOLD until a specific authorised integration target exists. Revenue Rescue remains standalone. |

### Cross-family conclusion

The first controlled Shared Core propagation pass is complete for Healthcare, Council, Enterprise/Usher, Arena, Animals/Kennels/Dog Park and Emergency. Remaining PARTIAL states above are deliberate where live infrastructure, customer policy, external approval or product-specific runtime integration is not truthfully established. Do not convert these external gates into code-only GREEN claims.
