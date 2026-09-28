# ChatGPT Operating Instructions

## Purpose

These instructions define how ChatGPT should resume and operate the two-brand Meta Ads project.

Brands:
- Magasin Coffee
- Magasin Cup

## When the user says

Examples:
- "Đọc lại dự án Meta Ads"
- "Đọc source of truth rồi tiếp tục"
- "Kiểm tra Meta Ads theo chiến lược hiện tại"
- "Xem lại chiến dịch quảng cáo"
- "Đọc lại Magasin Coffee"
- "Đọc lại Magasin Cup"

Follow the reload sequence below.

## Reload sequence

1. Read `SOURCE_OF_TRUTH.md`.
2. Read root `CURRENT_STATE.md`.
3. Read `brands/README.md`.
4. Identify which brand the request concerns.
5. Read that brand's:
   - `BRAND.md`
   - `CURRENT_STATE.md`
   - `strategy.md`
6. If the request concerns both brands, read both brand folders and keep analysis separated by brand.
7. Read relevant shared files in `strategy/`.
8. Read relevant files in `campaigns/active/` and `campaigns/planned/`.
9. Read relevant experiments.
10. Read recent entries in `decisions/decision-log.md`.
11. Read the latest relevant performance review.
12. Read live Meta Ads account state and current performance data.
13. Assign each live object to Magasin Coffee, Magasin Cup, or `UNRESOLVED`.
14. Compare GitHub state with Meta Ads state.
15. Explicitly identify mismatches, stale assumptions, missing data, and unresolved decisions.
16. Produce analysis and proposed actions.
17. Do not make consequential Meta Ads changes without explicit user approval.
18. After an approved strategic or operational change, update the relevant GitHub records.

## Brand identification

Preferred evidence:
1. confirmed Instagram/Page identity;
2. campaign/ad naming;
3. ad creative/body;
4. destination;
5. existing documented mapping.

Confirmed mappings as of 2026-09-28:
- `magasincoffee` → Magasin Coffee
- `th.xuonginlymagasincupcan` → Magasin Cup

If evidence conflicts or is insufficient, use `UNRESOLVED` rather than guessing.

## Source priority

When sources conflict:

- live Meta Ads wins for current platform state and metrics;
- `SOURCE_OF_TRUTH.md` wins for enduring project rules;
- relevant brand files win for brand-specific intent;
- the latest approved decision wins for strategy;
- campaign and experiment files win for their documented hypothesis and intended plan;
- conversation memory is supplementary only.

## Analysis discipline

Separate:
- observed fact;
- interpretation;
- hypothesis;
- recommendation;
- approved action;
- executed action.

Never report a recommendation as executed unless the external platform confirms the change.

## Brand separation discipline

Never:
- average Coffee and Cup KPIs into one benchmark for decision-making;
- use Cup lead economics to judge Coffee;
- use Coffee awareness economics to judge Cup;
- assign an unlabeled live object to a brand without evidence.

## Measurement discipline

Until conversion tracking is verified:
- do not treat connector-reported purchase events as verified sales;
- do not use ROAS as a primary optimization metric when purchase value is missing or unreliable;
- use the closest verified business outcome available for each brand.

## Update discipline

After meaningful work, update:
- root `CURRENT_STATE.md` for account-level state;
- brand `CURRENT_STATE.md` for brand-specific state;
- brand `strategy.md` for approved strategic changes;
- campaign file for campaign-specific changes;
- experiment file for experiment status/results;
- performance review for measured outcomes;
- decision log for durable strategic decisions.

## Safety

Before launch, pause, enable, budget changes, targeting changes, creative replacement, or other consequential live mutations:
- re-read current Meta Ads state;
- identify the exact brand;
- summarize the exact proposed change;
- obtain explicit approval;
- execute only the approved scope;
- verify the result;
- record the outcome in GitHub.
