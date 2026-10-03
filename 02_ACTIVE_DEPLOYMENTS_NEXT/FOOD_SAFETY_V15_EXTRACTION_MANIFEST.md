# GENEVIEVE App™ Food Safety V15 No-Guess — Extraction Manifest

## Source package

Repository:
`tracey727/Genevieve-Business-Deployment`

Archive path:
`02_ACTIVE_DEPLOYMENTS_NEXT/GENEVIEVE_APP_FOOD_SAFETY_V15_NO_GUESS_FULL_DEPLOY.zip`

Git blob SHA:
`0606a925662fa409a41893aa659f8cb4bafd3290`

Archive size:
**15,533 bytes**

## Classification

**UNIQUE STANDALONE PRODUCT — DO NOT DELETE**

Account-wide repository/code search found no second Food Safety V15 application source. The older `GENEVIEVE Food & Grocery` references exist only in historical master registers and are not a current competing source repository.

This package is not part of:
- Family Budget Cookbook runtime;
- Irene's Sunday Cook-Up runtime;
- Animal Nutrition / Feeding / Allergy;
- Revenue Rescue.

Do not merge its runtime into those products merely because they involve food.

## ZIP contents

1. `index.html`
2. `styles.css`
3. `app.js`
4. `privacy.html`
5. `terms.html`
6. `safety.html`
7. `manifest.webmanifest`
8. `sw.js`
9. `robots.txt`
10. `_redirects`
11. `netlify.toml`
12. `vercel.json`
13. `DEPLOYMENT_INSTRUCTIONS.txt`
14. `README.md`
15. `BUILD_VERIFICATION.json`
16. `assets/genevieve-food-icon.svg`

The archive also contains the `assets/` directory entry.

## Required extraction destination

Create a dedicated private canonical repository for **GENEVIEVE App™ Food Safety V15 No-Guess** before resuming development or deployment.

Suggested repository name:
`genevieve-food-safety`

The dedicated repository should preserve the original extracted files in its first provenance commit, then migrate deployment separately.

## Deployment migration rule

Historical deployment files inside the ZIP:
- `netlify.toml`
- `vercel.json`
- `_redirects`
- old deployment instructions

must be treated as **historical source evidence**, not as the current deployment standard.

Current ON TRACK by TRACE platform direction:
- GitHub source control;
- Cloudflare for active hosting/runtime;
- Neon only if a later governed version genuinely requires persistent data;
- no active Vercel or Netlify dependency.

Before removing historical header/routing behaviour, inspect those legacy config files and preserve any valid security headers or redirects in the Cloudflare equivalent.

## First canonical-repository gate

Before the extracted repository is called current or deployable:

1. extract the ZIP without editing its application content;
2. record provenance back to this archive path and Git blob SHA;
3. inventory security headers, redirects and service-worker behaviour;
4. separate historical Netlify/Vercel configuration from Cloudflare configuration;
5. add repository CI/integrity checks;
6. review food-safety statements and any operational claims before public use;
7. do not mix recipe/dietary suitability logic from Family Budget Cookbook into this product without a deliberate product-contract review.

## Family reference

The current family map is in:
`tracey727/Budget-cookbook-/01_MASTER_BLUEPRINT/FOOD_PRODUCT_FAMILY.md`
