# Magasin Coffee Meta Ads

This repository is the strategic Source of Truth for Magasin Coffee advertising on Meta.

## Purpose

The repository stores:
- advertising strategy and operating rules;
- campaign plans and lifecycle records;
- experiment hypotheses and results;
- performance reviews;
- creative concepts and copy;
- decision history;
- instructions for ChatGPT to reload project context.

Live advertising metrics remain in Meta Ads. GitHub stores the durable reasoning, decisions, plans, and review history.

## Read order

When starting or resuming work, read in this order:

1. `SOURCE_OF_TRUTH.md`
2. `CURRENT_STATE.md`
3. Relevant files under `strategy/`
4. Relevant active campaign under `campaigns/active/`
5. Relevant experiment under `experiments/`
6. Recent entries in `decisions/decision-log.md`
7. Recent performance review under `performance/`

## Operating model

```text
GitHub = strategy + decisions + hypotheses + history
Meta Ads = live campaigns + live delivery + live performance
ChatGPT = analysis + planning + comparison + execution support
```

Any meaningful change to strategy, campaign structure, budget rules, targeting logic, creative direction, or success criteria should be recorded here.

## Repository structure

```text
.
├── README.md
├── SOURCE_OF_TRUTH.md
├── CURRENT_STATE.md
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
