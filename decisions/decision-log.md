# Decision Log

This file records durable advertising decisions and why they were made.

## Format

### YYYY-MM-DD — Decision title

**Status:** Proposed / Approved / Reversed / Superseded

**Decision**

What was decided?

**Reason**

Why was it decided?

**Evidence**

What data, experiment, business constraint, or strategic consideration supported the decision?

**Impact**

What campaigns, budgets, targeting, creative, measurement, or process does this affect?

**Follow-up**

When should this decision be reviewed again?

---

### 2026-09-28 — Establish GitHub as Meta Ads strategic Source of Truth

**Status:** Approved

**Decision**

Use this repository as the durable Source of Truth for Meta Ads strategy, campaign plans, experiments, performance reviews, creative learnings, and decision history.

Use Meta Ads itself as the Source of Truth for live campaign configuration, delivery, and live performance metrics.

**Reason**

This separates durable project context from individual ChatGPT conversations and prevents advertising context from being mixed into unrelated repositories.

**Impact**

Future Meta Ads work should begin by reading this repository and current Meta Ads state before making recommendations.

---

### 2026-09-28 — Separate Magasin Coffee and Magasin Cup as independent advertising brands

**Status:** Approved

**Decision**

Operate Magasin Coffee and Magasin Cup as two separate brands inside the same Meta Ads project repository.

Every campaign, experiment, creative concept, performance review, and recommendation must identify one brand unless an explicit cross-brand exception is documented.

**Reason**

The two brands have different products, audiences, funnel behavior, campaign economics, and likely conversion paths. Combining their performance would produce misleading benchmarks and recommendations.

**Evidence**

The initial Meta Ads audit identified:
- Magasin Coffee via Instagram identity `magasincoffee`, with a local beverage awareness campaign.
- Magasin Cup via Instagram identity `th.xuonginlymagasincupcan`, with cup/product, printing, Messenger, and B2B-oriented campaigns.

**Impact**

Brand-specific files now live under:
- `brands/magasin-coffee/`
- `brands/magasin-cup/`

Campaign naming will use:
- `META-COFFEE-C###-...`
- `META-CUP-C###-...`

Performance benchmarks and KPI decisions must remain brand-specific.

**Follow-up**

Revisit only if the account structure changes materially or a legitimate cross-brand campaign is introduced.

---

### 2026-09-28 — Do not trust purchase/ROAS optimization until conversion tracking is verified

**Status:** Approved

**Decision**

Do not use current connector-reported purchase events or ROAS as the primary optimization basis for either brand until the conversion event source and value pipeline are verified.

**Reason**

The 90-day audit returned 13 omni purchase events for Magasin Cup but reported purchase conversion value of 0 VND. This is insufficient evidence of verified business sales.

**Impact**

- Magasin Cup should use qualified lead/message economics as the working measurement model.
- Magasin Coffee must define a measurable business outcome beyond awareness.
- CPA/ROAS targets remain unapproved.

**Follow-up**

Review immediately after conversion tracking and business-value attribution are verified.
