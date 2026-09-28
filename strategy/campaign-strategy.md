# Campaign Strategy

Status: Draft

## Architecture principles

Use the smallest campaign structure that can answer the business question reliably.

Prefer:
- fewer campaigns;
- fewer ad sets;
- enough budget per test;
- clear separation between materially different objectives or audiences.

Avoid:
- duplicated ad sets without a hypothesis;
- splitting small budgets across too many cells;
- changing multiple variables at once without recording it;
- optimizing to weak proxy metrics when the business outcome is measurable.

## Default campaign design

A campaign document should define:

- campaign ID and name;
- business objective;
- Meta objective;
- conversion location/event;
- audience role;
- geographic scope;
- placements;
- budget model;
- creative set;
- exclusions;
- hypothesis;
- primary KPI;
- guardrail KPIs;
- start criteria;
- stop criteria;
- scale criteria.

## Lifecycle

1. Planned
2. Approved
3. Active
4. Measuring
5. Iterating
6. Archived

The GitHub campaign record should always show the current lifecycle state.

## Change discipline

A material change is one that can invalidate interpretation of performance, including:
- budget shifts;
- audience changes;
- optimization event changes;
- major creative swaps;
- offer changes;
- landing destination changes.

Material changes must be logged in the campaign file and, when strategic, in the decision log.
