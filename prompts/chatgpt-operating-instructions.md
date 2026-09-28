# ChatGPT Operating Instructions

## Purpose

These instructions define how ChatGPT should resume and operate the Magasin Coffee Meta Ads project.

## When the user says

Examples:
- "Đọc lại dự án Meta Ads"
- "Đọc source of truth rồi tiếp tục"
- "Kiểm tra Meta Ads theo chiến lược hiện tại"
- "Xem lại chiến dịch quảng cáo"

Follow the reload sequence below.

## Reload sequence

1. Read `SOURCE_OF_TRUTH.md`.
2. Read `CURRENT_STATE.md`.
3. Read all files in `strategy/` relevant to the request.
4. Read `campaigns/active/` and any planned campaign related to the request.
5. Read relevant files in `experiments/`.
6. Read recent entries in `decisions/decision-log.md`.
7. Read the latest weekly/monthly performance review when relevant.
8. Read live Meta Ads account state and current performance data.
9. Compare GitHub state with Meta Ads state.
10. Explicitly identify mismatches, stale assumptions, missing data, and unresolved decisions.
11. Produce analysis and proposed actions.
12. Do not make consequential Meta Ads changes without explicit user approval.
13. After an approved strategic or operational change, update the relevant GitHub records so the project remains coherent.

## Source priority

When sources conflict:

- live Meta Ads wins for current platform state and metrics;
- `SOURCE_OF_TRUTH.md` wins for enduring project rules;
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

## Update discipline

After meaningful work, update:
- `CURRENT_STATE.md` for current priorities/state;
- campaign file for campaign-specific changes;
- experiment file for experiment status/results;
- performance review for measured outcomes;
- decision log for durable strategic decisions.

## Safety

Before launch, pause, enable, budget changes, targeting changes, creative replacement, or other consequential live mutations:
- re-read current Meta Ads state;
- summarize the exact proposed change;
- obtain explicit approval;
- execute only the approved scope;
- verify the result;
- record the outcome.
