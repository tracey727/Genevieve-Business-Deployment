# Current Product Routing / Extraction Queue

This document is the current routing overlay for the historical July 2026 Business Deployment archive. It does not alter the archived packages themselves.

## Already routed to canonical families

### PARKPOST
Historical ZIPs:
- `03_PRODUCT_PROTOTYPES_NEXT/GENEVIEVE_PARKPOST_CLEAN_WORKING_FINAL.zip`
- `03_PRODUCT_PROTOTYPES_NEXT/GENEVIEVE_PARKPOST_TELEMETRY_SIMULATOR_FINAL.zip`

Current specialised source: `tracey727/Genevieve-App-Council-bis-bags`  
Council umbrella/integration source: `tracey727/genevieve-council-centre-operations-centre`

Do not deploy the archive ZIPs.

### Animal Nutrition / Feeding / Allergy V1
Historical ZIP:
- `02_ACTIVE_DEPLOYMENTS_NEXT/genevieve_animal_nutrition_feeding_allergy_v1.zip`

ZIP index confirms a distinct module containing dashboard, diets, allergies, schedules, supplements, weight, stock, staff tick-offs, incidents, emergency, trust and an animal nutrition/allergy schema.

Family index: `tracey727/Genevieve-Animals-Dog-Parks-App`

Status: **PRESERVE / EXTRACT TO DEDICATED REPOSITORY BEFORE DEVELOPMENT**. It is not part of Dog Park or Kennels runtime code.

### Animal Developer Handover / Technical Architecture V1
Historical ZIP:
- `01_COMPANY_MASTER_FILES/genevieve_animal_developer_handover_technical_architecture_v1.zip`

ZIP index confirms architecture, module, data, API, security, build-phase, testing, production-warning and build-lock material.

Family index: `tracey727/Genevieve-Animals-Dog-Parks-App`

Status: **PRESERVE AS SHARED ANIMAL-SENSE ENGINEERING REFERENCE**.

## Unique orphan requiring its own repository

### Food Safety V15 No-Guess
Historical ZIP:
- `02_ACTIVE_DEPLOYMENTS_NEXT/GENEVIEVE_APP_FOOD_SAFETY_V15_NO_GUESS_FULL_DEPLOY.zip`

ZIP index confirms a complete static product package with:
- `index.html`, `styles.css`, `app.js`
- privacy, terms and safety pages
- PWA manifest/service worker
- build verification
- food icon asset
- historical Netlify/Vercel deployment files

No other repository currently contains this Food Safety V15 product.

Status: **UNIQUE — DO NOT DELETE.** Create a dedicated private canonical repository before further build/deployment. When extracted, migrate deployment deliberately to GitHub + Cloudflare; do not carry forward the archived Netlify/Vercel deployment files as active configuration.

Exact extraction inventory and provenance: `02_ACTIVE_DEPLOYMENTS_NEXT/FOOD_SAFETY_V15_EXTRACTION_MANIFEST.md`.

## Archive rule

The old folder names and July manifest are historical evidence. Do not use `02_ACTIVE_DEPLOYMENTS_NEXT` or the 2026-07-10 manifest as the current product priority list.
