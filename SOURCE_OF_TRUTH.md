# Magasin Coffee Meta Ads — Source of Truth

Last updated: 2026-09-28

## Scope

This repository governs Meta advertising strategy for Magasin Coffee.

It does not govern the Magasin Coffee web application or unrelated engineering projects.

## Source-of-truth hierarchy

1. **Business and advertising decisions:** this repository.
2. **Live campaign configuration and performance:** Meta Ads.
3. **Analysis and recommended actions:** derived by comparing this repository with live Meta Ads data.
4. **Conversation history:** useful context, but never the durable source of truth when it conflicts with this repository or live platform state.

## Live platform

- Platform: Meta Ads
- Connected ad account: Vi Tran
- Live metrics and campaign state must be re-read from Meta Ads before operational conclusions are made.

## Strategic objective

Not yet approved.

The primary business objective, conversion objective, target market, budget envelope, and KPI thresholds must be documented before a launch plan is considered approved.

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

### Campaigns
`META-C###-short-name.md`

Example:
`META-C001-new-customer-acquisition.md`

### Experiments
`EXP-###-short-name.md`

Example:
`EXP-001-hook-test.md`

### Performance reviews
Weekly:
`YYYY-W##.md`

Monthly:
`YYYY-MM.md`

## Review protocol

When asked to “read the project again” or continue work:

1. Read this file.
2. Read `CURRENT_STATE.md`.
3. Read all relevant strategy documents.
4. Read active campaign documents.
5. Read open/relevant experiments.
6. Read recent decisions.
7. Read recent performance reviews.
8. Read current Meta Ads live data.
9. Identify any mismatch between GitHub and Meta Ads.
10. Only then produce recommendations or execution proposals.

## Change policy

This file changes only when an enduring rule, scope, source-of-truth relationship, or project-wide strategic decision changes.
