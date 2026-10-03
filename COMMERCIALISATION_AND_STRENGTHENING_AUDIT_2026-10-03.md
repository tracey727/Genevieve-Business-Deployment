# Commercialisation & Repository Strengthening Audit — 3 October 2026

## Scope

This audit reconciles:
- all 119 owned GitHub repositories;
- the current repository-family register;
- the July/August GENEVIEVE archive manifests and master project registers;
- recovered portfolio/library evidence for aged care, childcare, the Main Command Centre, Animal Passport/Facilities and related governed modules;
- current October product work including Lens Saver.

This is a **portfolio-routing document**, not a claim that every recorded concept is production-ready, legally approved, clinically validated or commercially proven.

## Portfolio rule

Do **not** create one repository/business for every archived module.

Use three dispositions:
1. **STANDALONE BUSINESS / DEDICATED REPOSITORY** — distinct customer, data/governance boundary or commercial product.
2. **STRENGTHEN EXISTING PRODUCT** — reusable capability belongs inside an existing canonical product or behind an explicit shared contract.
3. **INCUBATOR / HOLD** — preserve IP/evidence but do not build until engineering, legal, clinical, ethical or market gates justify it.

---

# A. Existing repositories that already support a commercial product

These should be commercialised from their existing canonical repositories rather than duplicated:

- Revenue Rescue — protected existing commercial product.
- ON-TRACK Stock Sense — inventory/stock intelligence SaaS.
- Psych-Savings — psychology/practice savings and workflow product.
- ON TRACK Psychological Command Centre — governed practice command centre.
- Civic Project Controls — generic clean-room project-controls product.
- Property Operations Command Centre — real-estate/property-operations product.
- Gold Coast Arena Command Centre — venue/project-specific command-centre product.
- Nerang Street Command Centre — small-project pilot/product.
- ON TRACK Australia — government accountability/pilot product.
- GENEVIEVE Kennels Command Centre — kennel/cattery operational product.
- GENEVIEVE Gruff Dog Park — consumer/animal-safety product.
- VIP Pet Travel — premium pet-travel product.
- Family Budget Cookbook — consumer household budget/meal-planning product.
- ScriptGuard — governed prescription-expiry/repeat-protection product.
- Medication Safety — governed medication/dispensing safety product.
- Support Competency — workforce/participant-safety competency product.
- GENEVIEVE Dating — public/multi-user dating platform foundation.
- PARKPOST and CLEAN-SAFE — specialised council/facility products.
- Super Response editions — separate web/Python/Windows products, subject to current platform migration where still required.
- Macro System — business pattern/waste/prevention product, subject to Cloudflare migration.
- Ancestor Journey — personal product that could later be generalised only from a clean generic template, never by publishing Tracey's private content.
- Grounded / Restore / My-psych — personal tools; any consumer commercialisation should be a clean generic extraction, not publication of personal data/configuration.

---

# B. New standalone businesses / dedicated repositories justified by evidence

## 1. Lens Saver — CREATE
**Target repository:** `lens-saver` (private)

Distinct consumer Vision / Optical product:
- contact-lens prescription capture/verification;
- exact-match checks;
- Australian seller comparison;
- cheaper-option analysis;
- rebate/discount handling;
- 6/12-month cost estimates;
- reorder/expiry reminders;
- local export/delete.

Keep completely separate from Revenue Rescue.

## 2. Food Safety V15 No-Guess — RECOVER
**Suggested repository:** `genevieve-food-safety` (private)

Unique standalone static/PWA product already preserved in this archive. Existing issue #3 tracks extraction.

## 3. Animal Nutrition / Feeding / Allergy — RECOVER
**Suggested repository:** `genevieve-animal-nutrition` (private)

The archive contains a distinct module package. It is not present in current Dog Park or Kennels runtime and should not be collapsed into either product. It may later integrate through Animal Sense contracts.

## 4. Aged Care Command Centre V2.1 — RECOVER
**Suggested repository:** `genevieve-aged-care-command-centre` (private)

Library evidence records a V2.1 Aged Care Command Centre / Production Module with:
- 21/21 unit tests passing;
- secure APIs and PostgreSQL migration;
- older-person/rights profiles;
- care/live rounds;
- clinical safety;
- incidents/SIRS;
- staffing/WHS;
- Queensland emergency;
- quality standards/indicators;
- fail-safe readiness controls.

It remains provider/configuration/authorisation gated. Do not merge into Health Navigator, Medication Safety or the Psychology Command Centre.

## 5. Childcare Safety / Operations family — RECOVER AS ONE SECTOR PRODUCT
**Suggested repository:** `genevieve-childcare-command-centre` (private)

The master register contains childcare centre operations, excursion/transport safety, collection authority, staff ratios, sleep checks, allergy/anaphylaxis, medication, incident/injury, missing-child, protection escalation, emergency/evacuation, parent communication and learning/documentation concepts.

Do **not** create a separate app/repository for every childcare submodule. Recover/build one governed childcare product with configurations/modules.

Growing Up remains a separate education product and should not be swallowed into childcare operations.

## 6. ON TRACK Work Value — GENERIC COMMERCIAL EXTRACTION
**Suggested repository:** `on-track-work-value` (private)

`andy-my-work-value` is a strong product architecture but is person-specific. Build a clean generic commercial version from the proven worker-owned evidence / role-and-pay-review model. Do not commercialise Andy's personal repository or data directly.

---

# C. Shared platform/business infrastructure worth recovering

## Main Command Centre / Shared Production Core
Historical library records identify:
- `GENEVIEVE_CORE_PLATFORM_HEALTH_ECOSYSTEM_AUDITED_V1_19.zip`;
- `GENEVIEVE_ANIMAL_HEALTH_BRIDGE_AUDITED_V1_20.zip`;
- `GENEVIEVE_MAIN_COMMAND_CENTRE_PRODUCTION_CORE_V1_24.zip`.

The V1.24 record describes tested shared capabilities including identity, organisation/tenant separation, permissions, consent evidence, approval gates, notification/acknowledgement, durable queues, retry/dead-letter handling, deduplication, append-only audit chains, monitoring, backup/restore and authenticated Animal–Health bridge controls.

Historical repository intent:
- `genevieve-main-command-centre`;
- `genevieve-core-platform`;
- `genevieve-animal-health-bridge`.

These repositories are absent from the current GitHub account.

**Action:** recover these as private infrastructure repositories if the actual source packages/checksums can be materialised from the library. Do not recreate them from memory if the verified archives can be recovered.

**Boundary:** shared infrastructure may carry identity, consent, audit, delivery and minimum-authorised status. It must not become a shared unrestricted clinical/veterinary database.

---

# D. Strengthen existing repositories instead of creating duplicates

## Animal family — shared identity/passport + emergency handoff
Historical governed Animal branch evidence included Animal Passport, canonical Animal/Passport identifiers, Facilities, Veterinary, Welfare, Nutrition/Allergy and Biosecurity.

Current Gruff Dog Park already has voluntary QR exchange and emergency contacts, but does not clearly implement:
- temporary animal-care handoff;
- responsible-contact succession;
- lost/found/reunification workflow.

VIP Pet Travel does not currently expose an Animal Passport/travel-document module.

**Action:** define a shared Animal Identity / Passport contract in the Animal Sense family and integrate only the minimum approved fields into Dog Park and VIP Pet Travel. Do not create competing passport implementations in each repo.

## Kennels — commercial facility-operations depth
Current Kennels already has bookings, custody, rounds, transport, stock, compliance and maintenance checks.

Archived Animal family modules identify additional commercial capability themes:
- analytics/reporting;
- invoicing/payments/subscriptions;
- richer asset/facility maintenance;
- workforce/contractor management;
- client portal/service management;
- supplier/procurement.

**Action:** add these as a governed commercial backlog to the canonical Kennels repo. Reuse concepts, not old deployment assumptions.

## Family Budget Cookbook — recover grocery capture/optimisation
The historical Food & Grocery project recorded scanner, pantry and grocery-optimiser work. The current Cookbook already has pantry, pricing, pack conversion, shopping-list and weekly-planner architecture, but no barcode/scanner intake.

**Action:** add barcode/scanner grocery intake as a future phase feeding the existing canonical ingredient/pantry model. Do not revive a second Food & Grocery app.

## Civic Project Controls — weather/disruption communications
A historical Weather Cancellation Broadcast Tool exists as a concept. Civic Project Controls currently has no weather/disruption/broadcast module.

**Action:** add a future governed disruption-notice module:
- authorised sender;
- affected project/site;
- source weather/evidence reference;
- cancellation/delay decision remains human;
- acknowledgement and audit trail;
- no autonomous closure or mass messaging without explicit authority.

This may also become reusable in construction/company-specific siblings such as Usher, but Civic should own the generic contract.

## Nature Has No Borders — DO NOT DUPLICATE old emergency modules
Current Nature Has No Borders already contains:
- evacuation-support structures;
- CLEARWAY;
- traffic-control coordination evidence;
- cross-agency acknowledgement and escalation boundaries.

Do not import the old Emergency Response/Evacuation packages wholesale. They are reference lineage only unless a specific missing capability is proven.

## Dog Park emergency identity
The historical G-023 requirement for responsible-contact / temporary animal-care workflow remains only partially represented in current Dog Park. Add it through the shared Animal Passport/emergency-handoff contract rather than a new app.

---

# E. Incubator / physical-product businesses — preserve, do not software-build blindly

These can become businesses, but the next gate is professional engineering/product validation rather than GitHub feature work:

- AURA-800 Smart Coffee Table.
- GENEVIEVE Smart Boardroom Table.
- GENEVIEVE Sanctuary Pod.
- Automated body-shaving system.
- Construction furniture lift / hoist.
- Women in automotive smart leverage system.
- BagStation / physical waste-handling station (already has a stronger commercial/grant path than most physical concepts).

For physical products, create a dedicated product repository only when it will hold controlled CAD/specification/test/BOM/supplier evidence. Do not treat concept images or speculative features as an engineered design.

---

# F. Concepts to hold rather than commercialise immediately

- Compatibility placement system — requires ethics, consent, discrimination and housing/care-law review.
- Auslan Companion — requires Deaf-community-led validation; should not be commercialised from an unvalidated accessibility concept.
- Automated high-risk clinical/health functions — remain behind clinical/regulatory gates.
- Personal mental-health/support apps — do not turn personal histories or private configuration into a commercial dataset.
- Historical Firebase/Vercel platform packs — source/reference only; do not reintroduce obsolete deployment direction.

---

# G. Repository creation / recovery queue

1. `lens-saver`
2. `genevieve-food-safety` — issue #3 already open
3. `genevieve-animal-nutrition`
4. `genevieve-aged-care-command-centre`
5. `genevieve-childcare-command-centre`
6. `on-track-work-value`
7. Recover `genevieve-main-command-centre`, `genevieve-core-platform`, and `genevieve-animal-health-bridge` only from verified source archives/checksums.

The connected GitHub tool currently cannot create brand-new repositories. These are therefore tracked as explicit recovery/creation tasks rather than pretending the repositories already exist.

---

# H. Highest-value strengthening actions already supported by current evidence

- Recover Main Command Centre shared infrastructure rather than rebuilding shared identity/audit/queue plumbing separately in every product.
- Add shared Animal Passport/emergency handoff to Dog Park + VIP Pet Travel.
- Add enterprise facility commercial modules to Kennels.
- Add barcode/scanner intake to the existing Budget Cookbook roadmap.
- Add authorised weather/disruption notices to Civic Project Controls.
- Extract a generic commercial Work Value product from the Andy-specific implementation.
- Recover Aged Care V2.1 into its own governed private repository.
- Recover Childcare as one sector command-centre family, not dozens of mini-apps.
- Create Lens Saver as the new Vision / Optical standalone consumer product.


---

# I. Portfolio cleanup addendum — newly routed opportunities

- **Shelter Command Centre™ / Nobody Left Behind** — future standalone housing-support operations family; issue #13; future private target `on-track-shelter-command-centre`. Preserve case ownership/follow-up/outcome accountability. Older compatibility research remains separately governed and is not implemented by this cleanup.
- **GENEVIEVE Move** — Enterprise / Operations configuration; issue #14. Preserve relocation/logistics coordination scope without creating another shared core or repository until a named buyer/pilot exists.
- **ON TRACK Small Business Sales Kit** — productisation candidate; issue #15. Define a generic catalogue/order/payment/custom-work workflow from reusable patterns while keeping client-specific content/data separate. Suggested future repo only after the generic boundary is clean: `on-track-small-business-sales-kit`.
- **Physical / 3D Fabrication incubator** — issue #16. Keep the completed small-car package, 1978–79 Datsun accessory concept and other physical products in one incubator. Dedicated repos require controlled CAD/specification/BOM/test/supplier evidence.

Full routing record: `PORTFOLIO_CLEANUP_ADDENDUM_2026-10-03.md`.

---

# J. Full conversation + file reconciliation

A complete retrievable-history reconciliation is archived in `FULL_CONVERSATION_FILE_ECOSYSTEM_RECONCILIATION_2026-10-03.md`.

Key corrections/additions:
- explicitly places LISTENS, ADHD, Session Continuity, Health Navigator, Connection/Relationship, Synchronicity/Tarot, Macro System and Super Response in the ecosystem;
- maps the Food V10–V18 lineage to Food Safety / Family Budget Cookbook / Stock Sense rather than separate products;
- routes Waterproofing, painting, weather-broadcast and relocation concepts into Enterprise/Civic/Usher families;
- records the full 14-program Government Accountability stack under ON TRACK Australia;
- corrects Mind Mates / GIGI to excluded/client-specific provenance rather than ON TRACK-owned commercial assets;
- preserves physical-product concepts under one fabrication incubator;
- keeps private correspondence, complaints and personal evidence out of the commercial product register;
- confirms GENEVIEVE SEISMIC™ is already correctly routed inside Nature Has No Borders;
- leaves Revenue Rescue untouched.
