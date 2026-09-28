# Current Advertising State

Last reviewed: 2026-09-28
Audit window: last 90 days including 2026-09-28

## Project status

The repository now governs two brands separately:

- Magasin Coffee
- Magasin Cup

The first live Meta Ads baseline audit has been completed.

No new campaign launch strategy or budget plan is marked approved yet.

## Meta Ads connection

- Connected platform: Meta Ads
- Connected ad account: Vi Tran
- Account status: ACTIVE
- Currency: VND
- Timezone: Asia/Ho_Chi_Minh

## 90-day brand baseline

### Magasin Coffee

Observed identity: `magasincoffee`

Observed campaign with spend:
- `Chiến dịch Mức độ nhận biết mới`
- Objective: `OUTCOME_AWARENESS`
- Current campaign status: PAUSED
- Observed daily budget: 50,000 VND
- Spend: 1,712,107 VND
- Impressions: 366,062
- Clicks: 1,999
- CTR (all clicks / impressions): 0.55%
- CPC (all clicks): 856.48 VND
- CPM: 4,677.10 VND

Observed creative theme:
- 1-liter latte
- 25K price point
- student-oriented messaging
- local Magasin Coffee availability

No currently delivering Coffee campaign was confirmed in this audit.

### Magasin Cup

Observed identity: `th.xuonginlymagasincupcan`

Recent campaigns with spend are centered on:
- 700ml cups;
- 1300ml cups;
- logo printing;
- custom design;
- Messenger acquisition;
- nationwide or geographic sales.

90-day aggregate across Cup-attributed campaigns with spend:
- Spend: 7,469,959 VND
- Impressions: 141,495
- Clicks: 2,335
- CTR (all clicks / impressions): 1.65%
- CPC (all clicks): 3,199.13 VND
- CPM: 52,793.10 VND

Connector-reported omni purchase events across these rows: 13.
Reported purchase conversion value: 0 VND.

**Measurement warning:** do not use those purchase events for CPA or ROAS decisions until the conversion source and event quality are verified.

Current live-object observation:
- `LY700 - 690 - DONG NAI`: ad status ACTIVE, no insights in the 90-day query.
- `LY700 - 690 - LAM DONG`: ad status ACTIVE, no insights in the 90-day query.

The connector did not return parent campaign/ad set context for those two no-insight objects, so current serving status must be re-verified before any operational change.

## Approved strategy

None yet.

## Current budget policy

No account-level or brand-level spend ceiling has been approved in this repository.

## Current KPI policy

No final target KPI has been approved.

Observed historical baselines are recorded in `performance/benchmarks.md`, but they are not targets.

## Current priorities

### Shared

1. Enforce brand labeling for every future campaign and experiment.
2. Verify conversion tracking before using CPA/ROAS as decision metrics.
3. Standardize campaign naming by brand.
4. Establish explicit budget ceilings before launch or scaling.

### Magasin Coffee

1. Confirm the primary business outcome: store visits, messages, orders, or another measurable result.
2. Decide whether awareness remains the primary objective or becomes only a supporting layer.
3. Define local audience/geographic strategy.
4. Build a structured creative test around offer, product, and customer segment.

### Magasin Cup

1. Treat qualified lead/message acquisition as the likely working measurement path until purchase tracking is verified.
2. Separate geographic tests from creative tests.
3. Define lead quality and cost-per-qualified-lead measurement.
4. Review the two ACTIVE no-insight ads before deciding whether to retain, relaunch, or replace them.

## Active experiments

None documented yet.

## Known gaps

- No approved business objective per brand.
- No verified primary conversion event per brand.
- No approved budget envelope.
- No approved KPI thresholds.
- No qualified-lead definition for Magasin Cup.
- No store-visit/order measurement definition for Magasin Coffee.
- Active Cup ad parent campaign context needs re-verification.

## Next review

After brand objectives and measurement rules are approved, create the first planned campaign architecture for each brand.
