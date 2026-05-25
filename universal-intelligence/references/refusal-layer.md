# Evidence Refusal Layer

## Purpose

Block weak market findings before they become product direction. Use after `market-gap-research.md` and before routing a product, startup, or market-gap candidate into `the-forest-of-wrong.md`.

Default stance: the candidate is refused until it earns passage. The layer doubts the research, attacks the gap, and decides whether to route, narrow, rerun, or stop.

## Inputs Required

Do not run this layer on vibes. Require a completed evidence packet:

- Saturation map with named incumbents and substitutes.
- 3-5 gap hypotheses.
- Terrain pass sources.
- Doubt pass searches and strongest counterarguments.
- Survivor ledger for the current top candidate.

If any input is missing, return `RERUN: evidence packet incomplete` and specify the missing research.

## Routing Outcomes

Emit exactly one routing decision:

| Decision | Meaning | Next action |
|----------|---------|-------------|
| `ROUTE` | Candidate can feed Step 1 | Run Dogma & Heresy Mapping using the surviving market wedge |
| `NARROW` | Broad idea has a plausible subsegment but not enough precision | Re-scope segment/job and rerun terrain + doubt on the narrower version |
| `RERUN` | Research is too thin, stale, contradictory, or one-sided | Run another research/doubt pass before ideation |
| `REFUSE` | Candidate is saturated, unbuyable, unethical, legally unsafe, or built on false demand | Kill candidate and restart from a new market/segment |

Never route by enthusiasm. Route only when evidence survives refusal.

## Refusal Tests

Run these in order. The first hard failure controls the routing decision.

### R1 Evidence integrity

Refuse or rerun if claims are unsupported, stale, circular, source-poor, or based on absence of competitors. Current market claims need current sources when tools allow.

Minimum pass: at least one source-backed signal for pain/demand, one source-backed signal for market alternatives, and one explicit counter-signal.

### R2 Saturation pressure

Refuse if incumbents already serve the same narrow job with similar positioning, pricing, distribution, and trust.

Narrow if the broad category is crowded but a specific segment, compliance context, workflow, geography, buyer role, or timing shift remains poorly served.

### R3 Buyer reality

Refuse if no plausible buyer, budget holder, switching trigger, or urgent workflow cost appears. "People might like it" fails.

Minimum pass: named buyer/user pair, current workaround, switching moment, and reason the workaround hurts enough to test payment or adoption.

### R4 Wedge defensibility

Refuse if the only differentiation is "AI," nicer UI, lower price, generic automation, or brand taste.

Minimum pass: a wedge incumbents are structurally slow to copy: data access, trust channel, workflow custody, distribution route, compliance posture, underserved role, timing shock, or deliberately different operating model.

### R5 Counterevidence survival

Run at least one hostile explanation for why the idea is bad:

- Users do not care enough.
- Existing tools already solve it.
- The painful part is distribution/trust, not product.
- The segment lacks budget.
- Compliance, liability, or data access makes it impractical.
- The wedge collapses once an incumbent adds one feature.

If the hostile explanation is stronger than the positive case, `REFUSE` or `NARROW`.

### R6 Buildability and ethics

Refuse if the idea depends on deception, unlawful data access, harmful manipulation, unsafe regulated claims, or implementation assumptions the team cannot plausibly satisfy.

Rerun if feasibility is unknown but researchable.

## Refusal Memo Format

Before routing further, write a compact memo:

```text
DECISION: ROUTE | NARROW | RERUN | REFUSE
Candidate:
Why this almost fails:
Strongest evidence for:
Strongest evidence against:
Saturation verdict:
Buyer verdict:
Wedge verdict:
Riskiest assumption:
Kill criteria:
Next action:
```

For `ROUTE`, `Next action` must name which market dogma Step 1 should violate.

For `NARROW`, `RERUN`, or `REFUSE`, do not continue into the four-phase UI loop unless the user explicitly asks for speculative brainstorming despite the warning. If the user does override, label the output as speculative and preserve the refusal memo.

## Precision Rules

- Prefer "narrow and rerun" over broad optimism.
- Treat "market is fragmented" as an invitation to inspect buyer workflow, not proof of opportunity.
- Treat "users complain" as weak until linked to budget, urgency, or repeated workaround labor.
- Treat "incumbents ignore this" as ambiguous: it may signal a gap or a dead market.
- Treat all product ideas as provisional until a real validation probe runs.
