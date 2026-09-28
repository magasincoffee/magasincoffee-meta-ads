# Magasin Meta Ads — Source of Truth

Last updated: 2026-09-28

## Scope

This repository governs Meta advertising strategy for two separate brands:

- **Magasin Coffee**
- **Magasin Cup**

It does not govern the Magasin Coffee web application or unrelated engineering projects.

## Brand registry

### Magasin Coffee

- Brand: Magasin Coffee
- Confirmed live Instagram identity observed in Meta Ads: `magasincoffee`
- Current observed advertising theme: local beverage / coffee offers
- Brand-specific source files: `brands/magasin-coffee/`

### Magasin Cup

- Brand: Magasin Cup
- Confirmed live Instagram identity observed in Meta Ads: `th.xuonginlymagasincupcan`
- Current observed advertising theme: plastic cups, custom logo printing, nationwide/B2B sales and messaging
- Brand-specific source files: `brands/magasin-cup/`

## Live platform

- Platform: Meta Ads
- Connected ad account: Vi Tran
- Account status: ACTIVE
- Currency: VND
- Timezone: Asia/Ho_Chi_Minh
- Live metrics and platform state must be re-read before operational conclusions are made.

Do not store the internal account ID in this repository unless there is a specific operational need.

## Source-of-truth hierarchy

1. **Durable business and advertising decisions:** this repository.
2. **Live campaign configuration and performance:** Meta Ads.
3. **Brand-specific intent and state:** `brands/<brand>/`.
4. **Analysis and recommendations:** derived by comparing GitHub with live Meta Ads data.
5. **Conversation history:** supplementary only.

## Brand isolation rules

- Every campaign must declare exactly one brand unless explicitly documented as a cross-brand campaign.
- Every experiment must declare a brand.
- Performance baselines and KPI thresholds must be maintained separately by brand.
- Creative assets must be labeled by brand.
- Do not use Magasin Cup results to justify Magasin Coffee decisions, or vice versa, without an explicit cross-brand rationale.
- If a live Meta object cannot be confidently assigned to a brand, classify it as `UNRESOLVED` until evidence is available.

## Strategic objectives

No final brand-level business objective is approved yet.

Before a new launch plan is approved for either brand, document:
- primary business objective;
- conversion or lead objective;
- target market;
- budget envelope;
- KPI thresholds;
- measurement method.

## Governance rules

- Every campaign must have a documented objective and success criteria.
- Every experiment must state a hypothesis before launch.
- Budget changes should have a documented reason.
- Major strategic changes must be added to `decisions/decision-log.md`.
- Live Meta Ads state must be checked before recommending campaign changes.
- A recommendation is not an instruction to execute.
- Consequential changes to live Meta Ads require explicit user approval.
- Archived strategies and campaigns must remain available for historical reasoning.

## Naming conventions

### Campaign records

`META-COFFEE-C###-short-name.md`

`META-CUP-C###-short-name.md`

### Experiments

`EXP-COFFEE-###-short-name.md`

`EXP-CUP-###-short-name.md`

### Performance reviews

Weekly:
`YYYY-W##.md`

Monthly:
`YYYY-MM.md`

## Review protocol

When asked to “read the project again” or continue work:

1. Read this file.
2. Read `CURRENT_STATE.md`.
3. Read `brands/README.md`.
4. Read the relevant brand's `BRAND.md`, `CURRENT_STATE.md`, and `strategy.md`.
5. Read relevant shared strategy documents.
6. Read active/planned campaign documents.
7. Read open/relevant experiments.
8. Read recent decisions.
9. Read recent performance reviews.
10. Read current Meta Ads live data.
11. Identify mismatches between GitHub and Meta Ads.
12. Only then produce recommendations or execution proposals.

## Change policy

This file changes only when an enduring rule, scope, source-of-truth relationship, brand registry entry, or project-wide strategic decision changes.
