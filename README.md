# Magasin Brands Meta Ads

This repository is the strategic Source of Truth for Meta advertising across two brands:

1. **Magasin Coffee**
2. **Magasin Cup**

Both brands currently operate through the same connected Meta Ads account, but their strategy, campaign intent, creative, measurement, and performance must be analyzed separately.

## Purpose

The repository stores:
- shared advertising governance and operating rules;
- brand-specific strategy and current state;
- campaign plans and lifecycle records;
- experiment hypotheses and results;
- performance reviews;
- creative concepts and copy;
- decision history;
- instructions for ChatGPT to reload project context.

Live advertising metrics remain in Meta Ads. GitHub stores durable reasoning, decisions, plans, and review history.

## Read order

When starting or resuming work, read in this order:

1. `SOURCE_OF_TRUTH.md`
2. `CURRENT_STATE.md`
3. `brands/README.md`
4. The relevant brand files under `brands/<brand>/`
5. Relevant shared files under `strategy/`
6. Relevant active/planned campaign files
7. Relevant experiments
8. Recent entries in `decisions/decision-log.md`
9. Recent performance review under `performance/`
10. Current live Meta Ads data

## Operating model

```text
GitHub = strategy + decisions + hypotheses + history
Meta Ads = live campaigns + live delivery + live performance
ChatGPT = analysis + planning + comparison + execution support
```

## Brand isolation rule

Every campaign, experiment, creative concept, KPI review, and recommendation must identify its brand.

Do not combine Magasin Coffee and Magasin Cup performance into one decision unless the user explicitly asks for an account-level view.

## Repository structure

```text
.
├── README.md
├── SOURCE_OF_TRUTH.md
├── CURRENT_STATE.md
├── brands/
│   ├── magasin-coffee/
│   └── magasin-cup/
├── strategy/
├── campaigns/
│   ├── planned/
│   ├── active/
│   └── archived/
├── experiments/
├── performance/
│   ├── weekly/
│   └── monthly/
├── creatives/
│   ├── concepts/
│   └── copy/
├── decisions/
└── prompts/
```

## Safety rule

Do not activate, pause, materially change budgets, or otherwise mutate live Meta Ads campaigns solely because a document suggests doing so. Compare the repository with live Meta Ads first and obtain explicit approval for consequential changes.
