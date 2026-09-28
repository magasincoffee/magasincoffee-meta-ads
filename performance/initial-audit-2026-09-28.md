# Initial Meta Ads Baseline Audit — 2026-09-28

Audit date: 2026-09-28
Data window: last 90 days including audit date
Connected account: Vi Tran
Currency: VND
Timezone: Asia/Ho_Chi_Minh

## Scope

This audit establishes the first GitHub baseline for the two brands sharing the Meta Ads account:

- Magasin Coffee
- Magasin Cup

Brand classification was based on observed Instagram identity, campaign/ad naming, and ad content.

## Magasin Coffee

Confirmed identity: `magasincoffee`

| Campaign | Objective | Current campaign state | Spend | Impressions | Clicks | CTR | CPC |
|---|---|---|---:|---:|---:|---:|---:|
| Chiến dịch Mức độ nhận biết mới | OUTCOME_AWARENESS | PAUSED | 1,712,107 | 366,062 | 1,999 | 0.55% | 856.48 |

Creative evidence:
- “LATTE 1 LÍT ĐỒNG GIÁ 25K”
- student/value positioning
- local Magasin Coffee availability

Interpretation:
- efficient awareness delivery is visible;
- no verified business conversion outcome is established by the reviewed fields.

## Magasin Cup

Confirmed identity: `th.xuonginlymagasincupcan`

| Campaign | Observed state | Spend | Impressions | Clicks | CTR | CPC |
|---|---|---:|---:|---:|---:|---:|
| LY 700ML | Ad archived | 2,472,373 | 48,957 | 830 | 1.70% | 2,978.76 |
| TIN NHẮN 07/08/2026 | PAUSED | 2,023,402 | 43,636 | 505 | 1.16% | 4,006.74 |
| Ly 700ml - ship toàn quốc 690 đồng | PAUSED | 1,150,834 | 8,095 | 254 | 3.14% | 4,530.84 |
| 1300 ml lần 2 | Ad archived | 666,089 | 13,554 | 268 | 1.98% | 2,485.41 |
| Chiến dịch Lượt tương tác mới | Ad archived | 493,900 | 11,490 | 245 | 2.13% | 2,015.92 |
| Chiến dịch tin nhắn thiết kế riêng cho bạn 13/7/2026 Chiến dịch | Ad archived | 481,455 | 12,451 | 185 | 1.49% | 2,602.46 |
| Chiến dịch tin nhắn thiết kế riêng cho bạn 5/8/2026 Chiến dịch | Ad archived | 181,906 | 3,312 | 48 | 1.45% | 3,789.71 |

Aggregate:
- Spend: 7,469,959 VND
- Impressions: 141,495
- Clicks: 2,335
- CTR: 1.65%
- CPC: 3,199.13 VND
- CPM: 52,793.10 VND

Connector-reported omni purchases: 13
Reported purchase value: 0 VND

Interpretation:
- the account is functioning more like a message/lead acquisition system than a verified ecommerce system;
- purchase/ROAS optimization is not safe until tracking is validated.

## Current active-object anomaly

Two Cup ads were returned as ACTIVE with no insights in the 90-day query:
- `LY700 - 690 - DONG NAI`
- `LY700 - 690 - LAM DONG`

Their parent campaign/ad set context was not returned in the no-insight rows.

Treat their serving status as unresolved until a follow-up live check confirms the parent hierarchy.

## Cross-account findings

1. Campaign naming is inconsistent and does not reliably encode brand.
2. Coffee and Cup require separate KPI systems.
3. Conversion measurement is the highest-priority technical/business gap.
4. Cup should likely optimize around qualified leads/messages until revenue tracking is reliable.
5. Coffee needs a primary business outcome beyond awareness before a new campaign is approved.
6. No live Meta changes were made during this audit.
